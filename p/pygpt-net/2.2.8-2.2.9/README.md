# Comparing `tmp/pygpt_net-2.2.8.tar.gz` & `tmp/pygpt_net-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygpt_net-2.2.8.tar", max compression
+gzip compressed data, was "pygpt_net-2.2.9.tar", max compression
```

## Comparing `pygpt_net-2.2.8.tar` & `pygpt_net-2.2.9.tar`

### file list

```diff
@@ -1,869 +1,869 @@
--rwxr-xr-x   0        0        0    59583 2024-05-02 17:16:19.056982 pygpt_net-2.2.8/CHANGELOG.md
--rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.8/LICENSE
--rwxr-xr-x   0        0        0   139884 2024-05-02 17:15:54.645157 pygpt_net-2.2.8/README.md
--rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.8/icon.png
--rw-r--r--   0        0        0     2979 2024-05-02 17:16:47.776781 pygpt_net-2.2.8/pyproject.toml
--rwxr-xr-x   0        0        0    58551 2024-05-02 17:16:17.700991 pygpt_net-2.2.8/src/pygpt_net/CHANGELOG.txt
--rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.8/src/pygpt_net/LICENSE
--rwxr-xr-x   0        0        0     1024 2024-05-02 17:18:08.492251 pygpt_net-2.2.8/src/pygpt_net/__init__.py
--rwxr-xr-x   0        0        0    14447 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/app.py
--rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/config.py
--rwxr-xr-x   0        0        0     3839 2024-05-02 17:09:01.677147 pygpt_net-2.2.8/src/pygpt_net/container.py
--rwxr-xr-x   0        0        0     5333 2024-05-02 17:09:01.681147 pygpt_net-2.2.8/src/pygpt_net/controller/__init__.py
--rwxr-xr-x   0        0        0     2209 2024-05-02 18:21:41.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/__init__.py
--rwxr-xr-x   0        0        0     9179 2024-05-02 17:49:27.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/control.py
--rwxr-xr-x   0        0        0    11692 2024-05-02 18:21:41.000000 pygpt_net-2.2.8/src/pygpt_net/controller/access/voice.py
--rw-r--r--   0        0        0     3823 2024-05-02 17:09:01.877145 pygpt_net-2.2.8/src/pygpt_net/controller/agent/__init__.py
--rw-r--r--   0        0        0     1748 2024-05-02 17:09:01.797146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/common.py
--rw-r--r--   0        0        0     1407 2024-05-02 17:09:01.761146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/experts.py
--rw-r--r--   0        0        0     6904 2024-05-02 17:09:01.801146 pygpt_net-2.2.8/src/pygpt_net/controller/agent/flow.py
--rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/__init__.py
--rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/batch.py
--rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/editor.py
--rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/files.py
--rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/store.py
--rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/assistant/threads.py
--rwxr-xr-x   0        0        0    15661 2024-05-02 17:49:27.617904 pygpt_net-2.2.8/src/pygpt_net/controller/attachment.py
--rw-r--r--   0        0        0     6560 2024-05-02 17:09:01.665147 pygpt_net-2.2.8/src/pygpt_net/controller/audio/__init__.py
--rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/calendar/__init__.py
--rw-r--r--   0        0        0     8585 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/controller/calendar/note.py
--rwxr-xr-x   0        0        0    13013 2024-05-02 17:09:01.793146 pygpt_net-2.2.8/src/pygpt_net/controller/camera.py
--rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.8/src/pygpt_net/controller/chat/__init__.py
--rwxr-xr-x   0        0        0    11749 2024-05-02 17:09:01.809146 pygpt_net-2.2.8/src/pygpt_net/controller/chat/common.py
--rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/chat/files.py
--rwxr-xr-x   0        0        0     6533 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/chat/image.py
--rwxr-xr-x   0        0        0    10650 2024-05-02 17:09:01.713147 pygpt_net-2.2.8/src/pygpt_net/controller/chat/input.py
--rwxr-xr-x   0        0        0    11366 2024-05-02 17:09:01.693147 pygpt_net-2.2.8/src/pygpt_net/controller/chat/output.py
--rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.8/src/pygpt_net/controller/chat/render.py
--rw-r--r--   0        0        0    13022 2024-05-02 17:09:01.757146 pygpt_net-2.2.8/src/pygpt_net/controller/chat/text.py
--rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.8/src/pygpt_net/controller/chat/vision.py
--rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.8/src/pygpt_net/controller/command.py
--rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/controller/config/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/__init__.py
--rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/checkbox.py
--rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/cmd.py
--rw-r--r--   0        0        0     3237 2024-05-02 10:44:22.869251 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/combo.py
--rw-r--r--   0        0        0     6657 2024-05-02 14:53:21.198368 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/dictionary.py
--rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/input.py
--rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/slider.py
--rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.8/src/pygpt_net/controller/config/field/textarea.py
--rw-r--r--   0        0        0     8222 2024-05-02 17:09:01.869145 pygpt_net-2.2.8/src/pygpt_net/controller/config/placeholder.py
--rw-r--r--   0        0        0    30255 2024-05-02 17:09:01.845145 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/__init__.py
--rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/common.py
--rwxr-xr-x   0        0        0     7529 2024-05-02 17:54:44.930189 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/extra.py
--rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.8/src/pygpt_net/controller/ctx/summarizer.py
--rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/debug/__init__.py
--rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/__init__.py
--rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/confirm.py
--rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/debug.py
--rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/info.py
--rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/controller/files.py
--rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.8/src/pygpt_net/controller/finder.py
--rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/idx/__init__.py
--rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.8/src/pygpt_net/controller/idx/common.py
--rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.8/src/pygpt_net/controller/idx/indexer.py
--rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.8/src/pygpt_net/controller/idx/settings.py
--rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/lang/__init__.py
--rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/controller/lang/custom.py
--rw-r--r--   0        0        0    20280 2024-05-02 17:09:01.729147 pygpt_net-2.2.8/src/pygpt_net/controller/lang/mapping.py
--rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.8/src/pygpt_net/controller/lang/plugins.py
--rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.8/src/pygpt_net/controller/lang/settings.py
--rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.8/src/pygpt_net/controller/launcher.py
--rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/layout.py
--rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/mode.py
--rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/controller/model/__init__.py
--rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.8/src/pygpt_net/controller/model/editor.py
--rwxr-xr-x   0        0        0    13052 2024-05-02 17:09:01.821145 pygpt_net-2.2.8/src/pygpt_net/controller/notepad.py
--rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/painter/__init__.py
--rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.8/src/pygpt_net/controller/painter/capture.py
--rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.8/src/pygpt_net/controller/painter/common.py
--rw-r--r--   0        0        0    13977 2024-05-02 17:09:01.753146 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/__init__.py
--rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/presets.py
--rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.8/src/pygpt_net/controller/plugins/settings.py
--rwxr-xr-x   0        0        0    17127 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/__init__.py
--rwxr-xr-x   0        0        0    16058 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/editor.py
--rw-r--r--   0        0        0     4937 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/presets/experts.py
--rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/settings/__init__.py
--rwxr-xr-x   0        0        0    15241 2024-05-02 17:09:01.841145 pygpt_net-2.2.8/src/pygpt_net/controller/settings/editor.py
--rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/controller/settings/profile.py
--rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/controller/settings/workdir.py
--rwxr-xr-x   0        0        0     6308 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/theme/__init__.py
--rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/controller/theme/common.py
--rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/controller/theme/markdown.py
--rw-r--r--   0        0        0     4631 2024-04-24 02:39:32.054775 pygpt_net-2.2.8/src/pygpt_net/controller/theme/menu.py
--rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/controller/theme/nodes.py
--rw-r--r--   0        0        0     6934 2024-05-02 17:09:01.849145 pygpt_net-2.2.8/src/pygpt_net/controller/ui/__init__.py
--rw-r--r--   0        0        0     6663 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/controller/ui/mode.py
--rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/controller/ui/vision.py
--rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.8/src/pygpt_net/core/__init__.py
--rw-r--r--   0        0        0      874 2024-05-02 17:09:01.865145 pygpt_net-2.2.8/src/pygpt_net/core/access/__init__.py
--rw-r--r--   0        0        0     2351 2024-05-02 17:09:01.709147 pygpt_net-2.2.8/src/pygpt_net/core/access/actions.py
--rwxr-xr-x   0        0        0     2902 2024-05-02 18:17:27.000000 pygpt_net-2.2.8/src/pygpt_net/core/access/events.py
--rw-r--r--   0        0        0     3397 2024-05-02 17:09:01.749146 pygpt_net-2.2.8/src/pygpt_net/core/access/shortcuts.py
--rw-r--r--   0        0        0    10590 2024-05-02 17:43:40.444809 pygpt_net-2.2.8/src/pygpt_net/core/access/voice.py
--rw-r--r--   0        0        0     1382 2024-05-02 17:09:01.653148 pygpt_net-2.2.8/src/pygpt_net/core/agents/__init__.py
--rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/core/assistants/__init__.py
--rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/core/assistants/files.py
--rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/core/assistants/store.py
--rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.8/src/pygpt_net/core/attachments.py
--rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/core/audio.py
--rw-r--r--   0        0        0     7483 2024-05-02 17:09:01.725147 pygpt_net-2.2.8/src/pygpt_net/core/bridge.py
--rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/core/calendar/__init__.py
--rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.8/src/pygpt_net/core/camera.py
--rw-r--r--   0        0        0     3330 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/__init__.py
--rw-r--r--   0        0        0     4988 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/chat.py
--rw-r--r--   0        0        0     5413 2024-05-01 18:08:40.474948 pygpt_net-2.2.8/src/pygpt_net/core/chain/completion.py
--rwxr-xr-x   0        0        0    10538 2024-05-02 17:09:01.861145 pygpt_net-2.2.8/src/pygpt_net/core/command.py
--rwxr-xr-x   0        0        0    35701 2024-05-02 17:09:01.661147 pygpt_net-2.2.8/src/pygpt_net/core/ctx/__init__.py
--rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/ctx/idx.py
--rw-r--r--   0        0        0    15975 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/db/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/db/viewer.py
--rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.8/src/pygpt_net/core/debug/__init__.py
--rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.8/src/pygpt_net/core/debug/agent.py
--rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.8/src/pygpt_net/core/debug/assistants.py
--rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/attachments.py
--rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/debug/config.py
--rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.8/src/pygpt_net/core/debug/context.py
--rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.8/src/pygpt_net/core/debug/db.py
--rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/core/debug/indexes.py
--rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/models.py
--rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/plugins.py
--rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/presets.py
--rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.8/src/pygpt_net/core/debug/ui.py
--rwxr-xr-x   0        0        0    10010 2024-05-02 17:09:01.741146 pygpt_net-2.2.8/src/pygpt_net/core/dispatcher.py
--rw-r--r--   0        0        0    10014 2024-05-02 17:09:01.669147 pygpt_net-2.2.8/src/pygpt_net/core/experts/__init__.py
--rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/__init__.py
--rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/actions.py
--rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/editor.py
--rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/types.py
--rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/filesystem/url.py
--rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/core/history.py
--rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/__init__.py
--rwxr-xr-x   0        0        0    13030 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/idx/chat.py
--rw-r--r--   0        0        0     2443 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/idx/context.py
--rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/indexing.py
--rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.8/src/pygpt_net/core/idx/llm.py
--rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.8/src/pygpt_net/core/idx/metadata.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/__init__.py
--rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/ctx.py
--rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/external.py
--rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/core/idx/types/files.py
--rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.8/src/pygpt_net/core/idx/worker.py
--rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.8/src/pygpt_net/core/image.py
--rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.8/src/pygpt_net/core/info.py
--rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.8/src/pygpt_net/core/installer.py
--rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.8/src/pygpt_net/core/llm/__init__.py
--rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.8/src/pygpt_net/core/locale.py
--rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/core/models.py
--rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/core/modes.py
--rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/notepad.py
--rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/core/platforms.py
--rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.8/src/pygpt_net/core/plugins.py
--rw-r--r--   0        0        0    12366 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/presets.py
--rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.8/src/pygpt_net/core/profile.py
--rw-r--r--   0        0        0     4529 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/prompt/__init__.py
--rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/core/prompt/template.py
--rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.8/src/pygpt_net/core/render/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/render/base.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/__init__.py
--rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/parser.py
--rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/renderer.py
--rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.8/src/pygpt_net/core/render/plain/__init__.py
--rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/render/plain/renderer.py
--rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.8/src/pygpt_net/core/render/web/__init__.py
--rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.8/src/pygpt_net/core/render/web/parser.py
--rwxr-xr-x   0        0        0    43236 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/render/web/renderer.py
--rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/core/settings.py
--rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/__init__.py
--rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/finder.py
--rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.8/src/pygpt_net/core/text/utils.py
--rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/core/text/web_finder.py
--rwxr-xr-x   0        0        0    14472 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/core/tokens.py
--rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.8/src/pygpt_net/core/updater/__init__.py
--rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/core/web.py
--rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.8/src/pygpt_net/core/worker.py
--rw-r--r--   0        0        0    65201 2024-05-02 09:05:10.390389 pygpt_net-2.2.8/src/pygpt_net/data/audio/click_off.mp3
--rw-r--r--   0        0        0    65201 2024-05-02 09:04:45.466493 pygpt_net-2.2.8/src/pygpt_net/data/audio/click_on.mp3
--rw-r--r--   0        0        0    32256 2024-05-02 12:19:15.320423 pygpt_net-2.2.8/src/pygpt_net/data/audio/ok.mp3
--rwxr-xr-x   0        0        0    15381 2024-05-02 17:23:01.538643 pygpt_net-2.2.8/src/pygpt_net/data/config/config.json
--rwxr-xr-x   0        0        0    20573 2024-05-02 17:17:50.696364 pygpt_net-2.2.8/src/pygpt_net/data/config/models.json
--rw-r--r--   0        0        0     1595 2024-05-02 17:17:45.868395 pygpt_net-2.2.8/src/pygpt_net/data/config/modes.json
--rwxr-xr-x   0        0        0      528 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/batman_and_joker.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.agent.json
--rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.assistant.json
--rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.chat.json
--rwxr-xr-x   0        0        0      436 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.completion.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.expert.json
--rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.img.json
--rwxr-xr-x   0        0        0      433 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.langchain.json
--rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.llama_index.json
--rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/current.vision.json
--rwxr-xr-x   0        0        0      552 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/dalle_white_cat.json
--rw-r--r--   0        0        0      474 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_agent.json
--rw-r--r--   0        0        0      683 2024-05-01 18:08:40.478948 pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_expert.json
--rwxr-xr-x   0        0        0    36092 2024-05-02 16:55:04.321108 pygpt_net-2.2.8/src/pygpt_net/data/config/settings.json
--rw-r--r--   0        0        0      870 2024-05-02 06:04:41.700908 pygpt_net-2.2.8/src/pygpt_net/data/config/settings_section.json
--rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/fix_windows.css
--rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.css
--rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.dark.css
--rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.light.css
--rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/style.css
--rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.8/src/pygpt_net/data/css/style.dark.css
--rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.8/src/pygpt_net/data/css/style.light.css
--rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.8/src/pygpt_net/data/css/web.css
--rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.8/src/pygpt_net/data/css/web.dark.css
--rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.8/src/pygpt_net/data/css/web.light.css
--rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
--rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
--rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
--rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
--rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
--rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
--rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
--rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
--rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
--rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
--rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/OFL.txt
--rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
--rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
--rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
--rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
--rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
--rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
--rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
--rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
--rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
--rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
--rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
--rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
--rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
--rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
--rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
--rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
--rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
--rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
--rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
--rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
--rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
--rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
--rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
--rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
--rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/icon.ico
--rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/icon.png
--rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_busy.ico
--rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_error.ico
--rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_idle.ico
--rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/abc.svg
--rw-r--r--   0        0        0      360 2024-05-02 14:44:36.720121 pygpt_net-2.2.8/src/pygpt_net/data/icons/accessibility.svg
--rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add.svg
--rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_circle.svg
--rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_folder.svg
--rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/add_library.svg
--rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/alarm.svg
--rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/apps.svg
--rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/asterisk.svg
--rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/attachment.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/attachments.svg
--rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/back.svg
--rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/backspace.svg
--rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/block.svg
--rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/bookmark.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/brush.svg
--rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/build.svg
--rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/calendar.svg
--rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/camera.svg
--rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/audio.png
--rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/copy.png
--rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/delete.png
--rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/edit.png
--rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/join.png
--rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/reload.png
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/chat.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/check.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/check_circle.svg
--rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/checklist.svg
--rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/circle.svg
--rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/clear.svg
--rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/clock.svg
--rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/close.svg
--rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/close_circle.svg
--rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/code.svg
--rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/computer.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/copy.svg
--rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/crop.svg
--rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/cut.svg
--rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.8/src/pygpt_net/data/icons/db.svg
--rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/delete.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/done.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/download.svg
--rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/draft.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/drag.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/edit.svg
--rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/emergency.svg
--rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/equalizer.svg
--rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/error.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/event_available.svg
--rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/expand.svg
--rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fast_forward.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fast_rewind.svg
--rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/favorite.svg
--rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/folder.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/folder_filled.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/forward.svg
--rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/full.svg
--rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/fullscreen.svg
--rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/grid.svg
--rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/hearing.svg
--rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/help.svg
--rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/history.svg
--rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/home.svg
--rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/home_filled.svg
--rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/image.svg
--rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/info.svg
--rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/input.svg
--rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/key.svg
--rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/keyboard.svg
--rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/language.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/list.svg
--rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/lock.svg
--rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/logout.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/map.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/memory.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/menu.svg
--rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mic.svg
--rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mic_off.svg
--rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/more_horizontal.svg
--rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/mute.svg
--rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/open_tab.svg
--rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/palette.svg
--rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/paste.svg
--rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pause.svg
--rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pause_circle.svg
--rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/photos.svg
--rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/pin.svg
--rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/play.svg
--rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/play_pause.svg
--rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/playlist_add.svg
--rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/power.svg
--rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/print.svg
--rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/public_filled.svg
--rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.8/src/pygpt_net/data/icons/redo.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/reload.svg
--rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/repeat.svg
--rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/replay.svg
--rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/resize.svg
--rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/robot.svg
--rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/router.svg
--rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/save.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/schedule.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/screenshot.svg
--rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/search.svg
--rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/security.svg
--rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/sensors.svg
--rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/settings.svg
--rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/settings_filled.svg
--rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/share.svg
--rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/shedule.svg
--rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/sort.svg
--rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/stack.svg
--rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/stacks.svg
--rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.8/src/pygpt_net/data/icons/star.svg
--rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/stop.svg
--rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/stop_circle.svg
--rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/sync.svg
--rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/tag.svg
--rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/task.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/terminal.svg
--rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/text.svg
--rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/textfile.svg
--rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/timer.svg
--rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/today.svg
--rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/tune.svg
--rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/undo.svg
--rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/update.svg
--rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/updater.svg
--rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/upload.svg
--rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/video.svg
--rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/view.svg
--rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/voice.svg
--rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/volume.svg
--rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/warning.svg
--rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/webcam.svg
--rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.8/src/pygpt_net/data/icons/webcam_off.svg
--rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/width.svg
--rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/window.svg
--rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/work.svg
--rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/zoom_in.svg
--rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.8/src/pygpt_net/data/icons/zoom_out.svg
--rwxr-xr-x   0        0        0    52116 2024-05-02 17:53:00.806146 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.de.ini
--rwxr-xr-x   0        0        0    59899 2024-05-02 17:51:12.166053 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.en.ini
--rwxr-xr-x   0        0        0    52304 2024-05-02 17:53:33.870164 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.es.ini
--rwxr-xr-x   0        0        0    54105 2024-05-02 17:53:10.970152 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.fr.ini
--rwxr-xr-x   0        0        0    51291 2024-05-02 17:53:22.782159 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.it.ini
--rwxr-xr-x   0        0        0    51375 2024-05-02 17:52:46.058137 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.pl.ini
--rwxr-xr-x   0        0        0    71739 2024-05-02 17:39:36.711163 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.uk.ini
--rwxr-xr-x   0        0        0    54448 2024-05-02 17:53:45.590170 pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.zh.ini
--rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.en.ini
--rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.pl.ini
--rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini
--rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
--rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini
--rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
--rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
--rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
--rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
--rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
--rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
--rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
--rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
--rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
--rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
--rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
--rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
--rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
--rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
--rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
--rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.en.ini
--rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini
--rw-r--r--   0        0        0       99 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.experts.en.ini
--rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
--rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
--rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
--rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
--rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
--rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
--rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
--rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
--rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.en.ini
--rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini
--rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.8/src/pygpt_net/data/logo.png
--rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/data/prompts.csv
--rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.8/src/pygpt_net/data/win32/README.rtf
--rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/USER-LICENSE.rtf
--rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/pygpt.aip
--rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.8/src/pygpt_net/data/win32/qt.conf
--rw-r--r--   0        0        0    21910 2024-05-02 14:46:17.971808 pygpt_net-2.2.8/src/pygpt_net/icons.qrc
--rw-r--r--   0        0        0    91076 2024-05-02 14:46:18.099807 pygpt_net-2.2.8/src/pygpt_net/icons_rc.py
--rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.8/src/pygpt_net/item/__init__.py
--rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/item/assistant.py
--rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/item/attachment.py
--rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/calendar_note.py
--rw-r--r--   0        0        0    12376 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/item/ctx.py
--rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/index.py
--rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.8/src/pygpt_net/item/mode.py
--rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/model.py
--rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/item/notepad.py
--rw-r--r--   0        0        0     4680 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/item/preset.py
--rwxr-xr-x   0        0        0     8362 2024-05-02 17:09:01.717147 pygpt_net-2.2.8/src/pygpt_net/launcher.py
--rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231227152900.py
--rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231230095000.py
--rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231231230000.py
--rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240106060000.py
--rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240107060000.py
--rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240222160000.py
--rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240223050000.py
--rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240303190000.py
--rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240408180000.py
--rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240426050000.py
--rw-r--r--   0        0        0     1052 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240501030000.py
--rw-r--r--   0        0        0     1974 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/migrations/__init__.py
--rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.8/src/pygpt_net/migrations/base.py
--rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.8/src/pygpt_net/plugin/__init__.py
--rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/plugin/agent/__init__.py
--rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/__init__.py
--rw-r--r--   0        0        0     4929 2024-05-02 17:09:01.813145 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/simple.py
--rwxr-xr-x   0        0        0    11433 2024-05-02 17:09:01.781146 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/worker.py
--rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/__init__.py
--rw-r--r--   0        0        0     2340 2024-05-02 17:09:01.785146 pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/worker.py
--rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/plugin/base.py
--rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/__init__.py
--rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/worker.py
--rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
--rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
--rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
--rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/__init__.py
--rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/worker.py
--rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/__init__.py
--rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/worker.py
--rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/__init__.py
--rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/worker.py
--rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/__init__.py
--rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/worker.py
--rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/__init__.py
--rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/websearch.py
--rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/worker.py
--rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.8/src/pygpt_net/plugin/crontab/__init__.py
--rwxr-xr-x   0        0        0     2475 2024-05-02 17:09:01.789146 pygpt_net-2.2.8/src/pygpt_net/plugin/experts/__init__.py
--rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.8/src/pygpt_net/plugin/extra_prompt/__init__.py
--rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/__init__.py
--rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/worker.py
--rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/plugin/openai_dalle/__init__.py
--rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.8/src/pygpt_net/plugin/openai_vision/__init__.py
--rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.8/src/pygpt_net/plugin/real_time/__init__.py
--rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.8/src/pygpt_net/provider/__init__.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/__init__.py
--rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/base.py
--rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
--rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
--rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py
--rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper.py
--rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/__init__.py
--rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/base.py
--rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/eleven_labs.py
--rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/google_tts.py
--rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py
--rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/openai_tts.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/__init__.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/__init__.py
--rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/base.py
--rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/json_file.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/base.py
--rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
--rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
--rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
--rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/base.py
--rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
--rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
--rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
--rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
--rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/__init__.py
--rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/base.py
--rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/__init__.py
--rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/base.py
--rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
--rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/__init__.py
--rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/base.py
--rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/json_file.py
--rwxr-xr-x   0        0        0    78799 2024-05-02 17:22:33.110782 pygpt_net-2.2.8/src/pygpt_net/provider/core/config/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/__init__.py
--rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/base.py
--rw-r--r--   0        0        0     9815 2024-05-02 17:09:01.689147 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
--rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
--rw-r--r--   0        0        0    33830 2024-05-02 17:09:01.873145 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
--rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
--rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/json_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/__init__.py
--rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/base.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/patch.py
--rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/history/txt_file.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/__init__.py
--rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/base.py
--rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py
--rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py
--rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py
--rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/index/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/__init__.py
--rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/base.py
--rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/json_file.py
--rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/__init__.py
--rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/base.py
--rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/json_file.py
--rw-r--r--   0        0        0    10462 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/model/patch.py
--rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/__init__.py
--rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/base.py
--rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
--rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
--rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
--rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/json_file.py
--rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/__init__.py
--rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/base.py
--rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/json_file.py
--rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/patch.py
--rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/__init__.py
--rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/base.py
--rwxr-xr-x   0        0        0     8307 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/json_file.py
--rw-r--r--   0        0        0     4651 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/patch.py
--rw-r--r--   0        0        0     7410 2024-05-02 17:43:40.452809 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/__init__.py
--rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/assistants.py
--rw-r--r--   0        0        0     7034 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/chat.py
--rw-r--r--   0        0        0     5876 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/completion.py
--rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/image.py
--rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/store.py
--rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/summarizer.py
--rw-r--r--   0        0        0     8266 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/vision.py
--rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/__init__.py
--rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/assistants.py
--rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/importer.py
--rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/__init__.py
--rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/anthropic.py
--rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.8/src/pygpt_net/provider/llms/azure_openai.py
--rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.8/src/pygpt_net/provider/llms/base.py
--rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/hugging_face.py
--rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/llama.py
--rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/llms/ollama.py
--rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.8/src/pygpt_net/provider/llms/openai.py
--rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/__init__.py
--rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/base.py
--rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_csv.py
--rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_docx.py
--rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_epub.py
--rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_excel.py
--rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_html.py
--rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_image_vision.py
--rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_ipynb.py
--rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_json.py
--rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_markdown.py
--rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_pdf.py
--rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_video_audio.py
--rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_xml.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/__init__.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
--rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
--rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/__init__.py
--rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/base.py
--rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/__init__.py
--rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/issues.py
--rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/repo.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/__init__.py
--rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/calendar.py
--rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/docs.py
--rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/gmail.py
--rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/keep.py
--rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/sheets.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
--rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/__init__.py
--rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
--rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
--rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
--rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
--rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
--rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
--rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/base.py
--rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/__init__.py
--rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/base.py
--rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/utils.py
--rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_bitbucket.py
--rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_database.py
--rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_issues.py
--rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_repo.py
--rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_calendar.py
--rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_docs.py
--rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_drive.py
--rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_gmail.py
--rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_keep.py
--rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_sheets.py
--rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
--rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_page.py
--rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_rss.py
--rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_sitemap.py
--rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_twitter.py
--rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_yt.py
--rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/__init__.py
--rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/base.py
--rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/chroma.py
--rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/elasticsearch.py
--rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/pinecode.py
--rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/redis.py
--rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/simple.py
--rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/temp.py
--rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.8/src/pygpt_net/provider/web/__init__.py
--rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.8/src/pygpt_net/provider/web/base.py
--rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/web/google_custom_search.py
--rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.8/src/pygpt_net/provider/web/microsoft_bing.py
--rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/__init__.py
--rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
--rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
--rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/base.py
--rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
--rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/widgets.py
--rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/__init__.py
--rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/dialogs.py
--rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/__init__.py
--rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/browse.py
--rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/ctx.py
--rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/dialogs.py
--rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/files.py
--rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/web.py
--rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/widgets.py
--rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/__init__.py
--rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/dialogs.py
--rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/widgets.py
--rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/__init__.py
--rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/dialogs.py
--rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/widgets.py
--rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.8/src/pygpt_net/ui/base/__init__.py
--rw-r--r--   0        0        0     9255 2024-05-02 17:09:01.777146 pygpt_net-2.2.8/src/pygpt_net/ui/base/config_dialog.py
--rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/base/context_menu.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/__init__.py
--rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/about.py
--rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/applog.py
--rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant.py
--rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant_store.py
--rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/changelog.py
--rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/create.py
--rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/db.py
--rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/debug.py
--rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/dictionary.py
--rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/editor.py
--rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/find.py
--rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/image.py
--rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/license.py
--rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/logger.py
--rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/models.py
--rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/plugins.py
--rwxr-xr-x   0        0        0     7391 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset.py
--rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset_plugins.py
--rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/profile.py
--rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/rename.py
--rwxr-xr-x   0        0        0    15114 2024-05-02 17:09:01.773146 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/settings.py
--rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/snap.py
--rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/start.py
--rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/update.py
--rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/dialog/workdir.py
--rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/dialogs.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/layout/__init__.py
--rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/__init__.py
--rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments.py
--rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
--rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/calendar.py
--rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/input.py
--rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/markdown.py
--rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/output.py
--rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/painter.py
--rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/__init__.py
--rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/ctx_list.py
--rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/search_input.py
--rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/video.py
--rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.8/src/pygpt_net/ui/layout/status.py
--rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/__init__.py
--rw-r--r--   0        0        0     2385 2024-05-02 17:09:01.701147 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/agent.py
--rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/assistants.py
--rwxr-xr-x   0        0        0     4555 2024-05-02 17:09:01.697147 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/footer.py
--rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/image.py
--rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/indexes.py
--rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/mode.py
--rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/model.py
--rwxr-xr-x   0        0        0     5109 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/presets.py
--rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/prompt.py
--rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/vision.py
--rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.8/src/pygpt_net/ui/main.py
--rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.8/src/pygpt_net/ui/menu/__init__.py
--rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.8/src/pygpt_net/ui/menu/about.py
--rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.8/src/pygpt_net/ui/menu/audio.py
--rw-r--r--   0        0        0     8291 2024-05-02 17:09:01.769146 pygpt_net-2.2.8/src/pygpt_net/ui/menu/config.py
--rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/menu/debug.py
--rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.8/src/pygpt_net/ui/menu/file.py
--rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/menu/lang.py
--rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/menu/plugins.py
--rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.8/src/pygpt_net/ui/menu/theme.py
--rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/menu/tools.py
--rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.8/src/pygpt_net/ui/menu/video.py
--rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/tray.py
--rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.8/src/pygpt_net/ui/widget/__init__.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/__init__.py
--rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input.py
--rw-r--r--   0        0        0     3771 2024-05-02 17:09:01.685147 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input_button.py
--rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/output.py
--rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/__init__.py
--rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/select.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/__init__.py
--rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/alert.py
--rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/applog.py
--rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/assistant_store.py
--rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/audio.py
--rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/base.py
--rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/confirm.py
--rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/create.py
--rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/db.py
--rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/debug.py
--rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor.py
--rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor_file.py
--rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/find.py
--rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/image.py
--rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/info.py
--rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/license.py
--rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/logger.py
--rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/model.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/preset_plugins.py
--rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/profile.py
--rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/rename.py
--rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings.py
--rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py
--rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/snap.py
--rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/update.py
--rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/workdir.py
--rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/__init__.py
--rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/painter.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/button.py
--rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/checkbox.py
--rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/group.py
--rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/labels.py
--rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/__init__.py
--rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/explorer.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/__init__.py
--rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/display.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/__init__.py
--rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant.py
--rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant_store.py
--rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/attachment.py
--rwxr-xr-x   0        0        0     2435 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/base.py
--rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/context.py
--rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/db.py
--rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/debug.py
--rw-r--r--   0        0        0     5739 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/experts.py
--rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index.py
--rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index_combo.py
--rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/mode.py
--rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model.py
--rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model_editor.py
--rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/plugin.py
--rwxr-xr-x   0        0        0     5655 2024-05-01 18:08:40.482948 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset.py
--rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset_plugins.py
--rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/profile.py
--rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/settings.py
--rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/uploaded.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/__init__.py
--rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/checkbox.py
--rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/cmd.py
--rw-r--r--   0        0        0     3594 2024-05-02 17:09:01.737146 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/combo.py
--rwxr-xr-x   0        0        0    13004 2024-05-02 17:09:01.649148 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/dictionary.py
--rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/input.py
--rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/prompt.py
--rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/slider.py
--rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/textarea.py
--rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/Input.py
--rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/__init__.py
--rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/output.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/calendar_note.py
--rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/create.py
--rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/editor.py
--rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/find.py
--rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/input.py
--rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/name.py
--rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/notepad.py
--rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/output.py
--rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/rename.py
--rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/search_input.py
--rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/web.py
--rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/__init__.py
--rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/camera.py
--rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.8/src/pygpt_net/utils.py
--rw-r--r--   0        0        0   143600 1970-01-01 00:00:00.000000 pygpt_net-2.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0    59733 2024-05-02 21:39:59.609647 pygpt_net-2.2.9/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1077 2024-02-01 17:53:56.362106 pygpt_net-2.2.9/LICENSE
+-rwxr-xr-x   0        0        0   140238 2024-05-02 21:39:59.613648 pygpt_net-2.2.9/README.md
+-rwxr-xr-x   0        0        0    13970 2024-02-19 21:38:20.920806 pygpt_net-2.2.9/icon.png
+-rw-r--r--   0        0        0     2979 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/pyproject.toml
+-rwxr-xr-x   0        0        0    58699 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/CHANGELOG.txt
+-rwxr-xr-x   0        0        0     1146 2024-02-01 17:53:56.366106 pygpt_net-2.2.9/src/pygpt_net/LICENSE
+-rwxr-xr-x   0        0        0     1024 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/__init__.py
+-rwxr-xr-x   0        0        0    14447 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/app.py
+-rwxr-xr-x   0        0        0    15485 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/config.py
+-rwxr-xr-x   0        0        0     3839 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/container.py
+-rwxr-xr-x   0        0        0     5333 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/__init__.py
+-rwxr-xr-x   0        0        0     2209 2024-05-02 18:50:37.000000 pygpt_net-2.2.9/src/pygpt_net/controller/access/__init__.py
+-rwxr-xr-x   0        0        0    12534 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/access/control.py
+-rwxr-xr-x   0        0        0    11965 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/access/voice.py
+-rw-r--r--   0        0        0     3823 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/agent/__init__.py
+-rw-r--r--   0        0        0     1748 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/agent/common.py
+-rw-r--r--   0        0        0     1407 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/agent/experts.py
+-rw-r--r--   0        0        0     6904 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/agent/flow.py
+-rw-r--r--   0        0        0     9877 2024-04-29 15:13:32.571516 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/__init__.py
+-rw-r--r--   0        0        0    20310 2024-04-30 16:41:29.971889 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/batch.py
+-rw-r--r--   0        0        0    13203 2024-04-27 14:05:11.727541 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/editor.py
+-rw-r--r--   0        0        0    14434 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/files.py
+-rwxr-xr-x   0        0        0    15545 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/store.py
+-rw-r--r--   0        0        0    17631 2024-04-29 05:51:11.636212 pygpt_net-2.2.9/src/pygpt_net/controller/assistant/threads.py
+-rwxr-xr-x   0        0        0    15661 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/attachment.py
+-rw-r--r--   0        0        0     6560 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/audio/__init__.py
+-rw-r--r--   0        0        0     3922 2024-04-29 05:51:11.636212 pygpt_net-2.2.9/src/pygpt_net/controller/calendar/__init__.py
+-rw-r--r--   0        0        0     8937 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/calendar/note.py
+-rwxr-xr-x   0        0        0    13013 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/camera.py
+-rw-r--r--   0        0        0     1628 2024-04-29 05:51:11.636212 pygpt_net-2.2.9/src/pygpt_net/controller/chat/__init__.py
+-rwxr-xr-x   0        0        0    11749 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/chat/common.py
+-rw-r--r--   0        0        0     2156 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/controller/chat/files.py
+-rwxr-xr-x   0        0        0     6533 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/chat/image.py
+-rwxr-xr-x   0        0        0    10650 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/chat/input.py
+-rwxr-xr-x   0        0        0    11366 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/chat/output.py
+-rwxr-xr-x   0        0        0     9610 2024-04-25 00:06:58.371551 pygpt_net-2.2.9/src/pygpt_net/controller/chat/render.py
+-rw-r--r--   0        0        0    13022 2024-05-02 18:50:37.170695 pygpt_net-2.2.9/src/pygpt_net/controller/chat/text.py
+-rw-r--r--   0        0        0     3382 2024-04-11 20:50:24.189030 pygpt_net-2.2.9/src/pygpt_net/controller/chat/vision.py
+-rw-r--r--   0        0        0     5292 2024-03-26 17:12:51.286309 pygpt_net-2.2.9/src/pygpt_net/controller/command.py
+-rw-r--r--   0        0        0     4485 2024-04-26 21:55:50.675598 pygpt_net-2.2.9/src/pygpt_net/controller/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/__init__.py
+-rwxr-xr-x   0        0        0     2422 2024-01-30 20:56:32.772879 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/checkbox.py
+-rw-r--r--   0        0        0     4863 2024-03-12 06:49:17.164785 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/cmd.py
+-rw-r--r--   0        0        0     3237 2024-05-02 10:44:22.869251 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/combo.py
+-rw-r--r--   0        0        0     6657 2024-05-02 14:53:21.198368 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/dictionary.py
+-rw-r--r--   0        0        0     3556 2024-03-15 15:31:21.786121 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/input.py
+-rw-r--r--   0        0        0     4580 2024-04-21 01:33:54.239765 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/slider.py
+-rw-r--r--   0        0        0     2337 2024-04-22 21:31:19.988317 pygpt_net-2.2.9/src/pygpt_net/controller/config/field/textarea.py
+-rw-r--r--   0        0        0     8222 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/config/placeholder.py
+-rw-r--r--   0        0        0    30454 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/ctx/__init__.py
+-rw-r--r--   0        0        0     5434 2024-04-10 01:07:30.184635 pygpt_net-2.2.9/src/pygpt_net/controller/ctx/common.py
+-rwxr-xr-x   0        0        0     7529 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/ctx/extra.py
+-rw-r--r--   0        0        0     2552 2024-01-25 22:43:11.543975 pygpt_net-2.2.9/src/pygpt_net/controller/ctx/summarizer.py
+-rw-r--r--   0        0        0     7732 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/debug/__init__.py
+-rw-r--r--   0        0        0     1008 2023-12-31 03:09:04.107766 pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/__init__.py
+-rwxr-xr-x   0        0        0    13546 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/confirm.py
+-rw-r--r--   0        0        0     5634 2024-03-07 01:04:26.437955 pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/debug.py
+-rwxr-xr-x   0        0        0     2582 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/info.py
+-rwxr-xr-x   0        0        0    15699 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/controller/files.py
+-rwxr-xr-x   0        0        0     4874 2024-04-21 01:33:54.239765 pygpt_net-2.2.9/src/pygpt_net/controller/finder.py
+-rwxr-xr-x   0        0        0     7090 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/idx/__init__.py
+-rw-r--r--   0        0        0     2605 2024-02-29 03:07:51.274132 pygpt_net-2.2.9/src/pygpt_net/controller/idx/common.py
+-rwxr-xr-x   0        0        0    21150 2024-04-17 04:14:11.980074 pygpt_net-2.2.9/src/pygpt_net/controller/idx/indexer.py
+-rw-r--r--   0        0        0     7789 2024-03-03 03:52:54.350656 pygpt_net-2.2.9/src/pygpt_net/controller/idx/settings.py
+-rw-r--r--   0        0        0     3289 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/lang/__init__.py
+-rw-r--r--   0        0        0     5080 2024-04-27 14:05:11.727541 pygpt_net-2.2.9/src/pygpt_net/controller/lang/custom.py
+-rw-r--r--   0        0        0    20280 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/lang/mapping.py
+-rw-r--r--   0        0        0     3879 2024-01-15 13:47:55.919633 pygpt_net-2.2.9/src/pygpt_net/controller/lang/plugins.py
+-rw-r--r--   0        0        0     2634 2024-01-22 12:10:21.917245 pygpt_net-2.2.9/src/pygpt_net/controller/lang/settings.py
+-rwxr-xr-x   0        0        0     1566 2024-01-04 07:51:17.999390 pygpt_net-2.2.9/src/pygpt_net/controller/launcher.py
+-rwxr-xr-x   0        0        0    11297 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/layout.py
+-rw-r--r--   0        0        0     6521 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/mode.py
+-rw-r--r--   0        0        0     4656 2024-01-30 20:56:32.772879 pygpt_net-2.2.9/src/pygpt_net/controller/model/__init__.py
+-rw-r--r--   0        0        0    12599 2024-02-22 03:36:30.096422 pygpt_net-2.2.9/src/pygpt_net/controller/model/editor.py
+-rwxr-xr-x   0        0        0    13351 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/notepad.py
+-rw-r--r--   0        0        0     2572 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/painter/__init__.py
+-rw-r--r--   0        0        0     4461 2024-01-23 23:46:30.495197 pygpt_net-2.2.9/src/pygpt_net/controller/painter/capture.py
+-rw-r--r--   0        0        0     6292 2024-02-17 21:22:47.341663 pygpt_net-2.2.9/src/pygpt_net/controller/painter/common.py
+-rw-r--r--   0        0        0    13977 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/plugins/__init__.py
+-rw-r--r--   0        0        0    11914 2024-03-07 01:04:26.441956 pygpt_net-2.2.9/src/pygpt_net/controller/plugins/presets.py
+-rw-r--r--   0        0        0     6040 2024-04-10 03:33:51.491189 pygpt_net-2.2.9/src/pygpt_net/controller/plugins/settings.py
+-rwxr-xr-x   0        0        0    17127 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/presets/__init__.py
+-rwxr-xr-x   0        0        0    16058 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/presets/editor.py
+-rw-r--r--   0        0        0     4937 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/presets/experts.py
+-rw-r--r--   0        0        0     7684 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/settings/__init__.py
+-rwxr-xr-x   0        0        0    15241 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/settings/editor.py
+-rw-r--r--   0        0        0    20965 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/controller/settings/profile.py
+-rwxr-xr-x   0        0        0     8597 2024-04-14 16:40:07.849541 pygpt_net-2.2.9/src/pygpt_net/controller/settings/workdir.py
+-rwxr-xr-x   0        0        0     6308 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/theme/__init__.py
+-rwxr-xr-x   0        0        0     5437 2024-04-30 16:41:29.975888 pygpt_net-2.2.9/src/pygpt_net/controller/theme/common.py
+-rw-r--r--   0        0        0     5085 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/controller/theme/markdown.py
+-rw-r--r--   0        0        0     4631 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/controller/theme/menu.py
+-rw-r--r--   0        0        0     5028 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/controller/theme/nodes.py
+-rw-r--r--   0        0        0     6934 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/controller/ui/__init__.py
+-rw-r--r--   0        0        0     6663 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/controller/ui/mode.py
+-rw-r--r--   0        0        0     2378 2024-04-30 16:41:29.975888 pygpt_net-2.2.9/src/pygpt_net/controller/ui/vision.py
+-rw-r--r--   0        0        0        0 2024-01-26 16:05:36.561120 pygpt_net-2.2.9/src/pygpt_net/core/__init__.py
+-rwxr-xr-x   0        0        0      874 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/core/access/__init__.py
+-rwxr-xr-x   0        0        0     2351 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/core/access/actions.py
+-rwxr-xr-x   0        0        0     3194 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/core/access/events.py
+-rw-r--r--   0        0        0     3397 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/access/shortcuts.py
+-rwxr-xr-x   0        0        0    11152 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/core/access/voice.py
+-rw-r--r--   0        0        0     1382 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/agents/__init__.py
+-rw-r--r--   0        0        0     4330 2024-04-26 21:55:50.675598 pygpt_net-2.2.9/src/pygpt_net/core/assistants/__init__.py
+-rw-r--r--   0        0        0     9796 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/core/assistants/files.py
+-rw-r--r--   0        0        0     7990 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/core/assistants/store.py
+-rwxr-xr-x   0        0        0    10240 2024-01-31 15:19:17.738030 pygpt_net-2.2.9/src/pygpt_net/core/attachments.py
+-rw-r--r--   0        0        0     2708 2024-02-24 01:55:58.445111 pygpt_net-2.2.9/src/pygpt_net/core/audio.py
+-rw-r--r--   0        0        0     7483 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/bridge.py
+-rw-r--r--   0        0        0     6634 2024-03-12 06:49:17.164785 pygpt_net-2.2.9/src/pygpt_net/core/calendar/__init__.py
+-rwxr-xr-x   0        0        0     4034 2024-02-21 16:18:39.952987 pygpt_net-2.2.9/src/pygpt_net/core/camera.py
+-rw-r--r--   0        0        0     3330 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/core/chain/__init__.py
+-rw-r--r--   0        0        0     4988 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/core/chain/chat.py
+-rw-r--r--   0        0        0     5413 2024-05-01 18:08:40.474948 pygpt_net-2.2.9/src/pygpt_net/core/chain/completion.py
+-rwxr-xr-x   0        0        0    10538 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/command.py
+-rwxr-xr-x   0        0        0    35857 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/core/ctx/__init__.py
+-rw-r--r--   0        0        0     7709 2024-02-27 05:21:39.767084 pygpt_net-2.2.9/src/pygpt_net/core/ctx/idx.py
+-rw-r--r--   0        0        0    15975 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/db/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-17 01:35:30.422055 pygpt_net-2.2.9/src/pygpt_net/core/db/viewer.py
+-rwxr-xr-x   0        0        0     9240 2024-03-26 17:12:51.290309 pygpt_net-2.2.9/src/pygpt_net/core/debug/__init__.py
+-rw-r--r--   0        0        0     1467 2024-02-25 18:06:16.205368 pygpt_net-2.2.9/src/pygpt_net/core/debug/agent.py
+-rwxr-xr-x   0        0        0     2532 2024-04-26 21:55:50.675598 pygpt_net-2.2.9/src/pygpt_net/core/debug/assistants.py
+-rwxr-xr-x   0        0        0     1626 2024-02-25 22:01:41.690831 pygpt_net-2.2.9/src/pygpt_net/core/debug/attachments.py
+-rwxr-xr-x   0        0        0     2305 2024-04-10 01:07:30.184635 pygpt_net-2.2.9/src/pygpt_net/core/debug/config.py
+-rwxr-xr-x   0        0        0     3543 2024-04-14 04:42:08.288289 pygpt_net-2.2.9/src/pygpt_net/core/debug/context.py
+-rw-r--r--   0        0        0      776 2024-03-07 01:04:26.441956 pygpt_net-2.2.9/src/pygpt_net/core/debug/db.py
+-rw-r--r--   0        0        0     5194 2024-03-12 06:49:17.164785 pygpt_net-2.2.9/src/pygpt_net/core/debug/indexes.py
+-rwxr-xr-x   0        0        0     1848 2024-02-25 22:01:41.690831 pygpt_net-2.2.9/src/pygpt_net/core/debug/models.py
+-rwxr-xr-x   0        0        0     1258 2024-02-25 22:01:41.690831 pygpt_net-2.2.9/src/pygpt_net/core/debug/plugins.py
+-rwxr-xr-x   0        0        0     1994 2024-02-25 22:01:41.690831 pygpt_net-2.2.9/src/pygpt_net/core/debug/presets.py
+-rwxr-xr-x   0        0        0     2666 2024-02-25 22:01:41.690831 pygpt_net-2.2.9/src/pygpt_net/core/debug/ui.py
+-rwxr-xr-x   0        0        0    10010 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/dispatcher.py
+-rw-r--r--   0        0        0    10014 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/core/experts/__init__.py
+-rwxr-xr-x   0        0        0    15252 2024-04-29 10:51:04.365787 pygpt_net-2.2.9/src/pygpt_net/core/filesystem/__init__.py
+-rw-r--r--   0        0        0     4074 2024-03-26 17:12:51.290309 pygpt_net-2.2.9/src/pygpt_net/core/filesystem/actions.py
+-rw-r--r--   0        0        0     4123 2024-04-22 03:13:23.727782 pygpt_net-2.2.9/src/pygpt_net/core/filesystem/editor.py
+-rw-r--r--   0        0        0     3385 2024-03-19 09:04:41.050928 pygpt_net-2.2.9/src/pygpt_net/core/filesystem/types.py
+-rw-r--r--   0        0        0     2753 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/filesystem/url.py
+-rwxr-xr-x   0        0        0     3092 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/core/history.py
+-rwxr-xr-x   0        0        0    17238 2024-04-17 01:35:30.422055 pygpt_net-2.2.9/src/pygpt_net/core/idx/__init__.py
+-rwxr-xr-x   0        0        0    13030 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/idx/chat.py
+-rw-r--r--   0        0        0     2443 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/idx/context.py
+-rwxr-xr-x   0        0        0    31850 2024-04-17 01:35:30.422055 pygpt_net-2.2.9/src/pygpt_net/core/idx/indexing.py
+-rw-r--r--   0        0        0     4016 2024-04-26 23:49:43.379197 pygpt_net-2.2.9/src/pygpt_net/core/idx/llm.py
+-rw-r--r--   0        0        0     5304 2024-04-17 01:35:30.422055 pygpt_net-2.2.9/src/pygpt_net/core/idx/metadata.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.767084 pygpt_net-2.2.9/src/pygpt_net/core/idx/types/__init__.py
+-rw-r--r--   0        0        0     3113 2024-02-27 05:21:39.767084 pygpt_net-2.2.9/src/pygpt_net/core/idx/types/ctx.py
+-rw-r--r--   0        0        0     4722 2024-02-27 05:21:39.767084 pygpt_net-2.2.9/src/pygpt_net/core/idx/types/external.py
+-rw-r--r--   0        0        0     3733 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/core/idx/types/files.py
+-rwxr-xr-x   0        0        0     3774 2024-04-17 04:14:11.980074 pygpt_net-2.2.9/src/pygpt_net/core/idx/worker.py
+-rwxr-xr-x   0        0        0     3288 2024-03-17 13:18:45.634349 pygpt_net-2.2.9/src/pygpt_net/core/image.py
+-rwxr-xr-x   0        0        0      829 2023-12-31 03:18:56.426282 pygpt_net-2.2.9/src/pygpt_net/core/info.py
+-rw-r--r--   0        0        0     2040 2024-03-25 10:26:39.426403 pygpt_net-2.2.9/src/pygpt_net/core/installer.py
+-rw-r--r--   0        0        0     1168 2024-01-14 15:51:20.622630 pygpt_net-2.2.9/src/pygpt_net/core/llm/__init__.py
+-rwxr-xr-x   0        0        0     5112 2024-04-11 16:41:32.664297 pygpt_net-2.2.9/src/pygpt_net/core/locale.py
+-rw-r--r--   0        0        0     7573 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/core/models.py
+-rw-r--r--   0        0        0     1913 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/core/modes.py
+-rwxr-xr-x   0        0        0     3378 2024-04-10 01:07:30.184635 pygpt_net-2.2.9/src/pygpt_net/core/notepad.py
+-rwxr-xr-x   0        0        0     4395 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/core/platforms.py
+-rwxr-xr-x   0        0        0    14828 2024-04-28 08:05:35.578680 pygpt_net-2.2.9/src/pygpt_net/core/plugins.py
+-rw-r--r--   0        0        0    12366 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/presets.py
+-rw-r--r--   0        0        0     7650 2024-04-10 01:07:30.184635 pygpt_net-2.2.9/src/pygpt_net/core/profile.py
+-rw-r--r--   0        0        0     4529 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/prompt/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-22 22:35:26.800429 pygpt_net-2.2.9/src/pygpt_net/core/prompt/template.py
+-rw-r--r--   0        0        0      489 2024-01-05 12:12:41.797675 pygpt_net-2.2.9/src/pygpt_net/core/render/__init__.py
+-rw-r--r--   0        0        0     5024 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/core/render/base.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/render/markdown/__init__.py
+-rwxr-xr-x   0        0        0     5450 2024-04-22 05:35:04.663179 pygpt_net-2.2.9/src/pygpt_net/core/render/markdown/parser.py
+-rwxr-xr-x   0        0        0    23291 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/core/render/markdown/renderer.py
+-rw-r--r--   0        0        0      489 2024-01-05 13:07:04.262555 pygpt_net-2.2.9/src/pygpt_net/core/render/plain/__init__.py
+-rw-r--r--   0        0        0    15716 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/render/plain/renderer.py
+-rwxr-xr-x   0        0        0      489 2024-04-21 01:33:54.000000 pygpt_net-2.2.9/src/pygpt_net/core/render/web/__init__.py
+-rwxr-xr-x   0        0        0     8564 2024-04-28 06:16:26.324027 pygpt_net-2.2.9/src/pygpt_net/core/render/web/parser.py
+-rwxr-xr-x   0        0        0    43236 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/render/web/renderer.py
+-rwxr-xr-x   0        0        0     7512 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/text/__init__.py
+-rwxr-xr-x   0        0        0     6566 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/text/finder.py
+-rw-r--r--   0        0        0     2250 2024-04-29 05:51:11.640212 pygpt_net-2.2.9/src/pygpt_net/core/text/utils.py
+-rw-r--r--   0        0        0     6487 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/core/text/web_finder.py
+-rwxr-xr-x   0        0        0    14472 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/core/tokens.py
+-rw-r--r--   0        0        0    13722 2024-02-21 19:09:37.240983 pygpt_net-2.2.9/src/pygpt_net/core/updater/__init__.py
+-rw-r--r--   0        0        0     2343 2024-02-24 01:55:58.445111 pygpt_net-2.2.9/src/pygpt_net/core/web.py
+-rw-r--r--   0        0        0      901 2024-01-25 22:43:11.543975 pygpt_net-2.2.9/src/pygpt_net/core/worker.py
+-rw-r--r--   0        0        0    65201 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/audio/click_off.mp3
+-rw-r--r--   0        0        0    65201 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/audio/click_on.mp3
+-rw-r--r--   0        0        0    32256 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/audio/ok.mp3
+-rwxr-xr-x   0        0        0    15381 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/data/config/config.json
+-rwxr-xr-x   0        0        0    20573 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/data/config/models.json
+-rw-r--r--   0        0        0     1595 2024-05-02 21:39:59.617648 pygpt_net-2.2.9/src/pygpt_net/data/config/modes.json
+-rwxr-xr-x   0        0        0      528 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/batman_and_joker.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.agent.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.assistant.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.chat.json
+-rwxr-xr-x   0        0        0      436 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.completion.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.expert.json
+-rwxr-xr-x   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.img.json
+-rwxr-xr-x   0        0        0      433 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.langchain.json
+-rw-r--r--   0        0        0      419 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.llama_index.json
+-rwxr-xr-x   0        0        0      447 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/current.vision.json
+-rwxr-xr-x   0        0        0      552 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/dalle_white_cat.json
+-rw-r--r--   0        0        0      474 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/joke_agent.json
+-rw-r--r--   0        0        0      683 2024-05-01 18:08:40.478948 pygpt_net-2.2.9/src/pygpt_net/data/config/presets/joke_expert.json
+-rwxr-xr-x   0        0        0    36092 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/config/settings.json
+-rw-r--r--   0        0        0      870 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/config/settings_section.json
+-rwxr-xr-x   0        0        0      664 2024-03-18 04:54:07.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/fix_windows.css
+-rwxr-xr-x   0        0        0     1122 2024-04-19 00:29:50.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.css
+-rwxr-xr-x   0        0        0      730 2024-04-19 00:29:50.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.dark.css
+-rwxr-xr-x   0        0        0      833 2024-04-19 00:29:50.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.light.css
+-rwxr-xr-x   0        0        0      400 2024-04-20 05:54:38.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/style.css
+-rwxr-xr-x   0        0        0      729 2024-04-21 01:33:54.243764 pygpt_net-2.2.9/src/pygpt_net/data/css/style.dark.css
+-rwxr-xr-x   0        0        0     1726 2024-04-20 05:55:02.000000 pygpt_net-2.2.9/src/pygpt_net/data/css/style.light.css
+-rwxr-xr-x   0        0        0     3407 2024-04-24 23:37:32.612565 pygpt_net-2.2.9/src/pygpt_net/data/css/web.css
+-rwxr-xr-x   0        0        0     1260 2024-04-25 03:37:50.192528 pygpt_net-2.2.9/src/pygpt_net/data/css/web.dark.css
+-rwxr-xr-x   0        0        0     1235 2024-04-25 03:07:07.934949 pygpt_net-2.2.9/src/pygpt_net/data/css/web.light.css
+-rwxr-xr-x   0        0        0    69484 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf
+-rwxr-xr-x   0        0        0    71948 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf
+-rwxr-xr-x   0        0        0    73316 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf
+-rwxr-xr-x   0        0        0    77680 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf
+-rwxr-xr-x   0        0        0    75744 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf
+-rwxr-xr-x   0        0        0    77192 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf
+-rwxr-xr-x   0        0        0    49064 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf
+-rwxr-xr-x   0        0        0    75136 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf
+-rwxr-xr-x   0        0        0    69968 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf
+-rwxr-xr-x   0        0        0    48848 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf
+-rwxr-xr-x   0        0        0     4500 2023-12-08 15:03:16.000000 pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/OFL.txt
+-rw-r--r--   0        0        0    77432 2024-04-08 04:19:15.417912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf
+-rw-r--r--   0        0        0    82112 2024-04-08 04:19:15.417912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf
+-rw-r--r--   0        0        0    81240 2024-04-08 04:19:15.417912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf
+-rw-r--r--   0        0        0    75476 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf
+-rw-r--r--   0        0        0    75000 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf
+-rw-r--r--   0        0        0    77804 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf
+-rw-r--r--   0        0        0    76752 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf
+-rw-r--r--   0        0        0    74248 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf
+-rw-r--r--   0        0        0    74120 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf
+-rw-r--r--   0        0        0    79236 2024-04-08 04:19:15.421912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf
+-rw-r--r--   0        0        0    78488 2024-04-08 04:19:15.425912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf
+-rw-r--r--   0        0        0    73232 2024-04-08 04:19:15.425912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf
+-rw-r--r--   0        0        0    88992 2024-04-08 04:19:15.425912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf
+-rw-r--r--   0        0        0    94348 2024-04-08 04:19:15.425912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf
+-rw-r--r--   0        0        0    93720 2024-04-08 04:19:15.425912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf
+-rw-r--r--   0        0        0    88668 2024-04-08 04:19:15.429912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf
+-rw-r--r--   0        0        0    79280 2024-04-08 04:19:15.429912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf
+-rw-r--r--   0        0        0    85648 2024-04-08 04:19:15.429912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf
+-rw-r--r--   0        0        0    85824 2024-04-08 04:19:15.429912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf
+-rw-r--r--   0        0        0    80200 2024-04-08 04:19:15.429912 pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf
+-rwxr-xr-x   0        0        0     4352 2024-03-18 04:54:07.633826 pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/OFL.txt
+-rwxr-xr-x   0        0        0    86636 2024-03-18 04:54:07.633826 pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rwxr-xr-x   0        0        0    95292 2024-03-18 04:54:07.633826 pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rwxr-xr-x   0        0        0   103524 2024-03-18 04:54:07.633826 pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rwxr-xr-x   0        0        0    90904 2024-03-18 04:54:07.637826 pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rwxr-xr-x   0        0        0     3461 2023-04-14 00:10:28.000000 pygpt_net-2.2.9/src/pygpt_net/data/icon.ico
+-rwxr-xr-x   0        0        0    13970 2023-04-14 00:10:28.000000 pygpt_net-2.2.9/src/pygpt_net/data/icon.png
+-rw-r--r--   0        0        0     5471 2024-01-29 18:11:38.035830 pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_busy.ico
+-rw-r--r--   0        0        0    14837 2024-01-29 18:11:38.035830 pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_error.ico
+-rw-r--r--   0        0        0     4209 2024-01-29 18:11:38.035830 pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_idle.ico
+-rw-r--r--   0        0        0      538 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/abc.svg
+-rw-r--r--   0        0        0      360 2024-05-02 18:50:37.174695 pygpt_net-2.2.9/src/pygpt_net/data/icons/accessibility.svg
+-rw-r--r--   0        0        0      178 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/add.svg
+-rw-r--r--   0        0        0      463 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/add_circle.svg
+-rw-r--r--   0        0        0      348 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/add_folder.svg
+-rw-r--r--   0        0        0      391 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/add_library.svg
+-rw-r--r--   0        0        0      558 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/alarm.svg
+-rw-r--r--   0        0        0     1027 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/apps.svg
+-rw-r--r--   0        0        0      267 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/asterisk.svg
+-rw-r--r--   0        0        0      429 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/attachment.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/attachments.svg
+-rw-r--r--   0        0        0      185 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/back.svg
+-rw-r--r--   0        0        0      395 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/backspace.svg
+-rw-r--r--   0        0        0      472 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/block.svg
+-rw-r--r--   0        0        0      255 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/bookmark.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/brush.svg
+-rw-r--r--   0        0        0      523 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/build.svg
+-rw-r--r--   0        0        0      927 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/calendar.svg
+-rw-r--r--   0        0        0      496 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/camera.svg
+-rw-r--r--   0        0        0      987 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/audio.png
+-rw-r--r--   0        0        0      798 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/copy.png
+-rw-r--r--   0        0        0      737 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/delete.png
+-rw-r--r--   0        0        0      837 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/edit.png
+-rw-r--r--   0        0        0      715 2024-03-10 08:19:22.357281 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/join.png
+-rw-r--r--   0        0        0      956 2024-03-09 21:41:28.185853 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/reload.png
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/chat.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/check.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/check_circle.svg
+-rw-r--r--   0        0        0      265 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/checklist.svg
+-rw-r--r--   0        0        0      406 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/circle.svg
+-rw-r--r--   0        0        0      191 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/clear.svg
+-rw-r--r--   0        0        0      411 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/clock.svg
+-rw-r--r--   0        0        0      218 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/close.svg
+-rw-r--r--   0        0        0      503 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/close_circle.svg
+-rw-r--r--   0        0        0      224 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/code.svg
+-rw-r--r--   0        0        0      298 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/computer.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/copy.svg
+-rw-r--r--   0        0        0      264 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/crop.svg
+-rw-r--r--   0        0        0      666 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/cut.svg
+-rw-r--r--   0        0        0      725 2024-01-30 17:23:19.885579 pygpt_net-2.2.9/src/pygpt_net/data/icons/db.svg
+-rw-r--r--   0        0        0      271 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/delete.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/done.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/download.svg
+-rw-r--r--   0        0        0      283 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/draft.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/drag.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/edit.svg
+-rw-r--r--   0        0        0      497 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/emergency.svg
+-rw-r--r--   0        0        0      195 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/equalizer.svg
+-rw-r--r--   0        0        0      533 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/error.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/event_available.svg
+-rw-r--r--   0        0        0      174 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/expand.svg
+-rw-r--r--   0        0        0      247 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/fast_forward.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/fast_rewind.svg
+-rw-r--r--   0        0        0      504 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/favorite.svg
+-rw-r--r--   0        0        0      297 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/folder.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/folder_filled.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/forward.svg
+-rw-r--r--   0        0        0      194 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/full.svg
+-rw-r--r--   0        0        0      249 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/fullscreen.svg
+-rw-r--r--   0        0        0      459 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/grid.svg
+-rw-r--r--   0        0        0      602 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/hearing.svg
+-rw-r--r--   0        0        0      691 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/help.svg
+-rw-r--r--   0        0        0      440 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/history.svg
+-rw-r--r--   0        0        0      239 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/home.svg
+-rw-r--r--   0        0        0      176 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/home_filled.svg
+-rw-r--r--   0        0        0      323 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/image.svg
+-rw-r--r--   0        0        0      531 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/info.svg
+-rw-r--r--   0        0        0      337 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/input.svg
+-rw-r--r--   0        0        0      541 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/key.svg
+-rw-r--r--   0        0        0      517 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/keyboard.svg
+-rw-r--r--   0        0        0      972 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/language.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/list.svg
+-rw-r--r--   0        0        0      495 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/lock.svg
+-rw-r--r--   0        0        0      273 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/logout.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/map.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/memory.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/menu.svg
+-rw-r--r--   0        0        0      447 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/mic.svg
+-rw-r--r--   0        0        0      485 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/mic_off.svg
+-rw-r--r--   0        0        0      423 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/more_horizontal.svg
+-rw-r--r--   0        0        0      491 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/mute.svg
+-rw-r--r--   0        0        0      296 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/open_tab.svg
+-rw-r--r--   0        0        0      846 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/palette.svg
+-rw-r--r--   0        0        0      431 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/paste.svg
+-rw-r--r--   0        0        0      250 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/pause.svg
+-rw-r--r--   0        0        0      454 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/pause_circle.svg
+-rw-r--r--   0        0        0      377 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/photos.svg
+-rw-r--r--   0        0        0      441 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/pin.svg
+-rw-r--r--   0        0        0      186 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/play.svg
+-rw-r--r--   0        0        0      197 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/play_pause.svg
+-rw-r--r--   0        0        0      246 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/playlist_add.svg
+-rw-r--r--   0        0        0      318 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/power.svg
+-rw-r--r--   0        0        0      478 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/print.svg
+-rw-r--r--   0        0        0      598 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/public_filled.svg
+-rw-r--r--   0        0        0      283 2024-01-30 20:56:32.772879 pygpt_net-2.2.9/src/pygpt_net/data/icons/redo.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/reload.svg
+-rw-r--r--   0        0        0      260 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/repeat.svg
+-rw-r--r--   0        0        0      400 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/replay.svg
+-rw-r--r--   0        0        0      401 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/resize.svg
+-rw-r--r--   0        0        0      615 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/robot.svg
+-rw-r--r--   0        0        0      807 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/router.svg
+-rw-r--r--   0        0        0      384 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/save.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/schedule.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/screenshot.svg
+-rw-r--r--   0        0        0      372 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/search.svg
+-rw-r--r--   0        0        0      274 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/security.svg
+-rw-r--r--   0        0        0      660 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/sensors.svg
+-rw-r--r--   0        0        0      767 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/settings.svg
+-rw-r--r--   0        0        0      475 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/settings_filled.svg
+-rw-r--r--   0        0        0      792 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/share.svg
+-rw-r--r--   0        0        0      469 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/shedule.svg
+-rw-r--r--   0        0        0      189 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/sort.svg
+-rw-r--r--   0        0        0      386 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/stack.svg
+-rw-r--r--   0        0        0      306 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/stacks.svg
+-rw-r--r--   0        0        0      291 2024-01-30 17:23:19.889579 pygpt_net-2.2.9/src/pygpt_net/data/icons/star.svg
+-rw-r--r--   0        0        0      188 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/stop.svg
+-rw-r--r--   0        0        0      432 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/stop_circle.svg
+-rw-r--r--   0        0        0      381 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/sync.svg
+-rw-r--r--   0        0        0      317 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/tag.svg
+-rw-r--r--   0        0        0      334 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/task.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/terminal.svg
+-rw-r--r--   0        0        0      204 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/text.svg
+-rw-r--r--   0        0        0      329 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/textfile.svg
+-rw-r--r--   0        0        0      479 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/timer.svg
+-rw-r--r--   0        0        0      321 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/today.svg
+-rw-r--r--   0        0        0      308 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/tune.svg
+-rw-r--r--   0        0        0      282 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/undo.svg
+-rw-r--r--   0        0        0      444 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/update.svg
+-rw-r--r--   0        0        0      392 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/updater.svg
+-rw-r--r--   0        0        0      276 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/upload.svg
+-rw-r--r--   0        0        0      339 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/video.svg
+-rw-r--r--   0        0        0      550 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/view.svg
+-rw-r--r--   0        0        0      736 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/voice.svg
+-rw-r--r--   0        0        0      374 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/volume.svg
+-rw-r--r--   0        0        0      310 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/warning.svg
+-rw-r--r--   0        0        0      300 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/webcam.svg
+-rw-r--r--   0        0        0      375 2024-02-29 03:07:51.274132 pygpt_net-2.2.9/src/pygpt_net/data/icons/webcam_off.svg
+-rw-r--r--   0        0        0      325 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/width.svg
+-rw-r--r--   0        0        0      336 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/window.svg
+-rw-r--r--   0        0        0      365 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/work.svg
+-rw-r--r--   0        0        0      422 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/zoom_in.svg
+-rw-r--r--   0        0        0      396 2024-01-30 17:23:19.893578 pygpt_net-2.2.9/src/pygpt_net/data/icons/zoom_out.svg
+-rwxr-xr-x   0        0        0    52975 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.de.ini
+-rwxr-xr-x   0        0        0    60570 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.en.ini
+-rwxr-xr-x   0        0        0    53162 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.es.ini
+-rwxr-xr-x   0        0        0    54970 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.fr.ini
+-rwxr-xr-x   0        0        0    52142 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.it.ini
+-rwxr-xr-x   0        0        0    52299 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.pl.ini
+-rwxr-xr-x   0        0        0    72903 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.uk.ini
+-rwxr-xr-x   0        0        0    55293 2024-05-02 21:39:59.621649 pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.zh.ini
+-rwxr-xr-x   0        0        0     1477 2024-03-12 06:49:17.164785 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.agent.en.ini
+-rwxr-xr-x   0        0        0     1394 2024-03-12 06:49:17.164785 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.agent.pl.ini
+-rwxr-xr-x   0        0        0     5371 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_input.en.ini
+-rwxr-xr-x   0        0        0     5129 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_input.pl.ini
+-rwxr-xr-x   0        0        0     1721 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_output.en.ini
+-rwxr-xr-x   0        0        0     1395 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_output.pl.ini
+-rw-r--r--   0        0        0      622 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_api.en.ini
+-rw-r--r--   0        0        0      853 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini
+-rwxr-xr-x   0        0        0     2365 2024-03-19 03:42:00.618910 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini
+-rwxr-xr-x   0        0        0     1614 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini
+-rwxr-xr-x   0        0        0      455 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_custom.en.ini
+-rwxr-xr-x   0        0        0      528 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini
+-rwxr-xr-x   0        0        0     4234 2024-03-13 17:35:47.179523 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_files.en.ini
+-rwxr-xr-x   0        0        0     3584 2024-03-13 17:35:47.179523 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini
+-rw-r--r--   0        0        0     2280 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_history.en.ini
+-rw-r--r--   0        0        0     2765 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini
+-rw-r--r--   0        0        0     1042 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini
+-rw-r--r--   0        0        0     1511 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini
+-rwxr-xr-x   0        0        0     4840 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_web.en.ini
+-rwxr-xr-x   0        0        0     4660 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini
+-rw-r--r--   0        0        0      758 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.crontab.en.ini
+-rw-r--r--   0        0        0      871 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.crontab.pl.ini
+-rw-r--r--   0        0        0       99 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.experts.en.ini
+-rw-r--r--   0        0        0      338 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.extra_prompt.en.ini
+-rw-r--r--   0        0        0      474 2024-03-12 03:34:38.663323 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.extra_prompt.pl.ini
+-rwxr-xr-x   0        0        0     1970 2024-03-13 17:35:47.179523 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini
+-rwxr-xr-x   0        0        0     1180 2024-03-13 17:35:47.179523 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini
+-rw-r--r--   0        0        0      396 2024-03-17 13:18:45.662349 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_dalle.en.ini
+-rw-r--r--   0        0        0      427 2024-03-17 13:18:45.662349 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_dalle.pl.ini
+-rw-r--r--   0        0        0     1393 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_vision.en.ini
+-rw-r--r--   0        0        0     1426 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini
+-rwxr-xr-x   0        0        0      631 2024-01-30 20:56:32.776879 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.real_time.en.ini
+-rwxr-xr-x   0        0        0      752 2024-01-30 20:56:32.776879 pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.real_time.pl.ini
+-rwxr-xr-x   0        0        0    19418 2023-12-14 19:08:45.000000 pygpt_net-2.2.9/src/pygpt_net/data/logo.png
+-rw-r--r--   0        0        0    83051 2024-04-22 22:35:26.800429 pygpt_net-2.2.9/src/pygpt_net/data/prompts.csv
+-rwxr-xr-x   0        0        0    31708 2024-02-20 19:10:03.189314 pygpt_net-2.2.9/src/pygpt_net/data/win32/README.rtf
+-rwxr-xr-x   0        0        0     1633 2023-04-14 00:10:28.000000 pygpt_net-2.2.9/src/pygpt_net/data/win32/USER-LICENSE.rtf
+-rwxr-xr-x   0        0        0    87160 2023-04-14 00:10:28.000000 pygpt_net-2.2.9/src/pygpt_net/data/win32/pygpt.aip
+-rwxr-xr-x   0        0        0       45 2023-12-19 15:40:13.000000 pygpt_net-2.2.9/src/pygpt_net/data/win32/qt.conf
+-rw-r--r--   0        0        0    21910 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/icons.qrc
+-rw-r--r--   0        0        0    91076 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/icons_rc.py
+-rw-r--r--   0        0        0      488 2023-12-31 03:12:36.955235 pygpt_net-2.2.9/src/pygpt_net/item/__init__.py
+-rw-r--r--   0        0        0     9587 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/item/assistant.py
+-rw-r--r--   0        0        0     2110 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/item/attachment.py
+-rw-r--r--   0        0        0     2108 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/item/calendar_note.py
+-rw-r--r--   0        0        0    12376 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/item/ctx.py
+-rw-r--r--   0        0        0     1681 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/item/index.py
+-rw-r--r--   0        0        0      600 2023-12-31 03:12:34.283242 pygpt_net-2.2.9/src/pygpt_net/item/mode.py
+-rw-r--r--   0        0        0     6208 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/item/model.py
+-rw-r--r--   0        0        0     1508 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/item/notepad.py
+-rw-r--r--   0        0        0     4680 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/item/preset.py
+-rwxr-xr-x   0        0        0     8362 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/launcher.py
+-rw-r--r--   0        0        0     2849 2023-12-28 02:55:13.572642 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231227152900.py
+-rw-r--r--   0        0        0      906 2023-12-30 08:47:37.360628 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231230095000.py
+-rw-r--r--   0        0        0      901 2024-01-01 00:17:57.553256 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231231230000.py
+-rw-r--r--   0        0        0     1303 2024-01-06 06:27:36.351928 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240106060000.py
+-rw-r--r--   0        0        0      865 2024-01-07 09:35:02.638810 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240107060000.py
+-rw-r--r--   0        0        0     1756 2024-02-23 01:50:39.602419 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240222160000.py
+-rw-r--r--   0        0        0     1099 2024-02-23 06:06:25.510176 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240223050000.py
+-rw-r--r--   0        0        0      847 2024-03-03 22:43:17.403437 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240303190000.py
+-rw-r--r--   0        0        0     1110 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240408180000.py
+-rw-r--r--   0        0        0     1745 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240426050000.py
+-rw-r--r--   0        0        0     1052 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240501030000.py
+-rw-r--r--   0        0        0     1974 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/migrations/__init__.py
+-rw-r--r--   0        0        0      614 2023-12-28 02:55:13.572642 pygpt_net-2.2.9/src/pygpt_net/migrations/base.py
+-rwxr-xr-x   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.9/src/pygpt_net/plugin/__init__.py
+-rwxr-xr-x   0        0        0    15161 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/plugin/agent/__init__.py
+-rwxr-xr-x   0        0        0    23567 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/__init__.py
+-rw-r--r--   0        0        0     4929 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/simple.py
+-rwxr-xr-x   0        0        0    11433 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/worker.py
+-rwxr-xr-x   0        0        0     6940 2024-03-10 10:31:05.897000 pygpt_net-2.2.9/src/pygpt_net/plugin/audio_output/__init__.py
+-rw-r--r--   0        0        0     2340 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/plugin/audio_output/worker.py
+-rwxr-xr-x   0        0        0    12704 2024-03-18 04:54:07.637826 pygpt_net-2.2.9/src/pygpt_net/plugin/base.py
+-rwxr-xr-x   0        0        0    11734 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_api/__init__.py
+-rw-r--r--   0        0        0     6243 2024-03-16 12:28:31.211383 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_api/worker.py
+-rwxr-xr-x   0        0        0     9571 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    14580 2024-04-28 01:03:40.864507 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/runner.py
+-rw-r--r--   0        0        0     8841 2024-04-28 01:03:50.072481 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/worker.py
+-rwxr-xr-x   0        0        0     5875 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_custom/__init__.py
+-rw-r--r--   0        0        0     4507 2024-03-16 12:28:31.211383 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_custom/worker.py
+-rwxr-xr-x   0        0        0    17031 2024-04-25 01:16:54.112014 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_files/__init__.py
+-rwxr-xr-x   0        0        0    37969 2024-04-25 01:16:54.112014 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_files/worker.py
+-rwxr-xr-x   0        0        0    20404 2024-04-30 16:41:29.975888 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_history/__init__.py
+-rw-r--r--   0        0        0     6768 2024-04-30 16:41:29.975888 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_history/worker.py
+-rwxr-xr-x   0        0        0     6124 2024-03-16 12:28:31.211383 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_serial/__init__.py
+-rw-r--r--   0        0        0     8562 2024-03-16 12:28:31.211383 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_serial/worker.py
+-rwxr-xr-x   0        0        0    21060 2024-03-17 14:26:02.923314 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/__init__.py
+-rwxr-xr-x   0        0        0    12772 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/websearch.py
+-rw-r--r--   0        0        0    10794 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/worker.py
+-rwxr-xr-x   0        0        0     8163 2024-03-15 15:31:21.786121 pygpt_net-2.2.9/src/pygpt_net/plugin/crontab/__init__.py
+-rwxr-xr-x   0        0        0     2475 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/plugin/experts/__init__.py
+-rwxr-xr-x   0        0        0     2831 2024-02-18 01:14:49.758062 pygpt_net-2.2.9/src/pygpt_net/plugin/extra_prompt/__init__.py
+-rwxr-xr-x   0        0        0    14776 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/plugin/idx_llama_index/__init__.py
+-rw-r--r--   0        0        0     2825 2024-03-16 16:19:22.432875 pygpt_net-2.2.9/src/pygpt_net/plugin/idx_llama_index/worker.py
+-rwxr-xr-x   0        0        0     6579 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/plugin/openai_dalle/__init__.py
+-rwxr-xr-x   0        0        0    11659 2024-04-11 20:50:24.193030 pygpt_net-2.2.9/src/pygpt_net/plugin/openai_vision/__init__.py
+-rwxr-xr-x   0        0        0     3865 2024-03-17 13:18:45.662349 pygpt_net-2.2.9/src/pygpt_net/plugin/real_time/__init__.py
+-rw-r--r--   0        0        0      488 2023-12-25 22:13:46.802302 pygpt_net-2.2.9/src/pygpt_net/provider/__init__.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.445111 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/__init__.py
+-rw-r--r--   0        0        0     1819 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/base.py
+-rw-r--r--   0        0        0     2818 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/bing_speech_recognition.py
+-rw-r--r--   0        0        0     2904 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py
+-rw-r--r--   0        0        0     2840 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/google_speech_recognition.py
+-rw-r--r--   0        0        0     2244 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/openai_whisper.py
+-rw-r--r--   0        0        0     3129 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/openai_whisper_local.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/__init__.py
+-rw-r--r--   0        0        0     1995 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/base.py
+-rw-r--r--   0        0        0     4231 2024-02-25 00:27:02.862945 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/eleven_labs.py
+-rw-r--r--   0        0        0     4286 2024-02-25 00:27:02.862945 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/google_tts.py
+-rw-r--r--   0        0        0     4960 2024-02-24 01:55:58.449111 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/ms_azure_tts.py
+-rw-r--r--   0        0        0     3056 2024-02-24 01:55:58.449111 pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/openai_tts.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/__init__.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant/__init__.py
+-rw-r--r--   0        0        0     1186 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant/base.py
+-rw-r--r--   0        0        0     6399 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant/json_file.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/__init__.py
+-rw-r--r--   0        0        0     1291 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/base.py
+-rw-r--r--   0        0        0     5363 2024-04-29 15:13:32.575517 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py
+-rw-r--r--   0        0        0    10845 2024-04-29 15:13:32.575517 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py
+-rw-r--r--   0        0        0     1796 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py
+-rw-r--r--   0        0        0      488 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/base.py
+-rw-r--r--   0        0        0     3557 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      885 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7438 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py
+-rw-r--r--   0        0        0     2120 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py
+-rw-r--r--   0        0        0     4377 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/attachment/__init__.py
+-rw-r--r--   0        0        0     1204 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/attachment/base.py
+-rw-r--r--   0        0        0     5404 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/provider/core/attachment/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/__init__.py
+-rw-r--r--   0        0        0     1322 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/base.py
+-rw-r--r--   0        0        0     3953 2024-03-08 00:36:17.343108 pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py
+-rw-r--r--   0        0        0    11113 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/config/__init__.py
+-rw-r--r--   0        0        0     1235 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/config/base.py
+-rwxr-xr-x   0        0        0     5017 2024-04-11 01:27:21.134184 pygpt_net-2.2.9/src/pygpt_net/provider/core/config/json_file.py
+-rwxr-xr-x   0        0        0    78799 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/provider/core/config/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/__init__.py
+-rw-r--r--   0        0        0     2577 2024-04-17 05:13:33.075416 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/base.py
+-rw-r--r--   0        0        0     9815 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     3101 2024-01-23 23:46:30.499197 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py
+-rw-r--r--   0        0        0    33830 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7644 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py
+-rw-r--r--   0        0        0    11665 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/json_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/history/__init__.py
+-rw-r--r--   0        0        0      863 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/history/base.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/history/patch.py
+-rw-r--r--   0        0        0     2969 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/history/txt_file.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/__init__.py
+-rw-r--r--   0        0        0     2875 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/base.py
+-rw-r--r--   0        0        0     8502 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2972 2024-02-23 06:06:25.510176 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/patch.py
+-rw-r--r--   0        0        0    17470 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/storage.py
+-rw-r--r--   0        0        0      934 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/utils.py
+-rw-r--r--   0        0        0     6615 2024-02-23 01:50:39.606418 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/index/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/__init__.py
+-rw-r--r--   0        0        0     1062 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/base.py
+-rw-r--r--   0        0        0     4142 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/json_file.py
+-rw-r--r--   0        0        0      837 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/model/__init__.py
+-rw-r--r--   0        0        0     1246 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/model/base.py
+-rw-r--r--   0        0        0     6231 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/model/json_file.py
+-rw-r--r--   0        0        0    10462 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/core/model/patch.py
+-rw-r--r--   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/__init__.py
+-rw-r--r--   0        0        0     1262 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/base.py
+-rw-r--r--   0        0        0     3044 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py
+-rw-r--r--   0        0        0     2805 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py
+-rw-r--r--   0        0        0     7263 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py
+-rw-r--r--   0        0        0     7555 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/json_file.py
+-rw-r--r--   0        0        0      488 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/__init__.py
+-rw-r--r--   0        0        0      987 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/base.py
+-rwxr-xr-x   0        0        0     3198 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/json_file.py
+-rwxr-xr-x   0        0        0     1766 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/patch.py
+-rwxr-xr-x   0        0        0      488 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/__init__.py
+-rwxr-xr-x   0        0        0     1300 2024-02-01 01:48:09.374583 pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/base.py
+-rwxr-xr-x   0        0        0     8307 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/json_file.py
+-rw-r--r--   0        0        0     4651 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/patch.py
+-rw-r--r--   0        0        0     7410 2024-05-02 18:50:37.178695 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/__init__.py
+-rw-r--r--   0        0        0    13637 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/assistants.py
+-rw-r--r--   0        0        0     7034 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/chat.py
+-rw-r--r--   0        0        0     5876 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/completion.py
+-rw-r--r--   0        0        0     8255 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/image.py
+-rw-r--r--   0        0        0    16810 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/store.py
+-rw-r--r--   0        0        0     2072 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/summarizer.py
+-rw-r--r--   0        0        0     8266 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/vision.py
+-rw-r--r--   0        0        0        0 2024-02-20 19:10:03.189314 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/worker/__init__.py
+-rw-r--r--   0        0        0    20403 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/worker/assistants.py
+-rw-r--r--   0        0        0    15467 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/provider/gpt/worker/importer.py
+-rwxr-xr-x   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/llms/__init__.py
+-rwxr-xr-x   0        0        0     1641 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/llms/anthropic.py
+-rwxr-xr-x   0        0        0     2800 2024-03-13 15:08:01.569797 pygpt_net-2.2.9/src/pygpt_net/provider/llms/azure_openai.py
+-rw-r--r--   0        0        0     3940 2024-03-15 15:31:21.790122 pygpt_net-2.2.9/src/pygpt_net/provider/llms/base.py
+-rwxr-xr-x   0        0        0     1535 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/llms/hugging_face.py
+-rwxr-xr-x   0        0        0     1643 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/llms/llama.py
+-rwxr-xr-x   0        0        0     1517 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/llms/ollama.py
+-rwxr-xr-x   0        0        0     2727 2024-03-13 15:08:01.569797 pygpt_net-2.2.9/src/pygpt_net/provider/llms/openai.py
+-rw-r--r--   0        0        0        0 2024-01-23 23:46:30.503197 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/__init__.py
+-rw-r--r--   0        0        0     2515 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/base.py
+-rw-r--r--   0        0        0     1258 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_csv.py
+-rw-r--r--   0        0        0     1032 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_docx.py
+-rw-r--r--   0        0        0     1022 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_epub.py
+-rw-r--r--   0        0        0     1032 2024-02-28 03:58:59.309445 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_excel.py
+-rw-r--r--   0        0        0     1268 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_html.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_image_vision.py
+-rw-r--r--   0        0        0     1284 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_ipynb.py
+-rw-r--r--   0        0        0      996 2024-02-28 03:58:59.309445 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_json.py
+-rw-r--r--   0        0        0     1292 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_markdown.py
+-rw-r--r--   0        0        0     1214 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_pdf.py
+-rw-r--r--   0        0        0     1832 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_video_audio.py
+-rw-r--r--   0        0        0     1196 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_xml.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.960980 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/bitbucket/__init__.py
+-rw-r--r--   0        0        0     6194 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/__init__.py
+-rw-r--r--   0        0        0     2460 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/database/__init__.py
+-rw-r--r--   0        0        0     4228 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/database/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/github/__init__.py
+-rw-r--r--   0        0        0     4204 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/github/issues.py
+-rw-r--r--   0        0        0     3550 2024-03-01 17:40:19.825274 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/github/repo.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/__init__.py
+-rw-r--r--   0        0        0     2658 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/calendar.py
+-rw-r--r--   0        0        0     5370 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/docs.py
+-rw-r--r--   0        0        0     6772 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/gmail.py
+-rw-r--r--   0        0        0     1633 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/keep.py
+-rw-r--r--   0        0        0     5282 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/sheets.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/image_vision/__init__.py
+-rw-r--r--   0        0        0     6940 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/image_vision/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/json/__init__.py
+-rw-r--r--   0        0        0     3862 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/json/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     3940 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py
+-rw-r--r--   0        0        0        0 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1481 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/simple_csv/base.py
+-rw-r--r--   0        0        0        0 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/video_audio/__init__.py
+-rw-r--r--   0        0        0     4960 2024-03-01 03:17:53.457929 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/video_audio/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/web_page/__init__.py
+-rw-r--r--   0        0        0      556 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/web_page/base.py
+-rw-r--r--   0        0        0        0 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/yt/__init__.py
+-rw-r--r--   0        0        0     2427 2024-02-29 03:07:51.278132 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/yt/base.py
+-rw-r--r--   0        0        0      545 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/yt/utils.py
+-rw-r--r--   0        0        0     3626 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_bitbucket.py
+-rw-r--r--   0        0        0     2580 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_database.py
+-rw-r--r--   0        0        0     3832 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_github_issues.py
+-rw-r--r--   0        0        0     4377 2024-04-17 01:35:30.426055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_github_repo.py
+-rw-r--r--   0        0        0     2834 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_calendar.py
+-rw-r--r--   0        0        0     2480 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_docs.py
+-rw-r--r--   0        0        0     3582 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_drive.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_gmail.py
+-rw-r--r--   0        0        0     2412 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_keep.py
+-rw-r--r--   0        0        0     2590 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_sheets.py
+-rw-r--r--   0        0        0     4004 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py
+-rw-r--r--   0        0        0     1572 2024-03-12 06:49:17.168786 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_page.py
+-rw-r--r--   0        0        0     1584 2024-03-12 06:49:17.172787 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_rss.py
+-rw-r--r--   0        0        0     1853 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_sitemap.py
+-rw-r--r--   0        0        0     2831 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_twitter.py
+-rw-r--r--   0        0        0     1617 2024-03-12 06:49:17.172787 pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_yt.py
+-rw-r--r--   0        0        0     5976 2024-03-08 22:55:56.889343 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/__init__.py
+-rw-r--r--   0        0        0     3791 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/base.py
+-rwxr-xr-x   0        0        0     3036 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/chroma.py
+-rw-r--r--   0        0        0     3016 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/elasticsearch.py
+-rw-r--r--   0        0        0     5041 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/pinecode.py
+-rw-r--r--   0        0        0     3047 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/redis.py
+-rw-r--r--   0        0        0     2455 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/simple.py
+-rw-r--r--   0        0        0     4322 2024-03-11 03:15:21.875594 pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/temp.py
+-rw-r--r--   0        0        0      488 2024-02-24 01:55:58.449111 pygpt_net-2.2.9/src/pygpt_net/provider/web/__init__.py
+-rw-r--r--   0        0        0     1994 2024-02-27 05:21:39.771084 pygpt_net-2.2.9/src/pygpt_net/provider/web/base.py
+-rw-r--r--   0        0        0     4646 2024-02-25 00:27:02.862945 pygpt_net-2.2.9/src/pygpt_net/provider/web/google_custom_search.py
+-rw-r--r--   0        0        0     4104 2024-02-25 00:27:02.862945 pygpt_net-2.2.9/src/pygpt_net/provider/web/microsoft_bing.py
+-rw-r--r--   0        0        0     3917 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/tools/__init__.py
+-rwxr-xr-x   0        0        0     9791 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/audio_transcriber/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/audio_transcriber/ui/__init__.py
+-rw-r--r--   0        0        0     5666 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py
+-rw-r--r--   0        0        0     2116 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/tools/base.py
+-rwxr-xr-x   0        0        0    11427 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/ui/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/ui/dialogs.py
+-rw-r--r--   0        0        0     3518 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/ui/widgets.py
+-rwxr-xr-x   0        0        0     9063 2024-04-14 16:40:07.849541 pygpt_net-2.2.9/src/pygpt_net/tools/image_viewer/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/image_viewer/ui/__init__.py
+-rw-r--r--   0        0        0     4962 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/image_viewer/ui/dialogs.py
+-rwxr-xr-x   0        0        0    18833 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/browse.py
+-rw-r--r--   0        0        0     4355 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/ctx.py
+-rw-r--r--   0        0        0     7985 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/dialogs.py
+-rw-r--r--   0        0        0     4034 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/files.py
+-rw-r--r--   0        0        0    10477 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/web.py
+-rw-r--r--   0        0        0     3562 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/widgets.py
+-rwxr-xr-x   0        0        0     6028 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/media_player/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/media_player/ui/__init__.py
+-rw-r--r--   0        0        0     3590 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/media_player/ui/dialogs.py
+-rw-r--r--   0        0        0    15702 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/media_player/ui/widgets.py
+-rw-r--r--   0        0        0     8018 2024-04-14 16:40:07.849541 pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/ui/__init__.py
+-rw-r--r--   0        0        0     2906 2024-04-11 00:43:06.922864 pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/ui/dialogs.py
+-rw-r--r--   0        0        0     2754 2024-04-11 03:43:59.058733 pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/ui/widgets.py
+-rwxr-xr-x   0        0        0     6639 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-08 20:36:28.054492 pygpt_net-2.2.9/src/pygpt_net/ui/base/__init__.py
+-rw-r--r--   0        0        0     9255 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/base/config_dialog.py
+-rw-r--r--   0        0        0     3430 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/base/context_menu.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/__init__.py
+-rwxr-xr-x   0        0        0     5730 2024-04-11 20:50:24.193030 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/about.py
+-rwxr-xr-x   0        0        0     5140 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/applog.py
+-rwxr-xr-x   0        0        0     6480 2024-04-28 06:16:26.324027 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/assistant.py
+-rw-r--r--   0        0        0    22532 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/assistant_store.py
+-rwxr-xr-x   0        0        0     1765 2024-03-18 02:45:45.661442 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/changelog.py
+-rw-r--r--   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/create.py
+-rw-r--r--   0        0        0    18520 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/db.py
+-rwxr-xr-x   0        0        0     1864 2024-03-18 04:54:07.637826 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/debug.py
+-rw-r--r--   0        0        0     5835 2024-03-12 06:49:17.172787 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/dictionary.py
+-rwxr-xr-x   0        0        0     2926 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/editor.py
+-rw-r--r--   0        0        0      957 2024-04-08 04:19:15.433912 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/find.py
+-rwxr-xr-x   0        0        0     2876 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/image.py
+-rwxr-xr-x   0        0        0     2272 2024-03-18 02:45:42.817463 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/license.py
+-rwxr-xr-x   0        0        0     1823 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/logger.py
+-rw-r--r--   0        0        0    13166 2024-03-10 12:05:00.639613 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/models.py
+-rwxr-xr-x   0        0        0    20679 2024-03-12 06:49:17.172787 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/plugins.py
+-rwxr-xr-x   0        0        0     7391 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/preset.py
+-rw-r--r--   0        0        0     3796 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     4105 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/profile.py
+-rwxr-xr-x   0        0        0      973 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/rename.py
+-rwxr-xr-x   0        0        0    15114 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/settings.py
+-rw-r--r--   0        0        0      954 2024-02-26 22:26:37.124323 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/snap.py
+-rwxr-xr-x   0        0        0     2436 2024-02-25 05:55:37.513980 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/start.py
+-rwxr-xr-x   0        0        0      842 2023-12-28 18:11:19.000000 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/update.py
+-rw-r--r--   0        0        0     4275 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/dialog/workdir.py
+-rwxr-xr-x   0        0        0     9009 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/ui/dialogs.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/layout/__init__.py
+-rwxr-xr-x   0        0        0     1535 2024-04-09 20:34:52.308546 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/__init__.py
+-rwxr-xr-x   0        0        0     5518 2024-04-14 20:50:29.556142 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/attachments.py
+-rwxr-xr-x   0        0        0     5280 2024-04-29 15:13:32.575517 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/attachments_uploaded.py
+-rw-r--r--   0        0        0     5996 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/calendar.py
+-rwxr-xr-x   0        0        0     9885 2024-04-09 20:35:55.668463 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/input.py
+-rwxr-xr-x   0        0        0    18656 2024-01-01 00:17:57.553256 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/markdown.py
+-rwxr-xr-x   0        0        0    10452 2024-04-21 18:06:27.128064 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/output.py
+-rw-r--r--   0        0        0     5199 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/painter.py
+-rwxr-xr-x   0        0        0     1697 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/__init__.py
+-rwxr-xr-x   0        0        0     6648 2024-04-21 19:42:04.971470 pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/ctx_list.py
+-rwxr-xr-x   0        0        0     1441 2024-01-07 09:35:02.638810 pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/search_input.py
+-rwxr-xr-x   0        0        0     1068 2023-12-31 01:26:09.880264 pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/video.py
+-rwxr-xr-x   0        0        0     1405 2024-01-31 15:19:17.742029 pygpt_net-2.2.9/src/pygpt_net/ui/layout/status.py
+-rwxr-xr-x   0        0        0     3477 2024-04-27 14:05:11.727541 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/__init__.py
+-rw-r--r--   0        0        0     2385 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/agent.py
+-rwxr-xr-x   0        0        0     4436 2024-04-30 02:35:43.578880 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/assistants.py
+-rwxr-xr-x   0        0        0     4555 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/footer.py
+-rwxr-xr-x   0        0        0     2382 2024-01-21 16:42:14.672394 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/image.py
+-rw-r--r--   0        0        0     7007 2024-04-30 16:41:29.979888 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/indexes.py
+-rwxr-xr-x   0        0        0     3169 2024-02-21 03:55:24.484309 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/mode.py
+-rwxr-xr-x   0        0        0     3067 2024-02-21 03:55:24.484309 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/model.py
+-rwxr-xr-x   0        0        0     5109 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/presets.py
+-rwxr-xr-x   0        0        0     3242 2024-03-15 15:31:21.790122 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/prompt.py
+-rwxr-xr-x   0        0        0     2447 2023-12-31 01:26:09.000000 pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/vision.py
+-rw-r--r--   0        0        0     9644 2024-04-29 05:51:11.644212 pygpt_net-2.2.9/src/pygpt_net/ui/main.py
+-rw-r--r--   0        0        0     1784 2024-03-26 17:12:51.294309 pygpt_net-2.2.9/src/pygpt_net/ui/menu/__init__.py
+-rw-r--r--   0        0        0     5067 2024-04-19 00:32:20.498428 pygpt_net-2.2.9/src/pygpt_net/ui/menu/about.py
+-rw-r--r--   0        0        0     1655 2024-03-20 16:01:43.283339 pygpt_net-2.2.9/src/pygpt_net/ui/menu/audio.py
+-rw-r--r--   0        0        0     8291 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/menu/config.py
+-rw-r--r--   0        0        0     5185 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/ui/menu/debug.py
+-rw-r--r--   0        0        0     3356 2024-04-17 05:13:33.075416 pygpt_net-2.2.9/src/pygpt_net/ui/menu/file.py
+-rw-r--r--   0        0        0      897 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/ui/menu/lang.py
+-rw-r--r--   0        0        0     2880 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/ui/menu/plugins.py
+-rwxr-xr-x   0        0        0     3440 2024-04-24 23:37:32.616565 pygpt_net-2.2.9/src/pygpt_net/ui/menu/theme.py
+-rw-r--r--   0        0        0     1134 2024-03-26 17:12:51.298308 pygpt_net-2.2.9/src/pygpt_net/ui/menu/tools.py
+-rw-r--r--   0        0        0     2026 2024-03-20 16:01:43.283339 pygpt_net-2.2.9/src/pygpt_net/ui/menu/video.py
+-rw-r--r--   0        0        0     6711 2024-04-14 20:50:29.556142 pygpt_net-2.2.9/src/pygpt_net/ui/tray.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 18:11:19.000000 pygpt_net-2.2.9/src/pygpt_net/ui/widget/__init__.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/__init__.py
+-rwxr-xr-x   0        0        0     1721 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/input.py
+-rw-r--r--   0        0        0     3771 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/input_button.py
+-rwxr-xr-x   0        0        0     1586 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/output.py
+-rw-r--r--   0        0        0        0 2024-01-06 03:25:04.270157 pygpt_net-2.2.9/src/pygpt_net/ui/widget/calendar/__init__.py
+-rw-r--r--   0        0        0     8120 2024-04-27 07:58:32.754704 pygpt_net-2.2.9/src/pygpt_net/ui/widget/calendar/select.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/__init__.py
+-rwxr-xr-x   0        0        0     1429 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/alert.py
+-rw-r--r--   0        0        0     1502 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/applog.py
+-rw-r--r--   0        0        0     1712 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/assistant_store.py
+-rw-r--r--   0        0        0      551 2024-03-26 17:12:51.298308 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/audio.py
+-rwxr-xr-x   0        0        0     3802 2024-04-11 03:43:59.058733 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/base.py
+-rwxr-xr-x   0        0        0     2302 2024-04-12 10:08:45.275113 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/confirm.py
+-rw-r--r--   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/create.py
+-rw-r--r--   0        0        0     1585 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/db.py
+-rwxr-xr-x   0        0        0     1572 2024-02-21 16:35:35.211671 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/debug.py
+-rwxr-xr-x   0        0        0     1749 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/editor.py
+-rwxr-xr-x   0        0        0     6185 2024-04-14 16:40:07.849541 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/editor_file.py
+-rw-r--r--   0        0        0     3242 2024-04-11 03:43:59.058733 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/find.py
+-rwxr-xr-x   0        0        0      816 2024-03-26 17:12:51.298308 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/image.py
+-rwxr-xr-x   0        0        0     1568 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/info.py
+-rw-r--r--   0        0        0     1717 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/license.py
+-rwxr-xr-x   0        0        0     1627 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/logger.py
+-rw-r--r--   0        0        0     1625 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 01:07:30.188635 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/preset_plugins.py
+-rw-r--r--   0        0        0     6686 2024-04-19 00:32:20.502428 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/profile.py
+-rwxr-xr-x   0        0        0     2191 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/rename.py
+-rwxr-xr-x   0        0        0     1614 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/settings.py
+-rwxr-xr-x   0        0        0     1696 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/settings_plugin.py
+-rw-r--r--   0        0        0     2724 2024-02-26 22:26:37.124323 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/snap.py
+-rwxr-xr-x   0        0        0     6789 2024-02-17 21:22:47.345663 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/update.py
+-rw-r--r--   0        0        0     1523 2024-03-26 17:12:51.298308 pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/workdir.py
+-rwxr-xr-x   0        0        0      488 2024-01-11 15:56:53.277343 pygpt_net-2.2.9/src/pygpt_net/ui/widget/draw/__init__.py
+-rw-r--r--   0        0        0    10903 2024-04-12 07:23:35.946682 pygpt_net-2.2.9/src/pygpt_net/ui/widget/draw/painter.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-29 15:13:32.575517 pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/button.py
+-rw-r--r--   0        0        0     2532 2024-03-07 01:04:26.445956 pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/checkbox.py
+-rwxr-xr-x   0        0        0     2559 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/group.py
+-rw-r--r--   0        0        0     3789 2024-02-28 03:58:59.313445 pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/labels.py
+-rwxr-xr-x   0        0        0        0 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/filesystem/__init__.py
+-rwxr-xr-x   0        0        0    22934 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/widget/filesystem/explorer.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/image/__init__.py
+-rwxr-xr-x   0        0        0     3797 2024-03-26 17:12:51.298308 pygpt_net-2.2.9/src/pygpt_net/ui/widget/image/display.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/__init__.py
+-rwxr-xr-x   0        0        0     2682 2024-01-29 13:41:53.379769 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/assistant.py
+-rw-r--r--   0        0        0     3715 2024-04-29 15:13:32.575517 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/assistant_store.py
+-rwxr-xr-x   0        0        0     7055 2024-04-14 20:50:29.556142 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/attachment.py
+-rwxr-xr-x   0        0        0     2435 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/base.py
+-rwxr-xr-x   0        0        0    17502 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/context.py
+-rw-r--r--   0        0        0     5861 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/db.py
+-rw-r--r--   0        0        0     3658 2024-03-07 01:04:26.449956 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/debug.py
+-rw-r--r--   0        0        0     5739 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/experts.py
+-rw-r--r--   0        0        0     4818 2024-04-17 01:35:30.430055 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/index.py
+-rw-r--r--   0        0        0     6794 2024-04-27 14:05:11.727541 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/index_combo.py
+-rwxr-xr-x   0        0        0     1080 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/mode.py
+-rwxr-xr-x   0        0        0     1912 2024-01-29 13:41:53.379769 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/model.py
+-rw-r--r--   0        0        0     1919 2024-01-29 13:41:53.379769 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/model_editor.py
+-rwxr-xr-x   0        0        0     1028 2024-01-12 09:25:47.589375 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/plugin.py
+-rwxr-xr-x   0        0        0     5655 2024-05-01 18:08:40.482948 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/preset.py
+-rw-r--r--   0        0        0     3899 2024-03-07 01:04:26.449956 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/preset_plugins.py
+-rw-r--r--   0        0        0     4432 2024-04-10 01:07:30.192635 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/profile.py
+-rw-r--r--   0        0        0     1052 2024-01-12 09:25:47.589375 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/settings.py
+-rwxr-xr-x   0        0        0     4382 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/uploaded.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.362230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/__init__.py
+-rwxr-xr-x   0        0        0     2068 2024-01-19 21:21:41.774598 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/checkbox.py
+-rw-r--r--   0        0        0     5503 2024-03-12 06:49:17.172787 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/cmd.py
+-rw-r--r--   0        0        0     3594 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/combo.py
+-rwxr-xr-x   0        0        0    13004 2024-05-02 18:50:37.182695 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/dictionary.py
+-rwxr-xr-x   0        0        0     9304 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/input.py
+-rw-r--r--   0        0        0     2601 2024-04-22 22:35:26.800429 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/prompt.py
+-rwxr-xr-x   0        0        0     3569 2024-01-08 20:36:28.058493 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/slider.py
+-rwxr-xr-x   0        0        0     2684 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/textarea.py
+-rw-r--r--   0        0        0     1668 2024-01-29 13:41:53.379769 pygpt_net-2.2.9/src/pygpt_net/ui/widget/tabs/Input.py
+-rw-r--r--   0        0        0      488 2023-12-30 09:04:29.205425 pygpt_net-2.2.9/src/pygpt_net/ui/widget/tabs/__init__.py
+-rw-r--r--   0        0        0     2814 2024-04-10 01:07:30.192635 pygpt_net-2.2.9/src/pygpt_net/ui/widget/tabs/output.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-21 01:33:54.247764 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/calendar_note.py
+-rw-r--r--   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/create.py
+-rw-r--r--   0        0        0     5450 2024-04-21 01:33:54.247764 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/editor.py
+-rw-r--r--   0        0        0     1543 2024-04-11 03:43:59.058733 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/find.py
+-rwxr-xr-x   0        0        0     6059 2024-04-22 22:35:26.800429 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/input.py
+-rwxr-xr-x   0        0        0     1132 2024-01-27 21:42:30.964980 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/name.py
+-rwxr-xr-x   0        0        0     6583 2024-04-21 01:33:54.247764 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/notepad.py
+-rwxr-xr-x   0        0        0     5086 2024-04-23 23:11:13.260159 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/output.py
+-rwxr-xr-x   0        0        0     1358 2024-01-28 19:32:28.495073 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/rename.py
+-rwxr-xr-x   0        0        0     1833 2024-04-12 10:08:45.275113 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/search_input.py
+-rwxr-xr-x   0        0        0    10060 2024-04-27 14:05:11.727541 pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/web.py
+-rwxr-xr-x   0        0        0      488 2023-12-28 21:20:40.366230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/vision/__init__.py
+-rwxr-xr-x   0        0        0     2584 2023-12-28 21:20:40.366230 pygpt_net-2.2.9/src/pygpt_net/ui/widget/vision/camera.py
+-rwxr-xr-x   0        0        0     5470 2024-04-26 21:55:50.679597 pygpt_net-2.2.9/src/pygpt_net/utils.py
+-rw-r--r--   0        0        0   143954 1970-01-01 00:00:00.000000 pygpt_net-2.2.9/PKG-INFO
```

### Comparing `pygpt_net-2.2.8/CHANGELOG.md` & `pygpt_net-2.2.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+# 2.2.9 (2024-05-02)
+
+- Added more commands to voice control: search for contexts, clear search, add, read and clear calendar memos, context rename.
+
 # 2.2.8 (2024-05-02)
 
 - Added support for disabled people, including voice control and screen event translation with audio synthesis.
 - A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
 - A new section called 'Accessibility' has been added to the Documentation.
 
 # 2.2.7 (2024-05-01)
```

### Comparing `pygpt_net-2.2.8/LICENSE` & `pygpt_net-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/README.md` & `pygpt_net-2.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.8** | build: **2024.05.02** | Python: **>=3.10, <3.12**
+Release: **2.2.9** | build: **2024.05.02** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -898,14 +898,17 @@
 
 - Get the current application status
 - Exit the application
 - Enable audio output
 - Disable audio output
 - Enable audio input
 - Disable audio input
+- Add a memo to the calendar
+- Clear memos from calendar
+- Read the calendar memos
 - Enable the camera
 - Disable the camera
 - Capture the camera
 - Create a new context
 - Go to the previous context
 - Go to the next context
 - Go to the last context
@@ -913,19 +916,23 @@
 - Send the input
 - Clear the input
 - Get current conversation info
 - Stop executing current action
 - Clear the attachments
 - Read the last conversation entry
 - Read the whole conversation
+- Rename current context
+- Search for a string in the conversation
+- Clear the search results
 - Send the message to input
 - Append message to current input without sending it
 - Switch to chat mode
 - Switch to Chat with files (llama-index) mode
 - Add note to notepad
+- Clear notepad contents
 - Read current notepad contents
 - Switch to the chat tab
 - Switch to the calendar tab
 - Switch to the draw (painter) tab
 - Switch to the files tab
 - Switch to the notepad tab
 - Switch to the next tab
@@ -3194,14 +3201,18 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.9 (2024-05-02)**
+
+- Added more commands to voice control: search for contexts, clear search, add, read and clear calendar memos, context rename.
+
 **2.2.8 (2024-05-02)**
 
 - Added support for disabled people, including voice control and screen event translation with audio synthesis.
 - A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
 - A new section called 'Accessibility' has been added to the Documentation.
 
 **2.2.7 (2024-05-01)**
```

### Comparing `pygpt_net-2.2.8/icon.png` & `pygpt_net-2.2.9/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/pyproject.toml` & `pygpt_net-2.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygpt-net"
-version = "2.2.8"
+version = "2.2.9"
 description = "Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more"
 authors = ["Marcin Szczyglinski <info@pygpt.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/szczyglis-dev/py-gpt"
 repository = "https://github.com/szczyglis-dev/py-gpt"
 documentation = "https://pygpt.readthedocs.io/"
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/CHANGELOG.txt` & `pygpt_net-2.2.9/src/pygpt_net/CHANGELOG.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2.2.9 (2024-05-02)
+
+- Added more commands to voice control: search for contexts, clear search, add, read and clear calendar memos, context rename.
+
 2.2.8 (2024-05-02)
 
 - Added support for disabled people, including voice control and screen event translation with audio synthesis.
 - A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
 - A new section called 'Accessibility' has been added to the Documentation.
 
 2.2.7 (2024-05-01)
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/LICENSE` & `pygpt_net-2.2.9/src/pygpt_net/LICENSE`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 # -*- coding: utf-8 -*-
 # ================================================== #
 # This file is a part of PYGPT package               #
 # Website: https://pygpt.net                         #
 # GitHub:  https://github.com/szczyglis-dev/py-gpt   #
 # MIT License                                        #
 # Created By  : Marcin Szczygliński                  #
-# Updated Date: 2024.05.02 18:00:00                  #
+# Updated Date: 2024.05.02 22:00:00                  #
 # ================================================== #
 
 __author__ = "Marcin Szczygliński"
 __copyright__ = "Copyright 2024, Marcin Szczygliński"
 __credits__ = ["Marcin Szczygliński"]
 __license__ = "MIT"
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __build__ = "2024.05.02"
 __maintainer__ = "Marcin Szczygliński"
 __github__ = "https://github.com/szczyglis-dev/py-gpt"
 __website__ = "https://pygpt.net"
 __pypi__ = "https://pypi.org/project/pygpt-net"
 __snap__ = "https://snapcraft.io/pygpt"
 __donate__ = "https://pygpt.net/#donate"
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/app.py` & `pygpt_net-2.2.9/src/pygpt_net/app.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/config.py` & `pygpt_net-2.2.9/src/pygpt_net/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/container.py` & `pygpt_net-2.2.9/src/pygpt_net/container.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/access/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/access/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/access/control.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/access/control.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,30 +19,43 @@
     def __init__(self, window=None):
         """
         Control handler
 
         :param window: Window instance
         """
         self.window = window
+        self.last_confirm = None
 
-    def handle(self, event: ControlEvent):
+    def handle(self, event: ControlEvent, force: bool = False):
         """
         Handle accessibility event (control)
 
         :param event: event object
+        :param force: force handle
         """
         self.window.core.debug.info("EVENT CTRL: " + event.name)
+
+        # reset last confirm
+        if event.name != ControlEvent.CMD_CONFIRM:
+            self.last_confirm = None
+
         # app
         if event.name == ControlEvent.APP_EXIT:
             self.window.close()
         elif event.name == ControlEvent.APP_STATUS:
             status = self.window.core.access.voice.get_status()
             if status != "":
                 self.window.controller.audio.read_text(status)
 
+        # confirm last action
+        elif event.name == ControlEvent.CMD_CONFIRM:
+            if self.last_confirm is not None:
+                self.handle(self.last_confirm, force=True)
+                self.last_confirm = None
+
         # camera
         elif event.name == ControlEvent.CAMERA_ENABLE:
             self.window.controller.camera.enable_capture()
         elif event.name == ControlEvent.CAMERA_DISABLE:
             self.window.controller.camera.disable_capture()
         elif event.name == ControlEvent.CAMERA_CAPTURE:
             self.window.controller.camera.manual_capture()
@@ -74,21 +87,57 @@
             text = self.window.core.access.voice.get_last_ctx_item()
             if text != "":
                 self.window.controller.audio.read_text(text)
         elif event.name == ControlEvent.CTX_READ_ALL:
             text = self.window.core.access.voice.get_all_ctx_items()
             if text != "":
                 self.window.controller.audio.read_text(text)
+        elif event.name == ControlEvent.CTX_RENAME:
+            if event.data is not None and "params" in event.data:
+                msg = event.data["params"]
+                if msg != "":
+                    self.window.controller.ctx.update_name_current(msg)
+                    msg = trans("event.audio.ctx.rename").format(ctx=msg)
+                    self.window.controller.audio.read_text(msg)
+        elif event.name == ControlEvent.CTX_SEARCH_STRING:
+            if event.data is not None and "params" in event.data:
+                msg = event.data["params"]
+                if msg != "":
+                    self.window.controller.ctx.append_search_string(msg)
+                    num = self.window.core.ctx.count_found_meta()
+                    msg = trans("event.audio.ctx.search.string").format(num=num)
+                    self.window.controller.audio.read_text(msg)
+        elif event.name == ControlEvent.CTX_SEARCH_CLEAR:
+                self.window.controller.ctx.search_string_clear()
+                self.handle_result(event, True)
+
+        # calendar
+        elif event.name == ControlEvent.CALENDAR_ADD:
+            if event.data is not None and "params" in event.data:
+                msg = event.data["params"]
+                if msg != "":
+                    self.window.controller.calendar.note.append_text(msg)
+                    self.handle_result(event, True)
+        elif event.name == ControlEvent.CALENDAR_CLEAR:
+            if force:
+                self.window.controller.calendar.note.clear_note()
+                self.handle_result(event, True)
+            else:
+                self.last_confirm = event
+                self.window.controller.audio.read_text(trans("event.audio.confirm"))
+        elif event.name == ControlEvent.CALENDAR_READ:
+            text = self.window.controller.calendar.note.get_note_text()
+            self.window.controller.audio.read_text(text)
 
         # mode
         elif event.name == ControlEvent.MODE_CHAT:
             self.window.controller.mode.set("chat")
             self.handle_result(event, True)
         elif event.name == ControlEvent.MODE_LLAMA_INDEX:
-            self.window.controller.mode.se("llama_index")
+            self.window.controller.mode.set("llama_index")
             self.handle_result(event, True)
 
         # tabs
         elif event.name == ControlEvent.TAB_NEXT:
             self.window.controller.ui.next_tab()
         elif event.name == ControlEvent.TAB_PREV:
             self.window.controller.ui.prev_tab()
@@ -175,14 +224,34 @@
                 if msg != "":
                     if self.window.controller.notepad.is_active():
                         idx = self.window.controller.notepad.get_current_active()
                         self.window.controller.notepad.append_text(msg, idx)
                     else:
                         self.window.controller.notepad.append_text(msg, 1)
                     self.handle_result(event, True)
+        elif event.name == ControlEvent.NOTEPAD_CLEAR:
+            if force:
+                if event.data is not None and "params" in event.data and event.data["params"] != "":
+                    idx = 1
+                    try:
+                        # regex extract number
+                        num = re.findall(r'\d+', event.data["params"])
+                        if len(num) > 0:
+                            idx = int(num[0])
+                    except:
+                        pass
+                    if self.window.controller.notepad.clear(idx):
+                        self.handle_result(event, True)
+                else:
+                    idx = self.window.controller.notepad.get_current_active()
+                    if idx is not None and self.window.controller.notepad.clear(idx):
+                        self.handle_result(event, True)
+            else:
+                self.last_confirm = event
+                self.window.controller.audio.read_text(trans("event.audio.confirm"))
         elif event.name == ControlEvent.NOTEPAD_READ:
             if event.data is not None and "params" in event.data and event.data["params"] != "":
                 idx = 1
                 try:
                     # regex extract number
                     num = re.findall(r'\d+', event.data["params"])
                     if len(num) > 0:
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/access/voice.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/access/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,18 @@
         self.timer = None
         self.input_file = "voice_control.wav"
         self.thread_started = False
         self.audio_disabled_events = [
             AppEvent.INPUT_CALL,
             AppEvent.VOICE_CONTROL_TOGGLE,
         ]
+        self.confirm_events = [
+            ControlEvent.NOTEPAD_CLEAR,
+            ControlEvent.CALENDAR_CLEAR,
+        ]
 
     def setup(self):
         """Setup voice control"""
         self.update()
 
     def play(self, event: AppEvent):
         """
@@ -267,16 +271,20 @@
                 event = ControlEvent(cmd)
                 event.data = {
                     "params": params,
                 }
                 self.window.core.dispatcher.dispatch(event)
                 self.window.core.debug.info("VOICE CONTROL COMMAND: " + cmd, params)
                 trans_key = "event.control." + cmd
-                self.window.ui.status("Voice command: " + trans(trans_key))
-                QApplication.processEvents()
+
+                if cmd in self.confirm_events:
+                    self.window.ui.status(trans("event.audio.confirm"))
+                else:
+                    self.window.ui.status("Voice command: " + trans(trans_key))
+                    QApplication.processEvents()
 
             # play OK sound
             if self.window.core.config.get("access.audio.notify.execute"):
                 self.window.controller.audio.play_sound("ok.mp3")
 
         else:
             self.window.ui.status("Voice command not recognized.")
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/agent/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/agent/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/agent/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/agent/experts.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/agent/experts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/agent/flow.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/agent/flow.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/batch.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/batch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/files.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/store.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/assistant/threads.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/assistant/threads.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/attachment.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/audio/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/calendar/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/calendar/note.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/calendar/note.py`

 * *Files 4% similar despite different names*

```diff
@@ -257,7 +257,21 @@
         self.window.ui.calendar['note'].setText(new_text)
         self.update()
 
         # move cursor to end
         cursor = self.window.ui.calendar['note'].textCursor()
         cursor.movePosition(QTextCursor.End)
         self.window.ui.calendar['note'].setTextCursor(cursor)
+
+    def clear_note(self):
+        """Clear note"""
+        self.window.ui.calendar['note'].clear()
+        self.update()
+        self.window.ui.calendar['note'].on_update()
+
+    def get_note_text(self) -> str:
+        """
+        Get notepad text
+
+        :return: notepad text
+        """
+        return self.window.ui.calendar['note'].toPlainText()
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/camera.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/files.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/image.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/input.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/output.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/render.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/render.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/text.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/text.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/chat/vision.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/chat/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/command.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/checkbox.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/cmd.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/combo.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/dictionary.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/input.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/slider.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/field/textarea.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/field/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/config/placeholder.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/config/placeholder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ctx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,14 +579,22 @@
             self.window.ui.dialog['rename'].close()
 
         if refresh:
             self.update()
         else:
             self.update(True, False)
 
+    def update_name_current(self, name: str):
+        """
+        Update current ctx name
+
+        :param name: context name
+        """
+        self.update_name(self.window.core.ctx.current, name)
+
     def handle_allowed(self, mode: str) -> bool:
         """
         Check if append to current ctx is allowed for this mode, if not then switch to new context
 
         :param mode: mode name
         :return: True if allowed
         """
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ctx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/extra.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ctx/extra.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ctx/summarizer.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ctx/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/debug/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/confirm.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/debug.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/dialogs/info.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/dialogs/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/files.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/finder.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/idx/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/idx/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/idx/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/idx/indexer.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/idx/indexer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/idx/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/idx/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/lang/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/lang/custom.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/lang/custom.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/lang/mapping.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/lang/mapping.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/lang/plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/lang/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/lang/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/lang/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/launcher.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/layout.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/layout.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/mode.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/model/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/model/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/model/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/notepad.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/notepad.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,7 +370,19 @@
 
         :param idx: notepad index
         :return: notepad text
         """
         if idx in self.window.ui.notepad:
             return self.window.ui.notepad[idx].toPlainText()
         return ""
+
+    def clear(self, idx: int) -> bool:
+        """
+        Clear notepad contents
+
+        :param idx: notepad idx
+        """
+        if idx in self.window.ui.notepad:
+            self.window.ui.notepad[idx].textarea.clear()
+            self.save(idx)
+            return True
+        return False
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/painter/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/painter/capture.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/painter/capture.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/painter/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/painter/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/presets.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/plugins/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/plugins/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/plugins/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/presets/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/presets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/presets/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/presets/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/presets/experts.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/presets/experts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/settings/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/settings/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/settings/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/settings/profile.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/settings/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/settings/workdir.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/settings/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/theme/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/theme/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/theme/common.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/theme/common.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/theme/markdown.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/theme/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/theme/menu.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/theme/menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,20 +83,20 @@
         for value in self.density_values:
             self.window.ui.menu['theme.layout.density'][value].setChecked(False)
             if value == current_density:
                 self.window.ui.menu['theme.layout.density'][value].setChecked(True)
 
     def update_list(self):
         """Update theme list menu"""
+        current = self.window.core.config.get('theme')
         for theme in self.window.ui.menu['theme']:
             self.window.ui.menu['theme'][theme].setChecked(False)
-        current = self.window.core.config.get('theme')
         if current in self.window.ui.menu['theme']:
             self.window.ui.menu['theme'][current].setChecked(True)
 
     def update_syntax(self):
         """Update syntax menu"""
+        current = self.window.core.config.get('render.code_syntax')
         for style in self.window.ui.menu['theme_syntax']:
             self.window.ui.menu['theme_syntax'][style].setChecked(False)
-        current = self.window.core.config.get('render.code_syntax')
         if current in self.window.ui.menu['theme_syntax']:
             self.window.ui.menu['theme_syntax'][current].setChecked(True)
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/theme/nodes.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/theme/nodes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ui/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ui/mode.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ui/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/controller/ui/vision.py` & `pygpt_net-2.2.9/src/pygpt_net/controller/ui/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/access/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/access/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/access/actions.py` & `pygpt_net-2.2.9/src/pygpt_net/core/access/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/access/events.py` & `pygpt_net-2.2.9/src/pygpt_net/core/access/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 from pygpt_net.core.dispatcher import BaseEvent
 
 
 class ControlEvent(BaseEvent):
     """Events used for app control"""
     APP_STATUS = "app.status"
     APP_EXIT = "app.exit"
+    CMD_CONFIRM = "cmd.confirm"
     AUDIO_OUTPUT_ENABLE = "audio.output.enable"
     AUDIO_OUTPUT_DISABLE = "audio.output.disable"
     AUDIO_INPUT_ENABLE = "audio.input.enable"
     AUDIO_INPUT_DISABLE = "audio.input.disable"
+    CALENDAR_ADD = "calendar.add"
+    CALENDAR_CLEAR = "calendar.clear"
+    CALENDAR_READ = "calendar.read"
     CAMERA_ENABLE = "camera.enable"
     CAMERA_DISABLE = "camera.disable"
     CAMERA_CAPTURE = "camera.capture"
     CTX_NEW = "ctx.new"
     CTX_PREV = "ctx.prev"
     CTX_NEXT = "ctx.next"
     CTX_LAST = "ctx.last"
@@ -31,19 +35,23 @@
     CTX_INPUT_SEND = "ctx.input.send"
     CTX_INPUT_CLEAR = "ctx.input.clear"
     CTX_STOP = "ctx.stop"
     CTX_ATTACHMENTS_CLEAR = "ctx.attachments.clear"
     CTX_CURRENT = "ctx.current"
     CTX_READ_LAST = "ctx.read.last"
     CTX_READ_ALL = "ctx.read.all"
+    CTX_RENAME = "ctx.rename"
+    CTX_SEARCH_STRING = "ctx.search.string"
+    CTX_SEARCH_CLEAR = "ctx.search.clear"
     INPUT_SEND = "input.send"
     INPUT_APPEND = "input.append"
     MODE_CHAT = "mode.chat"
     MODE_LLAMA_INDEX = "mode.llama_index"
     NOTE_ADD = "note.add"
+    NOTEPAD_CLEAR = "notepad.clear"
     NOTEPAD_READ = "notepad.read"
     TAB_CHAT = "tab.chat"
     TAB_CALENDAR = "tab.calendar"
     TAB_DRAW = "tab.draw"
     TAB_FILES = "tab.files"
     TAB_NOTEPAD = "tab.notepad"
     TAB_NEXT = "tab.next"
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/access/shortcuts.py` & `pygpt_net-2.2.9/src/pygpt_net/core/access/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/access/voice.py` & `pygpt_net-2.2.9/src/pygpt_net/core/access/voice.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,34 +28,42 @@
         self.commands = {
             ControlEvent.APP_STATUS: "Get the current application status",
             ControlEvent.APP_EXIT: "Exit the application",
             ControlEvent.AUDIO_OUTPUT_ENABLE: "Enable audio output",
             ControlEvent.AUDIO_OUTPUT_DISABLE: "Disable audio output",
             ControlEvent.AUDIO_INPUT_ENABLE: "Enable audio input",
             ControlEvent.AUDIO_INPUT_DISABLE: "Disable audio input",
+            ControlEvent.CALENDAR_ADD: "Add a memo to the calendar",
+            ControlEvent.CALENDAR_CLEAR: "Clear memos from calendar",
+            ControlEvent.CALENDAR_READ: "Read the calendar memos",
             ControlEvent.CAMERA_ENABLE: "Enable the camera",
             ControlEvent.CAMERA_DISABLE: "Disable the camera",
             ControlEvent.CAMERA_CAPTURE: "Capture the camera",
+            ControlEvent.CMD_CONFIRM: "Confirmation of the command",
             ControlEvent.CTX_NEW: "Create a new context",
             ControlEvent.CTX_PREV: "Go to the previous context",
             ControlEvent.CTX_NEXT: "Go to the next context",
             ControlEvent.CTX_LAST: "Go to the last context",
             ControlEvent.CTX_INPUT_FOCUS: "Focus on the input",
             ControlEvent.CTX_INPUT_SEND: "Send the input",
             ControlEvent.CTX_INPUT_CLEAR: "Clear the input",
             ControlEvent.CTX_CURRENT: "Get current conversation info",
             ControlEvent.CTX_STOP: "Stop executing current action",
             ControlEvent.CTX_ATTACHMENTS_CLEAR: "Clear the attachments",
             ControlEvent.CTX_READ_LAST: "Read the last conversation entry",
             ControlEvent.CTX_READ_ALL: "Read the whole conversation",
+            ControlEvent.CTX_RENAME: "Rename current context",
+            ControlEvent.CTX_SEARCH_STRING: "Search for a string in the conversation",
+            ControlEvent.CTX_SEARCH_CLEAR: "Clear the search results",
             ControlEvent.INPUT_SEND: "Send the message to input",
             ControlEvent.INPUT_APPEND: "Append message to current input without sending it",
             ControlEvent.MODE_CHAT: "Switch to chat mode",
             ControlEvent.MODE_LLAMA_INDEX: "Switch to Chat with files (llama-index) mode",
             ControlEvent.NOTE_ADD: "Add note to notepad",
+            ControlEvent.NOTEPAD_CLEAR: "Clear notepad contents",
             ControlEvent.NOTEPAD_READ: "Read current notepad contents",
             ControlEvent.TAB_CHAT: "Switch to the chat tab",
             ControlEvent.TAB_CALENDAR: "Switch to the calendar tab",
             ControlEvent.TAB_DRAW: "Switch to the draw (painter) tab",
             ControlEvent.TAB_FILES: "Switch to the files tab",
             ControlEvent.TAB_NOTEPAD: "Switch to the notepad tab",
             ControlEvent.TAB_NEXT: "Switch to the next tab",
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/agents/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/assistants/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/assistants/files.py` & `pygpt_net-2.2.9/src/pygpt_net/core/assistants/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/assistants/store.py` & `pygpt_net-2.2.9/src/pygpt_net/core/assistants/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/attachments.py` & `pygpt_net-2.2.9/src/pygpt_net/core/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/audio.py` & `pygpt_net-2.2.9/src/pygpt_net/core/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/bridge.py` & `pygpt_net-2.2.9/src/pygpt_net/core/bridge.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/calendar/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/calendar/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/camera.py` & `pygpt_net-2.2.9/src/pygpt_net/core/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/chain/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/chain/chat.py` & `pygpt_net-2.2.9/src/pygpt_net/core/chain/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/chain/completion.py` & `pygpt_net-2.2.9/src/pygpt_net/core/chain/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/command.py` & `pygpt_net-2.2.9/src/pygpt_net/core/command.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/ctx/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/ctx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -483,14 +483,22 @@
         :return: ctx meta count
         """
         extra = 0
         if self.tmp_meta is not None:
             extra = 1  # prevent create new if tmp meta exists
         return len(self.meta) + extra
 
+    def count_found_meta(self) -> int:
+        """
+        Count ctx meta items
+
+        :return: ctx meta count
+        """
+        return len(self.meta)
+
     def all(self, meta_id: int = None) -> list:
         """
         Return ctx items (current or by meta_id if provided)
 
         :param meta_id: meta id
         :return: ctx items
         """
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/ctx/idx.py` & `pygpt_net-2.2.9/src/pygpt_net/core/ctx/idx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/db/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/db/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/db/viewer.py` & `pygpt_net-2.2.9/src/pygpt_net/core/db/viewer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/agent.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/assistants.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/attachments.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/config.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/context.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/db.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/indexes.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/models.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/presets.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/debug/ui.py` & `pygpt_net-2.2.9/src/pygpt_net/core/debug/ui.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/dispatcher.py` & `pygpt_net-2.2.9/src/pygpt_net/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/experts/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/experts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/actions.py` & `pygpt_net-2.2.9/src/pygpt_net/core/filesystem/actions.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/core/filesystem/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/types.py` & `pygpt_net-2.2.9/src/pygpt_net/core/filesystem/types.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/filesystem/url.py` & `pygpt_net-2.2.9/src/pygpt_net/core/filesystem/url.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/history.py` & `pygpt_net-2.2.9/src/pygpt_net/core/history.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/chat.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/context.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/indexing.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/indexing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/llm.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/llm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/metadata.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/metadata.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/ctx.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/types/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/external.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/types/external.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/types/files.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/types/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/idx/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/core/idx/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/image.py` & `pygpt_net-2.2.9/src/pygpt_net/core/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/info.py` & `pygpt_net-2.2.9/src/pygpt_net/core/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/installer.py` & `pygpt_net-2.2.9/src/pygpt_net/core/installer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/llm/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/locale.py` & `pygpt_net-2.2.9/src/pygpt_net/core/locale.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/models.py` & `pygpt_net-2.2.9/src/pygpt_net/core/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/modes.py` & `pygpt_net-2.2.9/src/pygpt_net/core/modes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/notepad.py` & `pygpt_net-2.2.9/src/pygpt_net/core/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/platforms.py` & `pygpt_net-2.2.9/src/pygpt_net/core/platforms.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/core/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/presets.py` & `pygpt_net-2.2.9/src/pygpt_net/core/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/profile.py` & `pygpt_net-2.2.9/src/pygpt_net/core/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/prompt/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/prompt/template.py` & `pygpt_net-2.2.9/src/pygpt_net/core/prompt/template.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/base.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/parser.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/markdown/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/markdown/renderer.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/markdown/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/plain/renderer.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/plain/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/web/parser.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/web/parser.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/render/web/renderer.py` & `pygpt_net-2.2.9/src/pygpt_net/core/render/web/renderer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/core/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/text/finder.py` & `pygpt_net-2.2.9/src/pygpt_net/core/text/finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/text/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/core/text/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/text/web_finder.py` & `pygpt_net-2.2.9/src/pygpt_net/core/text/web_finder.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/tokens.py` & `pygpt_net-2.2.9/src/pygpt_net/core/tokens.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/updater/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/core/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/web.py` & `pygpt_net-2.2.9/src/pygpt_net/core/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/core/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/core/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/audio/click_off.mp3` & `pygpt_net-2.2.9/src/pygpt_net/data/audio/click_off.mp3`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/audio/click_on.mp3` & `pygpt_net-2.2.9/src/pygpt_net/data/audio/click_on.mp3`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/audio/ok.mp3` & `pygpt_net-2.2.9/src/pygpt_net/data/audio/ok.mp3`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/config.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/config.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989959839357428%*

 * *Differences: {"'__meta__'": "{'version': '2.2.9', 'app.version': '2.2.9'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.8",
+        "app.version": "2.2.9",
         "updated_at": "2024-05-02T00:00:00",
-        "version": "2.2.8"
+        "version": "2.2.9"
     },
     "access.audio.event.speech": false,
     "access.audio.notify.execute": true,
     "access.microphone.notify": true,
     "access.shortcuts": [
         {
             "action": "voice_cmd.toggle",
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/models.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/models.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'__meta__'": "{'version': '2.2.9', 'app.version': '2.2.9'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.8",
+        "app.version": "2.2.9",
         "updated_at": "2024-05-02T00:00:00",
-        "version": "2.2.8"
+        "version": "2.2.9"
     },
     "items": {
         "dall-e-2": {
             "ctx": 0,
             "default": false,
             "id": "dall-e-2",
             "langchain": {
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/modes.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/modes.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'__meta__'": "{'version': '2.2.9', 'app.version': '2.2.9'}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "__meta__": {
-        "app.version": "2.2.8",
+        "app.version": "2.2.9",
         "updated_at": "2024-05-02T00:00:00",
-        "version": "2.2.8"
+        "version": "2.2.9"
     },
     "items": {
         "agent": {
             "default": false,
             "id": "agent",
             "label": "mode.agent",
             "name": "Agent (autonomous)"
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/batman_and_joker.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/presets/batman_and_joker.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/dalle_white_cat.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/presets/dalle_white_cat.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/presets/joke_expert.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/presets/joke_expert.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/settings.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/settings.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/config/settings_section.json` & `pygpt_net-2.2.9/src/pygpt_net/data/config/settings_section.json`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/fix_windows.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/fix_windows.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.dark.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/markdown.light.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/markdown.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/style.dark.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/style.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/style.light.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/style.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/web.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/web.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/web.dark.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/web.dark.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/css/web.light.css` & `pygpt_net-2.2.9/src/pygpt_net/data/css/web.light.css`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/Lato/OFL.txt` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/Lato/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceArgon/MonaspaceArgon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceKrypton/MonaspaceKrypton-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceNeon/MonaspaceNeon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceRadon/MonaspaceRadon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Bold.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-BoldItalic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Italic.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/MonaspaceXenon/MonaspaceXenon-Regular.otf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/OFL.txt` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf` & `pygpt_net-2.2.9/src/pygpt_net/data/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icon.ico` & `pygpt_net-2.2.9/src/pygpt_net/data/icon.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icon.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icon.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_busy.ico` & `pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_busy.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_error.ico` & `pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_error.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icon_tray_idle.ico` & `pygpt_net-2.2.9/src/pygpt_net/data/icon_tray_idle.ico`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/abc.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/abc.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/alarm.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/alarm.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/apps.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/apps.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/build.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/build.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/calendar.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/calendar.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/audio.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/audio.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/copy.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/copy.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/delete.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/delete.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/edit.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/edit.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/join.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/join.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/chat/reload.png` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/chat/reload.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/cut.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/cut.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/db.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/db.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/error.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/error.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/hearing.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/hearing.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/help.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/help.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/info.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/info.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/key.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/key.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/keyboard.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/keyboard.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/language.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/language.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/palette.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/palette.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/public_filled.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/public_filled.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/robot.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/router.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/router.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/sensors.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/sensors.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/settings.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/share.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/share.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/view.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/view.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/icons/voice.svg` & `pygpt_net-2.2.9/src/pygpt_net/data/icons/voice.svg`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.de.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.de.ini`

 * *Files 2% similar despite different names*

```diff
@@ -331,21 +331,27 @@
 dt.days_ago = vor Tagen
 dt.month = vor einem Monat
 dt.today = heute
 dt.week = vor einer Woche
 dt.weeks = vor Wochen
 dt.yesterday = gestern
 event.audio.app.started = Willkommen!
+event.audio.confirm = Bestätigen Sie diesen Befehl, indem Sie die Spracheingabe mit dem Text "Ich bestätige den Befehl" erneut senden.
 event.audio.app.status = Aktueller Modus: {mode}.\nAktuelles Gespräch: {ctx}, zuletzt aktualisiert {last}.\nGesamtzahl der Gespräche: {total}.
+event.audio.calendar.add = Notiz zum Kalender hinzugefügt.
+event.audio.calendar.clear = Notizen im Kalender gelöscht.
 event.audio.ctx.created = Neuer Kontext wurde erstellt.
 event.audio.ctx.current = Aktuelles Gespräch: {ctx}, zuletzt aktualisiert: {last}.
 event.audio.ctx.last = Ihre Eingabe: {input}. KI-Antwort: {output}.
 event.audio.ctx.end = Beendet.
 event.audio.ctx.selected = Ausgewählter Kontext: {ctx}.
 event.audio.ctx.attachments.clear = Anhangsliste leer.
+event.audio.ctx.rename = Kontext in {ctx} umbenannt.
+event.audio.ctx.search.string = Gefundene Einträge: {num}.
+event.audio.ctx.search.clear = Suchbegriff gelöscht.
 event.audio.camera.enabled = Kamera aktiviert.
 event.audio.camera.disabled = Kamera deaktiviert.
 event.audio.camera.captured = Bild wurde von der Kamera aufgenommen.
 event.audio.output.enable = Audioausgabe aktiviert.
 event.audio.output.disable = Audioausgabe deaktiviert.
 event.audio.input.append = Text zur Eingabe hinzugefügt.
 event.audio.input.call = Eingabe aufrufen.
@@ -353,43 +359,51 @@
 event.audio.input.disable = Audioeingabe aktiviert.
 event.audio.input.error = Fehler beim Senden der Eingabe aufgetreten.
 event.audio.input.sent = Eingabe gesendet.
 event.audio.input.stopped = Eingabe gestoppt.
 event.audio.input.voice.listen.started = Abhören. Bitte sprechen Sie jetzt.
 event.audio.input.voice.listen.stopped = Zuhören wurde gestoppt.
 event.audio.note.add = Notiz zum Notizblock hinzugefügt.
+event.audio.notepad.clear = Notizblock geleert.
 event.audio.tab.switch = Ausgewählter Tab ist: {tab}.
 event.audio.voice.control.toggle = Sprachsteuerung wurde umgeschaltet.
 event.audio.voice.control.started = Sprachsteuerung aktiviert.
 event.audio.voice.control.stopped = Sprachsteuerung deaktiviert.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Befehl nicht erkannt.
+event.control.cmd.confirm = Bestätigt.
 event.control.app.status = App: Status
 event.control.app.exit = App: Beenden
 event.control.audio.output.enable = Audioausgang: Aktivieren
 event.control.audio.output.disable = Audioausgang: Deaktivieren
 event.control.audio.input.enable = Audioeingang: Aktivieren
 event.control.audio.input.disable = Audioeingang: Deaktivieren
+event.control.calendar.add = Notiz zum Kalender hinzugefügt.
+event.control.calendar.clear = Notizen im Kalender gelöscht.
 event.control.camera.enable = Kamera: Aktivieren
 event.control.camera.disable = Kamera: Deaktivieren
 event.control.camera.capture = Kamera: Aufnehmen
 event.control.ctx.new = Kontext: Neu
 event.control.ctx.prev = Kontext: Zurück
 event.control.ctx.next = Kontext: Weiter
 event.control.ctx.last = Kontext: Letzter
 event.control.ctx.input.focus = Eingabe: Fokus
 event.control.ctx.input.send = Eingabe: Senden
 event.control.ctx.input.clear = Eingabe: Löschen
 event.control.ctx.stop = Eingabe: Stoppen
 event.control.ctx.attachments.clear = Anhänge: Löschen
+event.control.ctx.rename = Kontext in {ctx} umbenannt.
+event.control.ctx.search.string = Gefundene Einträge: {num}.
+event.control.ctx.search.clear = Suchbegriff gelöscht.
 event.control.input.sent = Eingabe gesendet.
 event.control.input.stopped = Eingabe gestoppt.
 event.control.mode.chat = Modus: Chat
 event.control.mode.llama_index = Modus: Chat mit Dateien
 event.control.note.add = Notiz zum Notizblock hinzugefügt.
+event.control.notepad.clear = Notizblock geleert.
 event.control.tab.chat = Tab: Chat
 event.control.tab.calendar = Tab: Kalender
 event.control.tab.draw = Tab: Zeichnen
 event.control.tab.files = Tab: Dateien
 event.control.tab.notepad = Tab: Notizblock
 event.control.tab.next = Tab: Nächster
 event.control.tab.prev = Tab: Vorheriger
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.en.ini`

 * *Files 2% similar despite different names*

```diff
@@ -434,22 +434,28 @@
 dt.days_ago = days ago
 dt.month = month ago
 dt.today = today
 dt.week = week ago
 dt.weeks = weeks ago
 dt.yesterday = yesterday
 error.assistant_not_selected = Please create, import or select assistant at first!
+event.audio.confirm = Confirm this command by sending voice input again with text "I confirm the command".
 event.audio.app.started = Welcome!
 event.audio.app.status = Current mode: {mode}.\nCurrent conversation: {ctx}, last updated {last}.\nTotal conversations: {total}.
+event.audio.calendar.add = Memo added to calendar.
+event.audio.calendar.clear = Memos cleared in calendar.
 event.audio.ctx.created = New context has been created.
 event.audio.ctx.current = Current conversation: {ctx}, last updated: {last}.
 event.audio.ctx.last = Your input: {input}. AI response: {output}.
 event.audio.ctx.end = Finished.
 event.audio.ctx.selected = Selected context: {ctx}.
 event.audio.ctx.attachments.clear = Attachments list empty.
+event.audio.ctx.rename = Context renamed to {ctx}.
+event.audio.ctx.search.string = Found records: {num}.
+event.audio.ctx.search.clear = Search string cleared.
 event.audio.camera.enabled = Camera enabled.
 event.audio.camera.disabled = Camera disabled.
 event.audio.camera.captured = Image has been captured from camera.
 event.audio.output.enable = Audio output enabled.
 event.audio.output.disable = Audio output disabled.
 event.audio.input.append = Text appended to input.
 event.audio.input.call = Input call.
@@ -457,43 +463,49 @@
 event.audio.input.disable = Audio input enabled.
 event.audio.input.error = Error occurred during sending input.
 event.audio.input.sent = Input sent.
 event.audio.input.stopped = Input stopped.
 event.audio.input.voice.listen.started = Listening. Please speak now.
 event.audio.input.voice.listen.stopped = Listening has been stopped.
 event.audio.note.add = Note added to notepad.
+event.audio.notepad.clear = Notepad cleared.
 event.audio.tab.switch = Selected Tab is: {tab}.
 event.audio.voice.control.toggle = Voice control has been toggled.
 event.audio.voice.control.started = Voice control activated.
 event.audio.voice.control.stopped = Voice control deactivated.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Unrecognized command.
+event.control.cmd.confirm = Confirmed.
 event.control.app.status = App: Status
 event.control.app.exit = App: Exit
 event.control.audio.output.enable = Audio output: Enable
 event.control.audio.output.disable = Audio output: Disable
 event.control.audio.input.enable = Audio input: Enable
 event.control.audio.input.disable = Audio input: Disable
+event.control.calendar.add = Memo added to calendar.
+event.control.calendar.clear = Memos cleared in calendar.
 event.control.camera.enable = Camera: Enable
 event.control.camera.disable = Camera: Disable
 event.control.camera.capture = Camera: Capture
 event.control.ctx.new = Context: New
 event.control.ctx.prev = Context: Prev
 event.control.ctx.next = Context: Next
 event.control.ctx.last = Context: Last
 event.control.ctx.input.focus = Input: Focus
 event.control.ctx.input.send = Input: Send
 event.control.ctx.input.clear = Input: Clear
 event.control.ctx.stop = Input: Stop
 event.control.ctx.attachments.clear = Attachments: Clear
+event.control.ctx.search.clear = Search string cleared.
 event.control.input.sent = Input sent.
 event.control.input.stopped = Input stopped.
 event.control.mode.chat = Mode: Chat
 event.control.mode.llama_index = Mode: Chat with files
 event.control.note.add = Note added to notepad.
+event.control.notepad.clear = Notepad cleared.
 event.control.tab.chat = Tab: Chat
 event.control.tab.calendar = Tab: Calendar
 event.control.tab.draw = Tab: Draw
 event.control.tab.files = Tab: Files
 event.control.tab.notepad = Tab: Notepad
 event.control.tab.next = Tab: Next
 event.control.tab.prev = Tab: Prev
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.es.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.es.ini`

 * *Files 1% similar despite different names*

```diff
@@ -331,21 +331,27 @@
 dt.week = hace una semana
 dt.weeks = hace semanas
 dt.yesterday = ayer
 dictionary.config.access.shortcuts.action = Acción a desencadenar
 dictionary.config.access.shortcuts.key = Tecla del teclado
 dictionary.config.access.shortcuts.key_modifier = Modificador del teclado
 event.audio.app.started = ¡Bienvenido!
+event.audio.confirm = Confirma este comando enviando de nuevo la entrada de voz con el texto "Confirmo el comando".
 event.audio.app.status = Modo actual: {mode}.\nConversación actual: {ctx}, última actualización {last}.\nTotal de conversaciones: {total}.
+event.audio.calendar.add = Memo añadido al calendario.
+event.audio.calendar.clear = Memos borrados en el calendario.
 event.audio.ctx.created = Se ha creado un nuevo contexto.
 event.audio.ctx.current = Conversación actual: {ctx}, última actualización: {last}.
 event.audio.ctx.last = Tu entrada: {input}. Respuesta de la IA: {output}.
 event.audio.ctx.end = Finalizado.
 event.audio.ctx.selected = Contexto seleccionado: {ctx}.
 event.audio.ctx.attachments.clear = Lista de adjuntos vacía.
+event.audio.ctx.rename = Contexto renombrado a {ctx}.
+event.audio.ctx.search.string = Registros encontrados: {num}.
+event.audio.ctx.search.clear = Cadena de búsqueda borrada.
 event.audio.camera.enabled = Cámara activada.
 event.audio.camera.disabled = Cámara desactivada.
 event.audio.camera.captured = Se ha capturado una imagen de la cámara.
 event.audio.output.enable = Salida de audio habilitada.
 event.audio.output.disable = salida de audio deshabilitada.
 event.audio.input.append = Texto anexado a la entrada.
 event.audio.input.call = Llamada de entrada.
@@ -353,43 +359,51 @@
 event.audio.input.disable = Entrada de audio deshabilitada.
 event.audio.input.error = Error ocurrido durante el envío de la entrada.
 event.audio.input.sent = Entrada enviada.
 event.audio.input.stopped = Entrada detenida.
 event.audio.input.voice.listen.started = Escuchando. Por favor habla ahora.
 event.audio.input.voice.listen.stopped = La escucha ha sido detenida.
 event.audio.note.add = Nota añad
+event.audio.notepad.clear = Bloc de notas borrado.
 event.audio.tab.switch = Pestaña seleccionada: {tab}.
 event.audio.voice.control.toggle = Control de voz conmutado.
 event.audio.voice.control.started = Control de voz activado.
 event.audio.voice.control.stopped = Control de voz desactivado.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Comando no reconocido.
+event.control.cmd.confirm = Confirmado.
 event.control.app.status = Aplicación: Estado
 event.control.app.exit = Aplicación: Salir
 event.control.audio.output.enable = Salida de audio: Habilitar
 event.control.audio.output.disable = Salida de audio: Deshabilitar
 event.control.audio.input.enable = Entrada de audio: Habilitar
 event.control.audio.input.disable = Entrada de audio: Deshabilitar
+event.control.calendar.add = Memo añadido al calendario.
+event.control.calendar.clear = Memos borrados en el calendario.
 event.control.camera.enable = Cámara: Habilitar
 event.control.camera.disable = Cámara: Deshabilitar
 event.control.camera.capture = Cámara: Capturar
 event.control.ctx.new = Contexto: Nuevo
 event.control.ctx.prev = Contexto: Anterior
 event.control.ctx.next = Contexto: Siguiente
 event.control.ctx.last = Contexto: Último
 event.control.ctx.input.focus = Entrada: Enfocar
 event.control.ctx.input.send = Entrada: Enviar
 event.control.ctx.input.clear = Entrada: Limpiar
 event.control.ctx.stop = Entrada: Detener
 event.control.ctx.attachments.clear = Adjuntos: Limpiar
+event.control.ctx.rename = Contexto renombrado a {ctx}.
+event.control.ctx.search.string = Registros encontrados: {num}.
+event.control.ctx.search.clear = Cadena de búsqueda borrada.
 event.control.input.sent = Entrada enviada.
 event.control.input.stopped = Entrada detenida.
 event.control.mode.chat = Modo: Chat
 event.control.mode.llama_index = Modo: Chat con archivos
 event.control.note.add = Nota añad
+event.control.notepad.clear = Bloc de notas borrado.
 event.control.tab.chat = Pestaña: Chat
 event.control.tab.calendar = Pestaña: Calendario
 event.control.tab.draw = Pestaña: Dibujo
 event.control.tab.files = Pestaña: Archivos
 event.control.tab.notepad = Pestaña: Bloc de notas
 event.control.tab.next = Pestaña: Siguiente
 event.control.tab.prev = Pestaña: Anterior
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.fr.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.fr.ini`

 * *Files 2% similar despite different names*

```diff
@@ -331,21 +331,27 @@
 dt.week = il y a une semaine
 dt.weeks = il y a des semaines
 dt.yesterday = hier
 dictionary.config.access.shortcuts.action = Action à déclencher
 dictionary.config.access.shortcuts.key = Touche du clavier
 dictionary.config.access.shortcuts.key_modifier = Modificateur du clavier
 event.audio.app.started = Bienvenue !
+event.audio.confirm = Confirmez cette commande en renvoyant une instruction vocale avec le texte "Je confirme la commande".
 event.audio.app.status = Mode actuel : {mode}.\nConversation actuelle: {ctx}, dernière mise à jour {last}.\nNombre total de conversations : {total}.
+event.audio.calendar.add = Mémo ajouté au calendrier.
+event.audio.calendar.clear = Mémos effacés du calendrier.
 event.audio.ctx.created = Nouveau contexte créé.
 event.audio.ctx.current = Conversation actuelle : {ctx}, dernière mise à jour : {last}.
 event.audio.ctx.last = Votre entrée : {input}. Réponse de l'IA : {output}.
 event.audio.ctx.end = Terminé.
 event.audio.ctx.selected = Contexte sélectionné : {ctx}.
 event.audio.ctx.attachments.clear = La liste des pièces jointes est vide.
+event.audio.ctx.rename = Contexte renommé en {ctx}.
+event.audio.ctx.search.string = Enregistrements trouvés : {num}.
+event.audio.ctx.search.clear = Chaîne de recherche effacée.
 event.audio.camera.enabled = Caméra activée.
 event.audio.camera.disabled = Caméra désactivée.
 event.audio.camera.captured = Image capturée de la caméra.
 event.audio.output.enable = Sortie audio activée.
 event.audio.output.disable = Sortie audio désactivée.
 event.audio.input.append = Texte ajouté à l'entrée.
 event.audio.input.call = Appel d'entrée.
@@ -353,43 +359,51 @@
 event.audio.input.disable = Entrée audio activée.
 event.audio.input.error = Erreur survenue lors de l'envoi de l'entrée.
 event.audio.input.sent = Entrée envoyée.
 event.audio.input.stopped = Entrée arrêtée.
 event.audio.input.voice.listen.started = Écoute. Veuillez parler maintenant.
 event.audio.input.voice.listen.stopped = Écoute arrêtée.
 event.audio.note.add = Note ajoutée au bloc-notes.
+event.audio.notepad.clear = Bloc-notes effacé.
 event.audio.tab.switch = Onglet sélectionné : {tab}.
 event.audio.voice.control.toggle = Contrôle vocal basculé.
 event.audio.voice.control.started = Contrôle vocal activé.
 event.audio.voice.control.stopped = Contrôle vocal désactivé.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Commande non reconnue.
+event.control.cmd.confirm = Confirmé.
 event.control.app.status = Appli : Statut
 event.control.app.exit = Appli : Quitter
 event.control.audio.output.enable = Sortie audio : Activer
 event.control.audio.output.disable = Sortie audio : Désactiver
 event.control.audio.input.enable = Entrée audio : Activer
 event.control.audio.input.disable = Entrée audio : Désactiver
+event.control.calendar.add = Mémo ajouté au calendrier.
+event.control.calendar.clear = Mémos effacés du calendrier.
 event.control.camera.enable = Caméra : Activer
 event.control.camera.disable = Caméra : Désactiver
 event.control.camera.capture = Caméra : Capturer
 event.control.ctx.new = Contexte : Nouveau
 event.control.ctx.prev = Contexte : Précédent
 event.control.ctx.next = Contexte : Suivant
 event.control.ctx.last = Contexte : Dernier
 event.control.ctx.input.focus = Entrée : Focus
 event.control.ctx.input.send = Entrée : Envoyer
 event.control.ctx.input.clear = Entrée : Effacer
 event.control.ctx.stop = Entrée : Arrêter
 event.control.ctx.attachments.clear = Pièces jointes : Effacer
+event.control.ctx.rename = Contexte renommé en {ctx}.
+event.control.ctx.search.string = Enregistrements trouvés : {num}.
+event.control.ctx.search.clear = Chaîne de recherche effacée.
 event.control.input.sent = Entrée envoyée.
 event.control.input.stopped = Entrée arrêtée.
 event.control.mode.chat = Mode : Chat
 event.control.mode.llama_index = Mode : Chat avec fichiers
 event.control.note.add = Note ajoutée au bloc-notes.
+event.control.notepad.clear = Bloc-notes effacé.
 event.control.tab.chat = Onglet : Chat
 event.control.tab.calendar = Onglet : Calendrier
 event.control.tab.draw = Onglet : Dessin
 event.control.tab.files = Onglet : Fichiers
 event.control.tab.notepad = Onglet : Bloc-notes
 event.control.tab.next = Onglet : Suivant
 event.control.tab.prev = Onglet : Précédent
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.it.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.it.ini`

 * *Files 2% similar despite different names*

```diff
@@ -331,21 +331,27 @@
 dt.week = settimana fa
 dt.weeks = settimane fa
 dt.yesterday = ieri
 dictionary.config.access.shortcuts.action = Azione da attivare
 dictionary.config.access.shortcuts.key = Tasto della tastiera
 dictionary.config.access.shortcuts.key_modifier = Modificatore della tastiera
 event.audio.app.started = Benvenuto!
+event.audio.confirm = Conferma questo comando inviando nuovamente l'input vocale con il testo "Confermo il comando".
 event.audio.app.status = Modalità corrente: {mode}.\nConversazione attuale: {ctx}, ultimo aggiornamento {last}.\nConversazioni totali: {total}.
+event.audio.calendar.add = Memo aggiunto al calendario.
+event.audio.calendar.clear = Memo cancellati dal calendario.
 event.audio.ctx.created = È stato creato un nuovo contesto.
 event.audio.ctx.current = Conversazione attuale: {ctx}, ultimo aggiornamento: {last}.
 event.audio.ctx.last = Il tuo input: {input}. Risposta dell'IA: {output}.
 event.audio.ctx.end = Finito.
 event.audio.ctx.selected = Contesto selezionato: {ctx}.
 event.audio.ctx.attachments.clear = Elenco degli allegati vuoto.
+event.audio.ctx.rename = Contesto rinominato in {ctx}.
+event.audio.ctx.search.string = Record trovati: {num}.
+event.audio.ctx.search.clear = Stringa di ricerca cancellata.
 event.audio.camera.enabled = Fotocamera attivata.
 event.audio.camera.disabled = Fotocamera disattivata.
 event.audio.camera.captured = Immagine catturata dalla fotocamera.
 event.audio.output.enable = Uscita audio attivata.
 event.audio.output.disable = Uscita audio disattivata.
 event.audio.input.append = Testo aggiunto all'input.
 event.audio.input.call = Chiamata input.
@@ -353,43 +359,51 @@
 event.audio.input.disable = Ingresso audio disattivato.
 event.audio.input.error = Errore durante l'invio dell'input.
 event.audio.input.sent = Input inviato.
 event.audio.input.stopped = Input interrotto.
 event.audio.input.voice.listen.started = Ascoltando. Si prega di parlare ora.
 event.audio.input.voice.listen.stopped = Ascolto interrotto.
 event.audio.note.add = Nota aggiunta al blocco note.
+event.audio.notepad.clear = Blocco note cancellato.
 event.audio.tab.switch = Scheda selezionata: {tab}.
 event.audio.voice.control.toggle = Controllo vocale commutato.
 event.audio.voice.control.started = Controllo vocale attivato.
 event.audio.voice.control.stopped = Controllo vocale disattivato.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Comando non riconosciuto.
+event.control.cmd.confirm = Confermato.
 event.control.app.status = App: Stato
 event.control.app.exit = App: Uscita
 event.control.audio.output.enable = Uscita audio: Attiva
 event.control.audio.output.disable = Uscita audio: Disattiva
 event.control.audio.input.enable = Ingresso audio: Attiva
 event.control.audio.input.disable = Ingresso audio: Disattiva
+event.control.calendar.add = Memo aggiunto al calendario.
+event.control.calendar.clear = Memo cancellati dal calendario.
 event.control.camera.enable = Fotocamera: Attiva
 event.control.camera.disable = Fotocamera: Disattiva
 event.control.camera.capture = Fotocamera: Cattura
 event.control.ctx.new = Contesto: Nuovo
 event.control.ctx.prev = Contesto: Precedente
 event.control.ctx.next = Contesto: Successivo
 event.control.ctx.last = Contesto: Ultimo
 event.control.ctx.input.focus = Input: Focalizza
 event.control.ctx.input.send = Input: Invia
 event.control.ctx.input.clear = Input: Pulisci
 event.control.ctx.stop = Input: Arresta
 event.control.ctx.attachments.clear = Allegati: Pulisci
+event.control.ctx.rename = Contesto rinominato in {ctx}.
+event.control.ctx.search.string = Record trovati: {num}.
+event.control.ctx.search.clear = Stringa di ricerca cancellata.
 event.control.input.sent = Input inviato.
 event.control.input.stopped = Input interrotto.
 event.control.mode.chat = Modalità: Chat
 event.control.mode.llama_index = Modalità: Chat con file
 event.control.note.add = Nota aggiunta al blocco note.
+event.control.notepad.clear = Blocco note cancellato.
 event.control.tab.chat = Scheda: Chat
 event.control.tab.calendar = Scheda: Calendario
 event.control.tab.draw = Scheda: Disegno
 event.control.tab.files = Scheda: File
 event.control.tab.notepad = Scheda: Blocco note
 event.control.tab.next = Scheda: Successiva
 event.control.tab.prev = Scheda: Precedente
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.pl.ini`

 * *Files 2% similar despite different names*

```diff
@@ -330,22 +330,28 @@
 dictionary.config.access.shortcuts.key_modifier = Modyfikator klawiatury
 dt.days_ago = dni temu
 dt.month = miesiąc temu
 dt.today = dziś
 dt.week = tydzień temu
 dt.weeks = tygodnie temu
 dt.yesterday = wczoraj
-vent.audio.app.started = Witamy!
+event.audio.app.started = Witaj!
+event.audio.confirm = Potwierdź tę komendę, ponownie wysyłając polecenie głosowe z tekstem "Potwierdzam komendę".
 event.audio.app.status = Aktualny tryb: {mode}.\nAktualna rozmowa: {ctx}, ostatnia aktualizacja {last}.\nŁączna liczba rozmów: {total}.
+event.audio.calendar.add = Notatka dodana do kalendarza.
+event.audio.calendar.clear = Notatki w kalendarzu zostały wyczyszczone.
 event.audio.ctx.created = Utworzono nowy kontekst.
 event.audio.ctx.current = Aktualna rozmowa: {ctx}, ostatnio zaktualizowana: {last}.
 event.audio.ctx.last = Twoje wejście: {input}. Odpowiedź AI: {output}.
 event.audio.ctx.end = Zakończone.
 event.audio.ctx.selected = Wybrany kontekst: {ctx}.
 event.audio.ctx.attachments.clear = Lista załączników jest pusta.
+event.audio.ctx.rename = Kontekst zmieniony na {ctx}.
+event.audio.ctx.search.string = Znaleziono rekordów: {num}.
+event.audio.ctx.search.clear = Wyczyszczono ciąg wyszukiwania.
 event.audio.camera.enabled = Kamera włączona.
 event.audio.camera.disabled = Kamera wyłączona.
 event.audio.camera.captured = Zrobiono zdjęcie z kamery.
 event.audio.output.enable = Włączono wyjście audio.
 event.audio.output.disable = Wyłączono wyjście audio.
 event.audio.input.append = Dodano tekst do wejścia.
 event.audio.input.call = Wejście rozmowy.
@@ -353,22 +359,26 @@
 event.audio.input.disable = Włączono wejście audio.
 event.audio.input.error = Wystąpił błąd podczas wysyłania wejścia.
 event.audio.input.sent = Wejście wysłane.
 event.audio.input.stopped = Wejście zatrzymane.
 event.audio.input.voice.listen.started = Nasłuchiwanie. Proszę mówić.
 event.audio.input.voice.listen.stopped = Nasłuchiwanie zatrzymane.
 event.audio.note.add = Notatka dodana do notatnika.
+event.audio.notepad.clear = Notatnik został wyczyszczony.
 event.audio.tab.switch = Wybrana zakładka to: {tab}.
 event.audio.voice.control.toggle = Kontrola głosowa została przełączona.
 event.audio.voice.control.started = Kontrola głosowa aktywowana.
 event.audio.voice.control.stopped = Kontrola głosowa dezaktywowana.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Nierozpoznane polecenie.
+event.control.cmd.confirm = Potwierdzono.
 event.control.app.status = Aplikacja: Status
 event.control.app.exit = Aplikacja: Wyjście
+event.control.calendar.add = Notatka dodana do kalendarza.
+event.control.calendar.clear = Notatki w kalendarzu zostały wyczyszczone.
 event.control.audio.output.enable = Wyjście audio: Włącz
 event.control.audio.output.disable = Wyjście audio: Wyłącz
 event.control.audio.input.enable = Wejście audio: Włącz
 event.control.audio.input.disable = Wejście audio: Wyłącz
 event.control.camera.enable = Kamera: Włącz
 event.control.camera.disable = Kamera: Wyłącz
 event.control.camera.capture = Kamera: Złap obraz
@@ -377,19 +387,23 @@
 event.control.ctx.next = Kontekst: Następny
 event.control.ctx.last = Kontekst: Ostatni
 event.control.ctx.input.focus = Wejście: Skupienie
 event.control.ctx.input.send = Wejście: Wyślij
 event.control.ctx.input.clear = Wejście: Wyczyść
 event.control.ctx.stop = Wejście: Zatrzymaj
 event.control.ctx.attachments.clear = Załączniki: Wyczyść
+event.control.ctx.rename = Kontekst zmieniony na {ctx}.
+event.controlctx.search.string = Znaleziono rekordów: {num}.
+event.control.ctx.search.clear = Wyczyszczono ciąg wyszukiwania.
 event.control.input.sent = Wejście wysłane.
 event.control.input.stopped = Wejście zatrzymane.
 event.control.mode.chat = Tryb: Czat
 event.control.mode.llama_index = Tryb: Czat z plikami
 event.control.note.add = Notatka dodana do notatnika.
+event.control.notepad.clear = Notatnik został wyczyszczony.
 event.control.tab.chat = Zakładka: Czat
 event.control.tab.calendar = Zakładka: Kalendarz
 event.control.tab.draw = Zakładka: Rysowanie
 event.control.tab.files = Zakładka: Pliki
 event.control.tab.notepad = Zakładka: Notatnik
 event.control.tab.next = Zakładka: Następna
 event.control.tab.prev = Zakładka: Poprzednia
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.uk.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.uk.ini`

 * *Files 1% similar despite different names*

```diff
@@ -328,20 +328,26 @@
 dt.days_ago = днів тому
 dt.month = місяць тому
 dt.today = сьогодні
 dt.week = тиждень тому
 dt.weeks = тижнів тому
 dt.yesterday = вчора
 event.audio.app.started = Ласкаво просимо!
+event.audio.confirm = Підтвердьте цю команду, знову надіславши голосове введення з текстом "Я підтверджую команду".
 event.audio.app.status = Поточний режим: {mode}.\nПоточна розмова: {ctx}, останнє оновлення {last}.\nЗагальна кількість розмов: {total}.
+event.audio.calendar.add = Замітку додано до календаря.
+event.audio.calendar.clear = Усі замітки в календарі видалено.
 event.audio.ctx.created = Створено новий контекст.
 event.audio.ctx.current = Поточна розмова: {ctx}, останнє оновлення: {last}.
 event.audio.ctx.last = Ваш вхід: {input}. Відповідь ШІ: {output}.
 event.audio.ctx.end = Завершено.
 event.audio.ctx.selected = Вибраний контекст: {ctx}.
+event.audio.ctx.rename = Контекст перейменовано у {ctx}.
+event.audio.ctx.search.string = Знайдено записів: {num}.
+event.audio.ctx.search.clear = Рядок пошуку очищено.
 event.audio.camera.enabled = Камера ввімкнута.
 event.audio.camera.disabled = Камера вимкнута.
 event.audio.camera.captured = З камери зроблено знімок.
 event.audio.output.enable = Аудіовихід ввімкнуто.
 event.audio.output.disable = Аудіовихід вимкнуто.
 event.audio.input.append = Текст додано до входу.
 event.audio.input.call = Вхідний виклик.
@@ -349,43 +355,51 @@
 event.audio.input.disable = Аудіовхід вимкнуто.
 event.audio.input.error = Виникла помилка під час відправлення входу.
 event.audio.input.sent = Введення надіслано.
 event.audio.input.stopped = Введення зупинено.
 event.audio.input.voice.listen.started = Слухання. Будь ласка, говоріть зараз.
 event.audio.input.voice.listen.stopped = Слухання зупинено.
 event.audio.note.add = До блокнота додано нотатку.
+event.audio.notepad.clear = Блокнот очищено.
 event.audio.tab.switch = Вибрана вкладка: {tab}.
 event.audio.voice.control.toggle = Керування голосом перемкнуто.
 event.audio.voice.control.started = Керування голосом активовано.
 event.audio.voice.control.stopped = Керування голосом деактивовано.
 event.audio.voice.control.sent = OK.
 event.audio.voice.control.unrecognized = Команду не впізнано.
+event.control.cmd.confirm = Підтверджено.
 event.control.app.status = Додаток: Статус
 event.control.app.exit = Додаток: Вихід
 event.control.audio.output.enable = Аудіовихід: Увімкнуто
 event.control.audio.output.disable = Аудіовихід: Вимкнуто
 event.control.audio.input.enable = Аудіовхід: Увімкнуто
 event.control.audio.input.disable = Аудіовхід: Вимкнуто
+event.control.calendar.add = Замітку додано до календаря.
+event.control.calendar.clear = Усі замітки в календарі видалено.
 event.control.camera.enable = Камера: Увімкнути
 event.control.camera.disable = Камера: Вимкнути
 event.control.camera.capture = Камера: Зняти
 event.control.ctx.new = Контекст: Новий
 event.control.ctx.prev = Контекст: Попередній
 event.control.ctx.next = Контекст: Наступний
 event.control.ctx.last = Контекст: Останній
 event.control.ctx.input.focus = Введення: Фокус
 event.control.ctx.input.send = Введення: Надіслати
 event.control.ctx.input.clear = Введення: Очистити
 event.control.ctx.stop = Введення: Зупинити
 event.control.ctx.attachments.clear = Вкладення: Очистити
+event.control.ctx.rename = Контекст перейменовано у {ctx}.
+event.control.ctx.search.string = Знайдено записів: {num}.
+event.control.ctx.search.clear = Рядок пошуку очищено.
 event.control.input.sent = Введення надіслано.
 event.control.input.stopped = Введення зупинено.
 event.control.mode.chat = Режим: Чат
 event.control.mode.llama_index = Режим: Чат з файлами
 event.control.note.add = До блокнота додано нотатку.
+event.control.notepad.clear = Блокнот очищено.
 event.control.tab.chat = Вкладка: Чат
 event.control.tab.calendar = Вкладка: Календар
 event.control.tab.draw = Вкладка: Малювання
 event.control.tab.files = Вкладка: Файли
 event.control.tab.notepad = Вкладка: Блокнот
 event.control.tab.next = Вкладка: Наступна
 event.control.tab.prev = Вкладка: Попередня
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/locale.zh.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/locale.zh.ini`

 * *Files 2% similar despite different names*

```diff
@@ -402,21 +402,27 @@
 dt.days_ago = 天前
 dt.month = 月前
 dt.today = 今天
 dt.week = 周前
 dt.weeks = 周前
 dt.yesterday = 昨天
 event.audio.app.started = 欢迎！
+event.audio.confirm = 通过再次发送带有文字“我确认命令”的语音输入来确认此命令。
 event.audio.app.status = 当前模式: {mode}。\n当前会话: {ctx}，最后更新 {last}。\n会话总数: {total}。
+event.audio.calendar.add = 备忘录已添加到日历。
+event.audio.calendar.clear = 日历中的备忘录已清除。
 event.audio.ctx.created = 已创建新上下文。
 event.audio.ctx.current = 当前会话: {ctx}，最后更新: {last}。
 event.audio.ctx.last = 您的输入: {input}。AI 回应: {output}。
 event.audio.ctx.end = 完成。
 event.audio.ctx.selected = 选定上下文: {ctx}。
 event.audio.ctx.attachments.clear = 附件列表为空。
+event.audio.ctx.rename = 上下文重命名为{ctx}。
+event.audio.ctx.search.string = 找到记录：{num}。
+event.audio.ctx.search.clear = 搜索字符串已清除。
 event.audio.camera.enabled = 摄像头已启用。
 event.audio.camera.disabled = 摄像头已禁用。
 event.audio.camera.captured = 已从摄像头捕获图像。
 event.audio.output.enable = 音频输出已启用。
 event.audio.output.disable = 音频输出已禁用。
 event.audio.input.append = 文本已附加到输入。
 event.audio.input.call = 输入调用。
@@ -424,43 +430,51 @@
 event.audio.input.disable = 音频输入已启用。
 event.audio.input.error = 发送输入时发生错误。
 event.audio.input.sent = 输入已发送。
 event.audio.input.stopped = 输入已停止。
 event.audio.input.voice.listen.started = 正在监听。请现在说话。
 event.audio.input.voice.listen.stopped = 监听已停止。
 event.audio.note.add = 笔记已添加到记事本。
+event.audio.notepad.clear = 记事本已清除。
 event.audio.tab.switch = 选定标签是: {tab}。
 event.audio.voice.control.toggle = 语音控制已切换。
 event.audio.voice.control.started = 语音控制已激活。
 event.audio.voice.control.stopped = 语音控制已停用。
 event.audio.voice.control.sent = 好的。
 event.audio.voice.control.unrecognized = 无法识别的命令。
+event.control.cmd.confirm = 已确认。
 event.control.app.status = 应用程序：状态
 event.control.app.exit = 应用程序：退出
 event.control.audio.output.enable = 音频输出：启用
 event.control.audio.output.disable = 音频输出：禁用
 event.control.audio.input.enable = 音频输入：启用
 event.control.audio.input.disable = 音频输入：禁用
+event.control.calendar.add = 备忘录已添加到日历。
+event.control.calendar.clear = 日历中的备忘录已清除。
 event.control.camera.enable = 摄像头：启用
 event.control.camera.disable = 摄像头：禁用
 event.control.camera.capture = 摄像头：捕捉
 event.control.ctx.new = 上下文：新建
 event.control.ctx.prev = 上下文：上一个
 event.control.ctx.next = 上下文：下一个
 event.control.ctx.last = 上下文：最后一个
 event.control.ctx.input.focus = 输入：焦点
 event.control.ctx.input.send = 输入：发送
 event.control.ctx.input.clear = 输入：清除
 event.control.ctx.stop = 输入：停止
 event.control.ctx.attachments.clear = 附件：清除
+event.control.ctx.rename = 上下文重命名为{ctx}。
+event.control.ctx.search.string = 找到记录：{num}。
+event.control.ctx.search.clear = 搜索字符串已清除。
 event.control.input.sent = 输入已发送。
 event.control.input.stopped = 输入已停止。
 event.control.mode.chat = 模式：聊天
 event.control.mode.llama_index = 模式：带文件的聊天
 event.control.note.add = 笔记已添加到记事本。
+event.control.notepad.clear = 记事本已清除。
 event.control.tab.chat = 标签：聊天
 event.control.tab.calendar = 标签：日历
 event.control.tab.draw = 标签：绘图
 event.control.tab.files = 标签：文件
 event.control.tab.notepad = 标签：记事本
 event.control.tab.next = 标签：下一个
 event.control.tab.prev = 标签：上一个
```

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.agent.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.agent.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.agent.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_input.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_input.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_input.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_output.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.audio_output.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.audio_output.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_api.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_api.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_code_interpreter.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_custom.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_files.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_files.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_history.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_history.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_serial.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_serial.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_web.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.cmd_web.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.crontab.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.crontab.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.crontab.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.idx_llama_index.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.idx_llama_index.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_vision.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.openai_vision.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.en.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.real_time.en.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/locale/plugin.real_time.pl.ini` & `pygpt_net-2.2.9/src/pygpt_net/data/locale/plugin.real_time.pl.ini`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/logo.png` & `pygpt_net-2.2.9/src/pygpt_net/data/logo.png`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/prompts.csv` & `pygpt_net-2.2.9/src/pygpt_net/data/prompts.csv`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/win32/README.rtf` & `pygpt_net-2.2.9/src/pygpt_net/data/win32/README.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/win32/USER-LICENSE.rtf` & `pygpt_net-2.2.9/src/pygpt_net/data/win32/USER-LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/data/win32/pygpt.aip` & `pygpt_net-2.2.9/src/pygpt_net/data/win32/pygpt.aip`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/icons.qrc` & `pygpt_net-2.2.9/src/pygpt_net/icons.qrc`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/icons_rc.py` & `pygpt_net-2.2.9/src/pygpt_net/icons_rc.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/assistant.py` & `pygpt_net-2.2.9/src/pygpt_net/item/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/attachment.py` & `pygpt_net-2.2.9/src/pygpt_net/item/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/calendar_note.py` & `pygpt_net-2.2.9/src/pygpt_net/item/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/ctx.py` & `pygpt_net-2.2.9/src/pygpt_net/item/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/index.py` & `pygpt_net-2.2.9/src/pygpt_net/item/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/mode.py` & `pygpt_net-2.2.9/src/pygpt_net/item/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/model.py` & `pygpt_net-2.2.9/src/pygpt_net/item/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/notepad.py` & `pygpt_net-2.2.9/src/pygpt_net/item/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/item/preset.py` & `pygpt_net-2.2.9/src/pygpt_net/item/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/launcher.py` & `pygpt_net-2.2.9/src/pygpt_net/launcher.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231227152900.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231227152900.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231230095000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231230095000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20231231230000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20231231230000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240106060000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240106060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240107060000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240107060000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240222160000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240222160000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240223050000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240223050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240303190000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240303190000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240408180000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240408180000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240426050000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240426050000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/Version20240501030000.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/Version20240501030000.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/migrations/base.py` & `pygpt_net-2.2.9/src/pygpt_net/migrations/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/agent/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/simple.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_input/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/audio_input/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/audio_output/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/audio_output/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/audio_output/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/base.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_api/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_api/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/runner.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/runner.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_code_interpreter/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_code_interpreter/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_custom/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_custom/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_custom/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_files/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_files/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_files/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_history/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_history/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_history/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_serial/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_serial/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_serial/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/websearch.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/websearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/cmd_web/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/cmd_web/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/crontab/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/crontab/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/experts/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/experts/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/extra_prompt/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/extra_prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/idx_llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/idx_llama_index/worker.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/idx_llama_index/worker.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/openai_dalle/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/openai_dalle/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/openai_vision/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/openai_vision/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/plugin/real_time/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/plugin/real_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/bing_speech_recognition.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/bing_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/google_cloud_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/google_speech_recognition.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/google_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/openai_whisper.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_input/openai_whisper_local.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_input/openai_whisper_local.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/eleven_labs.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/google_tts.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/google_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/ms_azure_tts.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/ms_azure_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/audio_output/openai_tts.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/audio_output/openai_tts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_file/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/assistant_store/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/assistant_store/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/attachment/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/attachment/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/attachment/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/calendar/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/config/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/config/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/config/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/config/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/ctx/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/ctx/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/history/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/history/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/history/txt_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/history/txt_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/db_sqlite/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/db_sqlite/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/index/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/index/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/mode/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/mode/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/model/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/model/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/model/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/model/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/db_sqlite/storage.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/notepad/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/notepad/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/plugin_preset/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/plugin_preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/json_file.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/json_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/core/preset/patch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/core/preset/patch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/assistants.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/chat.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/chat.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/completion.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/completion.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/image.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/store.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/summarizer.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/summarizer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/vision.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/assistants.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/worker/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/gpt/worker/importer.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/gpt/worker/importer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/anthropic.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/azure_openai.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/hugging_face.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/hugging_face.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/llama.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/llama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/ollama.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/ollama.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/llms/openai.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/llms/openai.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_csv.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_csv.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_docx.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_docx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_epub.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_epub.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_excel.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_excel.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_html.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_html.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_image_vision.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_image_vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_ipynb.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_ipynb.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_json.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_json.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_markdown.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_pdf.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_pdf.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_video_audio.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_video_audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/file_xml.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/file_xml.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/bitbucket/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/chatgpt_retrieval/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/database/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/database/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/issues.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/github/issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/github/repo.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/github/repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/calendar.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/docs.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/gmail.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/keep.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/google/sheets.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/google/sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/image_vision/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/image_vision/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/json/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/json/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/pandas_excel/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/simple_csv/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/simple_csv/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/video_audio/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/video_audio/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/web_page/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/web_page/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/yt/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/hub/yt/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/hub/yt/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_bitbucket.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_bitbucket.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_chatgpt_retrieval.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_database.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_database.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_issues.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_github_issues.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_github_repo.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_github_repo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_calendar.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_docs.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_docs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_drive.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_drive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_gmail.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_gmail.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_keep.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_keep.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_google_sheets.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_microsoft_onedrive.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_page.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_page.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_rss.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_rss.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_sitemap.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_sitemap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_twitter.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_twitter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/loaders/web_yt.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/loaders/web_yt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/chroma.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/elasticsearch.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/pinecode.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/pinecode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/redis.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/simple.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/vector_stores/temp.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/vector_stores/temp.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/web/base.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/web/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/web/google_custom_search.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/web/google_custom_search.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/provider/web/microsoft_bing.py` & `pygpt_net-2.2.9/src/pygpt_net/provider/web/microsoft_bing.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/audio_transcriber/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/audio_transcriber/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/base.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/code_interpreter/ui/widgets.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/code_interpreter/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/image_viewer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/image_viewer/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/image_viewer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/browse.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/browse.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/ctx.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/ctx.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/files.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/files.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/web.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/indexer/ui/widgets.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/indexer/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/media_player/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/media_player/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/media_player/ui/widgets.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/media_player/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/tools/text_editor/ui/widgets.py` & `pygpt_net-2.2.9/src/pygpt_net/tools/text_editor/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/base/config_dialog.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/base/config_dialog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/base/context_menu.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/base/context_menu.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/about.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/applog.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/assistant_store.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/changelog.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/changelog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/create.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/db.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/debug.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/dictionary.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/find.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/image.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/license.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/logger.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/models.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/models.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/preset_plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/profile.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/rename.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/snap.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/start.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/start.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/update.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialog/workdir.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/dialogs.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/attachments.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/attachments_uploaded.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/attachments_uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/calendar.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/calendar.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/markdown.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/markdown.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/output.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/chat/painter.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/chat/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/ctx_list.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/ctx_list.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/search_input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/ctx/video.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/ctx/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/status.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/status.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/agent.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/agent.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/assistants.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/assistants.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/footer.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/footer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/image.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/indexes.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/indexes.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/mode.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/model.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/presets.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/presets.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/prompt.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/layout/toolbox/vision.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/layout/toolbox/vision.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/main.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/main.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/__init__.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/about.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/about.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/audio.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/config.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/config.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/debug.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/file.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/lang.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/lang.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/theme.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/theme.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/tools.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/tools.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/menu/video.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/menu/video.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/tray.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/tray.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/input_button.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/input_button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/audio/output.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/audio/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/calendar/select.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/calendar/select.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/alert.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/alert.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/applog.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/applog.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/assistant_store.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/audio.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/audio.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/base.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/confirm.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/confirm.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/create.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/db.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/debug.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/editor_file.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/editor_file.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/find.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/image.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/image.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/info.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/info.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/license.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/license.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/logger.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/logger.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/model.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/preset_plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/profile.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/rename.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/settings_plugin.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/settings_plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/snap.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/snap.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/update.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/update.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/dialog/workdir.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/dialog/workdir.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/draw/painter.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/draw/painter.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/button.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/button.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/checkbox.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/group.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/group.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/element/labels.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/element/labels.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/filesystem/explorer.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/filesystem/explorer.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/image/display.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/image/display.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/assistant.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/assistant_store.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/assistant_store.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/attachment.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/attachment.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/base.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/base.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/context.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/context.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/db.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/db.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/debug.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/debug.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/experts.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/experts.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/index.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/index_combo.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/index_combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/mode.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/mode.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/model.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/model_editor.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/model_editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/plugin.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/plugin.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/preset.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/preset_plugins.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/profile.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/profile.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/settings.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/settings.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/lists/uploaded.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/lists/uploaded.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/checkbox.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/checkbox.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/cmd.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/cmd.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/combo.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/combo.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/dictionary.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/dictionary.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/prompt.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/prompt.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/slider.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/slider.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/option/textarea.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/option/textarea.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/Input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/tabs/Input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/tabs/output.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/tabs/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/calendar_note.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/calendar_note.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/create.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/create.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/editor.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/editor.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/find.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/find.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/name.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/name.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/notepad.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/notepad.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/output.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/output.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/rename.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/rename.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/search_input.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/search_input.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/textarea/web.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/textarea/web.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/ui/widget/vision/camera.py` & `pygpt_net-2.2.9/src/pygpt_net/ui/widget/vision/camera.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/src/pygpt_net/utils.py` & `pygpt_net-2.2.9/src/pygpt_net/utils.py`

 * *Files identical despite different names*

### Comparing `pygpt_net-2.2.8/PKG-INFO` & `pygpt_net-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygpt-net
-Version: 2.2.8
+Version: 2.2.9
 Summary: Desktop AI Assistant powered by GPT-4, GPT-4V, GPT-3.5, DALL-E 3, Langchain LLMs, Llama-index, Whisper with chatbot, assistant, text completion, vision and image generation, internet access, chat with files, commands and code execution, file upload and download and more
 Home-page: https://github.com/szczyglis-dev/py-gpt
 License: MIT
 Keywords: py_gpt,py-gpt,pygpt,desktop,app,gpt,gpt4,gpt4-v,gpt3.5,gpt-4,gpt-4V,gpt-3.5,tts,whisper,vision,chatgpt,dall-e,chat,chatbot,assistant,text completion,image generation,ai,api,openai,api key,langchain,llama-index,presets,ui,qt,pyside
 Author: Marcin Szczyglinski
 Author-email: info@pygpt.net
 Requires-Python: >=3.10,<3.12
@@ -70,15 +70,15 @@
 Project-URL: Repository, https://github.com/szczyglis-dev/py-gpt
 Description-Content-Type: text/markdown
 
 # PyGPT - Desktop AI Assistant
 
 [![pygpt](https://snapcraft.io/pygpt/badge.svg)](https://snapcraft.io/pygpt)
 
-Release: **2.2.8** | build: **2024.05.02** | Python: **>=3.10, <3.12**
+Release: **2.2.9** | build: **2024.05.02** | Python: **>=3.10, <3.12**
 
 Official website: https://pygpt.net | Documentation: https://pygpt.readthedocs.io
 
 Snap Store: https://snapcraft.io/pygpt | PyPi: https://pypi.org/project/pygpt-net
 
 Compiled version for Linux (`tar.gz`) and Windows 10/11 (`msi`) 64-bit: https://pygpt.net/#download
 
@@ -970,14 +970,17 @@
 
 - Get the current application status
 - Exit the application
 - Enable audio output
 - Disable audio output
 - Enable audio input
 - Disable audio input
+- Add a memo to the calendar
+- Clear memos from calendar
+- Read the calendar memos
 - Enable the camera
 - Disable the camera
 - Capture the camera
 - Create a new context
 - Go to the previous context
 - Go to the next context
 - Go to the last context
@@ -985,19 +988,23 @@
 - Send the input
 - Clear the input
 - Get current conversation info
 - Stop executing current action
 - Clear the attachments
 - Read the last conversation entry
 - Read the whole conversation
+- Rename current context
+- Search for a string in the conversation
+- Clear the search results
 - Send the message to input
 - Append message to current input without sending it
 - Switch to chat mode
 - Switch to Chat with files (llama-index) mode
 - Add note to notepad
+- Clear notepad contents
 - Read current notepad contents
 - Switch to the chat tab
 - Switch to the calendar tab
 - Switch to the draw (painter) tab
 - Switch to the files tab
 - Switch to the notepad tab
 - Switch to the next tab
@@ -3266,14 +3273,18 @@
 
 ---
 
 # CHANGELOG
 
 ## Recent changes:
 
+**2.2.9 (2024-05-02)**
+
+- Added more commands to voice control: search for contexts, clear search, add, read and clear calendar memos, context rename.
+
 **2.2.8 (2024-05-02)**
 
 - Added support for disabled people, including voice control and screen event translation with audio synthesis.
 - A new section in Settings called 'Accessibility' has been added with options for assistance: voice control, keyboard shortcut definitions for actions, and screen event translation using audio synthesis.
 - A new section called 'Accessibility' has been added to the Documentation.
 
 **2.2.7 (2024-05-01)**
```

