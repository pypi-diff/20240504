# Comparing `tmp/unmanic-0.2.6.tar.gz` & `tmp/unmanic-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unmanic-0.2.6.tar", last modified: Tue Mar 12 19:47:26 2024, max compression
+gzip compressed data, was "unmanic-0.2.7.tar", last modified: Sat May  4 03:59:43 2024, max compression
```

## Comparing `unmanic-0.2.6.tar` & `unmanic-0.2.7.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.850765 unmanic-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 19:46:25.000000 unmanic-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-12 19:46:25.000000 unmanic-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43806 2024-03-12 19:47:26.850765 unmanic-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-03-12 19:46:25.000000 unmanic-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    27920 2024-03-12 19:46:25.000000 unmanic-0.2.6/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-12 19:46:25.000000 unmanic-0.2.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-12 19:46:25.000000 unmanic-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-12 19:47:26.850765 unmanic-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-03-12 19:46:25.000000 unmanic-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.810765 unmanic-0.2.6/unmanic/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15537 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.814765 unmanic-0.2.6/unmanic/libs/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/db_migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/directoryinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/eventmonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/fileinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/filetest.py
--rw-r--r--   0 runner    (1001) docker     (127)    37626 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/foreman.py
--rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    76109 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/installation_link.py
--rw-r--r--   0 runner    (1001) docker     (127)    20594 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/library.py
--rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/libraryscanner.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)    32972 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21766 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/taskqueue.py
--rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/uiserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.814765 unmanic-0.2.6/unmanic/libs/unffmpeg/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codec_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.818765 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/aac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/ac3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/base_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/base_containers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.818765 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/avi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/flv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/matroska.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mov.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mp4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mpegts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/ogv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/psp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/containers/vob.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.818765 unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/ffprobe.py
--rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/hardware_acceleration_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.818765 unmanic-0.2.6/unmanic/libs/unffmpeg/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/lib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/lib/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.818765 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/ass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/srt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/video_codec_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/h264.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/hevc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unlogger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unmodels/
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/completedtasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/completedtaskscommandlogs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/enabledplugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/installation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unmodels/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/lib/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/librarypluginflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/pluginrepos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/workergroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unmodels/workerschedules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unplugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.822765 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/library_management/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/library_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/library_management/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/plugin_type_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/worker/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/worker/process_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/pluginscli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/unplugins/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/worker_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/libs/workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/migrations_v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/migrations_v1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    11420 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/service.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/version
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/webserver/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_request_router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.826765 unmanic-0.2.6/unmanic/webserver/api_v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/base_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/filebrowser_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/history_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/pending_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/plugins_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v1/session_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.830765 unmanic-0.2.6/unmanic/webserver/api_v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/base_api_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/docs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/filebrowser_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/history_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/notifications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30798 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/pending_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46051 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/plugins_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.830765 unmanic-0.2.6/unmanic/webserver/api_v2/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43658 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/schema/schemas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/schema/unmanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/session_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    50039 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/upload_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/version_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/api_v2/workers_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.830765 unmanic-0.2.6/unmanic/webserver/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   261856 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/docs/api_schema_v2.json
--rw-r--r--   0 runner    (1001) docker     (127)   132047 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/docs/api_schema_v2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/docs/privacy_policy.md
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/.eslintrc.js
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/babel.config.js
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/jsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   447807 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/postcss.config.cjs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/public/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/public/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/public/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-128x128.png
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/quasar.conf.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      712 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/scripts/translate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/src/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/App.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.834765 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   228094 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/bg-md1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    37547 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/coffee-btn-image.png
--rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/logo-lg.png
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)    37204 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.838765 unmanic-0.2.6/unmanic/webserver/frontend/src/boot/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/boot/axios.js
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/boot/global-event-bus.js
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/boot/i18n.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.842765 unmanic-0.2.6/unmanic/webserver/frontend/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTasks.vue
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerAvatar.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerMainNav.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerNotifications.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/EssentialLink.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/FooterData.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/LanguageSwitch.vue
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/LoginDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/MarkdownDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/PendingTasks.vue
--rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/PendingTasksTable.vue
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/ThemeSwitch.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgress.vue
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.842765 unmanic-0.2.6/unmanic/webserver/frontend/src/components/dialogs/
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue
--rw-r--r--   0 runner    (1001) docker     (127)    23291 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.842765 unmanic-0.2.6/unmanic/webserver/frontend/src/components/forms/
--rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/components/iframe-directive.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.842765 unmanic-0.2.6/unmanic/webserver/frontend/src/css/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/css/app.scss
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/css/markdown-admonitions.css
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/css/quasar.variables.scss
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/index.template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.842765 unmanic-0.2.6/unmanic/webserver/frontend/src/js/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/js/dateTools.js
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/js/markupParser.js
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/js/unmanicGlobals.js
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/js/unmanicWebsocket.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.846765 unmanic-0.2.6/unmanic/webserver/frontend/src/language/
--rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/de.json
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/en.json
--rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/es.json
--rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/fr.json
--rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/it.json
--rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/ja.json
--rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/mi.json
--rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/nl.json
--rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/pl.json
--rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/pt-br.json
--rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/ru.json
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/sv.json
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/language/zh.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.846765 unmanic-0.2.6/unmanic/webserver/frontend/src/layouts/
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/layouts/MainLayout.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.846765 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/ActionTrigger.vue
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/DataPanels.vue
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/ErrorNotFound.vue
--rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/MainDashboard.vue
--rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue
--rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsLink.vue
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue
--rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsSupport.vue
--rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.846765 unmanic-0.2.6/unmanic/webserver/frontend/src/router/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/router/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-12 19:46:26.000000 unmanic-0.2.6/unmanic/webserver/frontend/src/router/routes.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.850765 unmanic-0.2.6/unmanic/webserver/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/completed_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/pending_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/helpers/workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.806765 unmanic-0.2.6/unmanic/webserver/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.850765 unmanic-0.2.6/unmanic/webserver/templates/global/
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/templates/global/insufficient-permissions.html
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/templates/global/login-popup.html
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/templates/global/support-future-development.html
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-03-12 19:46:25.000000 unmanic-0.2.6/unmanic/webserver/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:47:26.850765 unmanic-0.2.6/unmanic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43806 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:46:54.000000 unmanic-0.2.6/unmanic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-12 19:47:26.000000 unmanic-0.2.6/unmanic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-03-12 19:46:25.000000 unmanic-0.2.6/versioninfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.095912 unmanic-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 03:58:41.000000 unmanic-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-04 03:58:41.000000 unmanic-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    43806 2024-05-04 03:59:43.095912 unmanic-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-05-04 03:58:41.000000 unmanic-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27920 2024-05-04 03:58:41.000000 unmanic-0.2.7/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 03:58:41.000000 unmanic-0.2.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-04 03:58:41.000000 unmanic-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-04 03:59:43.095912 unmanic-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-04 03:58:41.000000 unmanic-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.051912 unmanic-0.2.7/unmanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15537 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.055912 unmanic-0.2.7/unmanic/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10398 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/db_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/directoryinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/eventmonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/fileinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/filetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37626 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/foreman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10702 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76109 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/installation_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20594 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/library.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14360 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/libraryscanner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32972 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21999 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9228 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24375 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9865 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/taskqueue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15034 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/uiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.059912 unmanic-0.2.7/unmanic/libs/unffmpeg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codec_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.059912 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/aac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/ac3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/base_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/base_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.059912 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/avi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/flv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/matroska.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mp4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mpegts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/ogv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/psp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/containers/vob.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.059912 unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/ffprobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/hardware_acceleration_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.059912 unmanic-0.2.7/unmanic/libs/unffmpeg/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/lib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/lib/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.063912 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/ass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/srt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/video_codec_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.063912 unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/h264.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/hevc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unlogger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.063912 unmanic-0.2.7/unmanic/libs/unmodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/completedtasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/completedtaskscommandlogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/enabledplugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/installation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.063912 unmanic-0.2.7/unmanic/libs/unmodels/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/lib/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/librarypluginflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/pluginrepos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/workergroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unmodels/workerschedules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18496 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/library_management/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/library_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/library_management/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/plugin_type_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/worker/process_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/pluginscli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/unplugins/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/worker_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/libs/workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/migrations_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/migrations_v1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11312 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.067912 unmanic-0.2.7/unmanic/webserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_request_router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.071912 unmanic-0.2.7/unmanic/webserver/api_v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/base_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/filebrowser_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/pending_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8936 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/plugins_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v1/session_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.071912 unmanic-0.2.7/unmanic/webserver/api_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10995 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/base_api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7098 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/docs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/filebrowser_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/notifications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30798 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/pending_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46051 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/plugins_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.071912 unmanic-0.2.7/unmanic/webserver/api_v2/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43658 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/schema/schemas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/schema/unmanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/session_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50039 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/version_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/api_v2/workers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.075912 unmanic-0.2.7/unmanic/webserver/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   261856 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/docs/api_schema_v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132047 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/docs/api_schema_v2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/docs/privacy_policy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.075912 unmanic-0.2.7/unmanic/webserver/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/.eslintrc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1474 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/babel.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/jsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   447807 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/postcss.config.cjs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.075912 unmanic-0.2.7/unmanic/webserver/frontend/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/public/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.075912 unmanic-0.2.7/unmanic/webserver/frontend/public/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-128x128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/quasar.conf.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.079912 unmanic-0.2.7/unmanic/webserver/frontend/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      712 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/scripts/translate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.079912 unmanic-0.2.7/unmanic/webserver/frontend/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/App.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.079912 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   228094 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/bg-md1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    37547 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/coffee-btn-image.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/logo-lg.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    37204 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.079912 unmanic-0.2.7/unmanic/webserver/frontend/src/boot/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/boot/axios.js
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/boot/global-event-bus.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/boot/i18n.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.083912 unmanic-0.2.7/unmanic/webserver/frontend/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTasks.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerAvatar.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerMainNav.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerNotifications.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/EssentialLink.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/FooterData.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/LanguageSwitch.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/LoginDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/MarkdownDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/PendingTasks.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    10486 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/PendingTasksTable.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/ThemeSwitch.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgress.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.083912 unmanic-0.2.7/unmanic/webserver/frontend/src/components/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    23291 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.087912 unmanic-0.2.7/unmanic/webserver/frontend/src/components/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    14055 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/components/iframe-directive.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.087912 unmanic-0.2.7/unmanic/webserver/frontend/src/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/css/app.scss
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/css/markdown-admonitions.css
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/css/quasar.variables.scss
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/index.template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.087912 unmanic-0.2.7/unmanic/webserver/frontend/src/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/js/dateTools.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/js/markupParser.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/js/unmanicGlobals.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/js/unmanicWebsocket.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.087912 unmanic-0.2.7/unmanic/webserver/frontend/src/language/
+-rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/de.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/es.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/fr.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/it.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20757 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/ja.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17402 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/mi.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17763 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/nl.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/pl.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17991 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/pt-br.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25420 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/ru.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/sv.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/language/zh.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.087912 unmanic-0.2.7/unmanic/webserver/frontend/src/layouts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/layouts/MainLayout.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.091912 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/ActionTrigger.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/DataPanels.vue
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/ErrorNotFound.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    16115 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/MainDashboard.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsLink.vue
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    18251 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsSupport.vue
+-rw-r--r--   0 runner    (1001) docker     (127)    12153 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.091912 unmanic-0.2.7/unmanic/webserver/frontend/src/router/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/router/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-04 03:58:42.000000 unmanic-0.2.7/unmanic/webserver/frontend/src/router/routes.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.091912 unmanic-0.2.7/unmanic/webserver/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/completed_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/pending_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18233 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/helpers/workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.047912 unmanic-0.2.7/unmanic/webserver/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.091912 unmanic-0.2.7/unmanic/webserver/templates/global/
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/templates/global/insufficient-permissions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/templates/global/login-popup.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/templates/global/support-future-development.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-04 03:58:41.000000 unmanic-0.2.7/unmanic/webserver/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 03:59:43.091912 unmanic-0.2.7/unmanic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43806 2024-05-04 03:59:42.000000 unmanic-0.2.7/unmanic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11499 2024-05-04 03:59:43.000000 unmanic-0.2.7/unmanic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:59:42.000000 unmanic-0.2.7/unmanic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-04 03:59:42.000000 unmanic-0.2.7/unmanic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 03:59:10.000000 unmanic-0.2.7/unmanic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-04 03:59:42.000000 unmanic-0.2.7/unmanic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 03:59:42.000000 unmanic-0.2.7/unmanic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-04 03:58:41.000000 unmanic-0.2.7/versioninfo.py
```

### Comparing `unmanic-0.2.6/LICENSE` & `unmanic-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/MANIFEST.in` & `unmanic-0.2.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/PKG-INFO` & `unmanic-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmanic
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple tool for optimising your video library to a single format
 Home-page: https://github.com/Josh5/unmanic
 Author: Josh.5
 Author-email: jsunnex@gmail.com
 Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com
 License: GPLv3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unmanic Version: 0.2.6 Summary: A simple tool for
+Metadata-Version: 2.1 Name: unmanic Version: 0.2.7 Summary: A simple tool for
 optimising your video library to a single format Home-page: https://github.com/
 Josh5/unmanic Author: Josh.5 Author-email: jsunnex@gmail.com Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com License: GPLv3 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `unmanic-0.2.6/README.md` & `unmanic-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/logo.png` & `unmanic-0.2.7/logo.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/setup.py` & `unmanic-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/__init__.py` & `unmanic-0.2.7/unmanic/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/__main__.py` & `unmanic-0.2.7/unmanic/__main__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/config.py` & `unmanic-0.2.7/unmanic/config.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/__init__.py` & `unmanic-0.2.7/unmanic/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/common.py` & `unmanic-0.2.7/unmanic/libs/common.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/db_migrate.py` & `unmanic-0.2.7/unmanic/libs/db_migrate.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/directoryinfo.py` & `unmanic-0.2.7/unmanic/libs/directoryinfo.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/eventmonitor.py` & `unmanic-0.2.7/unmanic/libs/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/fileinfo.py` & `unmanic-0.2.7/unmanic/libs/fileinfo.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/filetest.py` & `unmanic-0.2.7/unmanic/libs/filetest.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/foreman.py` & `unmanic-0.2.7/unmanic/libs/foreman.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/history.py` & `unmanic-0.2.7/unmanic/libs/history.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/installation_link.py` & `unmanic-0.2.7/unmanic/libs/installation_link.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/library.py` & `unmanic-0.2.7/unmanic/libs/library.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/libraryscanner.py` & `unmanic-0.2.7/unmanic/libs/libraryscanner.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/notifications.py` & `unmanic-0.2.7/unmanic/libs/notifications.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/plugins.py` & `unmanic-0.2.7/unmanic/libs/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/postprocessor.py` & `unmanic-0.2.7/unmanic/libs/postprocessor.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/scheduler.py` & `unmanic-0.2.7/unmanic/libs/scheduler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/session.py` & `unmanic-0.2.7/unmanic/libs/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,42 @@
            IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
            DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
            OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
            OR OTHER DEALINGS IN THE SOFTWARE.
 
 """
 import base64
+import datetime
 import pickle
 import random
 import time
+
 import requests
 
 from unmanic import config
 from unmanic.libs import common, unlogger
 from unmanic.libs.singleton import SingletonType
 from unmanic.libs.unmodels import Installation
 
 
+class RemoteApiException(Exception):
+    """
+    RemoteApiException
+    Custom exception for errors contacting the remote Unmanic API
+    """
+
+    def __init__(self, message, status_code):
+        super().__init__(f"Session Error - Remote API [CODE: {status_code}]: {message}")
+
+
 class Session(object, metaclass=SingletonType):
     """
     Session
 
-    Manages the Unbmanic applications session for unlocking
+    Manages the Unmanic applications session for unlocking
     features and fetching data from the Unmanic site API.
 
     """
 
     """
     level - The user auth level
     Set level to 0 by default
@@ -98,23 +110,28 @@
 
     """
     user_access_token - The access token to authenticate requests with the Unmanic API
     """
     user_access_token = None
 
     """
+    user_refresh_token - The refresh token for acquiring an updated access token
+    """
+    user_refresh_token = None
+
+    """
     session_cookies - A stored copy of the session cookies to persist between restarts
     """
     session_cookies = None
 
     def __init__(self, *args, **kwargs):
         unmanic_logging = unlogger.UnmanicLogger.__call__()
         self.logger = unmanic_logging.get_logger(__class__.__name__)
         self.timeout = 30
-        self.dev_local_api = kwargs.get('dev_local_api', False)
+        self.dev_api = kwargs.get('dev_api', None)
         self.requests_session = requests.Session()
         self.logger.info('Initialising new session object')
 
     def __created_older_than_x_days(self, days=1):
         # (86400 = 24 hours)
         seconds = (days * 86400)
         # Get session expiration time
@@ -159,16 +176,15 @@
         seconds = time.time()
         # Create a seconds offset of some random number between 300 (5 mins) and 900 (15 mins)
         seconds_offset = random.randint(300, 900 - 1)
         # Set the created flag with the seconds variable plus a random offset to avoid people joining
         #   together to register if the site goes down
         self.created = (seconds + seconds_offset)
         # Print only the accurate update time in debug log
-        from datetime import datetime
-        created = datetime.fromtimestamp(seconds)
+        created = datetime.datetime.fromtimestamp(seconds)
         self.logger.debug('Updated session at %s', str(created))
 
     def __fetch_installation_data(self):
         """
         Fetch installation data from DB
 
         :return:
@@ -185,35 +201,39 @@
             current_installation = db_installation.create()
 
         self.uuid = str(current_installation.uuid)
         self.level = int(current_installation.level)
         self.picture_uri = str(current_installation.picture_uri)
         self.name = str(current_installation.name)
         self.email = str(current_installation.email)
-        self.created = current_installation.created
+        self.created = current_installation.created if current_installation.created else None
+        if isinstance(self.created, datetime.datetime):
+            self.created = self.created.timestamp()
 
         self.__update_session_auth(access_token=current_installation.user_access_token,
                                    session_cookies=current_installation.session_cookies)
 
-    def __store_installation_data(self):
+    def __store_installation_data(self, force_save_access_token=False):
         """
         Store installation data in DB to persist reboot
 
         :return:
         """
         if self.uuid:
             db_installation = Installation.get_or_none(uuid=self.uuid)
             db_installation.level = self.level
             db_installation.picture_uri = self.picture_uri
             db_installation.name = self.name
             db_installation.email = self.email
             db_installation.created = self.created
-            if self.user_access_token:
+            if self.user_access_token or force_save_access_token:
                 db_installation.user_access_token = self.user_access_token
-            if self.session_cookies:
+            if self.user_refresh_token or force_save_access_token:
+                db_installation.user_refresh_token = self.user_refresh_token
+            if self.session_cookies or force_save_access_token:
                 db_installation.session_cookies = self.session_cookies
             db_installation.save()
 
     def __reset_session_installation_data(self):
         """
         Reset stored session data
 
@@ -222,29 +242,35 @@
         self.logger.debug('Resetting session installation data.')
         self.level = 0
         self.picture_uri = ''
         self.name = ''
         self.email = ''
         self.created = time.time()
         self.user_access_token = None
-        self.__store_installation_data()
+        self.user_refresh_token = None
+        self.__store_installation_data(force_save_access_token=True)
+        self.__clear_session_auth()
 
     def __update_session_auth(self, access_token=None, session_cookies=None):
         # Update session headers
         if access_token:
             self.user_access_token = access_token
             self.requests_session.headers.update({'Authorization': self.user_access_token})
         # Update session cookies
         if session_cookies:
             self.session_cookies = session_cookies
             try:
                 self.requests_session.cookies = pickle.loads(base64.b64decode(session_cookies))
             except Exception as e:
                 self.logger.error('Error trying to reload session cookies - %s', str(e))
 
+    def __clear_session_auth(self):
+        self.requests_session.cookies.clear()
+        self.requests_session.headers.update({'Authorization': ''})
+
     def get_installation_uuid(self):
         """
         Returns the installation UUID as a string.
         If it does not yet exist, it will create one.
 
         :return:
         """
@@ -265,17 +291,16 @@
     def get_site_url(self):
         """
         Set the Unmanic application site URL
         :return:
         """
         api_proto = "https"
         api_domain = "api.unmanic.app"
-        if self.dev_local_api:
-            api_proto = "http"
-            api_domain = "api.unmanic.localhost"
+        if self.dev_api:
+            return self.dev_api
         return "{0}://{1}".format(api_proto, api_domain)
 
     def set_full_api_url(self, api_prefix, api_version, api_path):
         """
         Set the API path URL
 
         :param api_prefix:
@@ -295,28 +320,25 @@
         :param api_path:
         :return:
         """
         u = self.set_full_api_url(api_prefix, api_version, api_path)
         r = self.requests_session.get(u, timeout=self.timeout)
         if r.status_code > 403:
             # There is an issue with the remote API
-            self.logger.debug(
-                "Sorry! There seems to be an issue with the remote servers. Please try GET request again later. Status code %s",
-                r.status_code)
+            raise RemoteApiException(f"GET request failed for {u}", r.status_code)
         if r.status_code == 401:
             # Verify the token. Refresh as required
+            self.logger.debug("Auto exec token verification (api_get)")
             token_verified = self.verify_token()
             # If successful, then retry request
             if token_verified:
                 r = self.requests_session.get(u, timeout=self.timeout)
                 if r.status_code > 403:
                     # There is an issue with the remote API
-                    self.logger.debug(
-                        "Sorry! There seems to be an issue with the remote servers on retry. Please try GET request again later. Status code %s",
-                        r.status_code)
+                    raise RemoteApiException(f"GET request still failed for {u}", r.status_code)
             else:
                 self.logger.debug('Failed to verify auth (api_get)')
         return r.json(), r.status_code
 
     def api_post(self, api_prefix, api_version, api_path, data):
         """
         Generate and execute a POST API call.
@@ -327,28 +349,25 @@
         :param data:
         :return:
         """
         u = self.set_full_api_url(api_prefix, api_version, api_path)
         r = self.requests_session.post(u, json=data, timeout=self.timeout)
         if r.status_code > 403:
             # There is an issue with the remote API
-            self.logger.debug(
-                "Sorry! There seems to be an issue with the remote servers. Please try POST request again later. Status code %s",
-                r.status_code)
+            raise RemoteApiException(f"POST request failed for {u}", r.status_code)
         if r.status_code == 401:
             # Verify the token. Refresh as required
+            self.logger.debug("Auto exec token verification (api_post)")
             token_verified = self.verify_token()
             # If successful, then retry request
             if token_verified:
                 r = self.requests_session.post(u, json=data, timeout=self.timeout)
                 if r.status_code > 403:
                     # There is an issue with the remote API
-                    self.logger.debug(
-                        "Sorry! There seems to be an issue with the remote servers on retry. Please try POST request again later. Status code %s",
-                        r.status_code)
+                    raise RemoteApiException(f"POST request still failed for {u}", r.status_code)
             else:
                 self.logger.debug('Failed to verify auth (api_post)')
         return r.json(), r.status_code
 
     def verify_token(self):
         if not self.user_access_token:
             # No valid tokens exist
@@ -357,90 +376,118 @@
         u = self.set_full_api_url('support-auth-api', 1, 'user_auth/verify_token')
         r = self.requests_session.get(u, timeout=self.timeout)
         if r.status_code in [202]:
             # Token is valid
             return True
         elif r.status_code > 403:
             # Issue with server... Just carry on with current access token can't fix that here.
-            self.logger.debug(
-                "Sorry! There seems to be an issue with the token auth servers. Please try again later. Status code %s",
-                r.status_code)
-            # Return True here to prevent the app from lowering the level
-            return True
+            raise RemoteApiException(f"Token verification request failed for {u}", r.status_code)
 
         # Access token is not valid. Refresh it.
         self.logger.debug('Unable to verify authentication token. Refreshing...')
-        u = self.set_full_api_url('support-auth-api', 1, 'user_auth/refresh_token')
-        r = self.requests_session.get(u, timeout=self.timeout)
+        d = {"refreshToken": self.user_refresh_token}
+        u = self.set_full_api_url('support-auth-api', 1, 'user_auth/token')
+        r = self.requests_session.post(u, json=d, timeout=self.timeout)
         if r.status_code in [202]:
             # Token refreshed
             # Store the updated access token
             response = r.json()
             self.__update_session_auth(access_token=response.get('data', {}).get('accessToken'))
+            # Store the updated refresh token
+            self.user_refresh_token = response.get('data', {}).get('refreshToken')
             # Store the updated session cookies
             self.session_cookies = base64.b64encode(pickle.dumps(self.requests_session.cookies)).decode('utf-8')
             self.__store_installation_data()
             return True
         elif r.status_code > 403:
             # Issue was with server... Just carry on with current access token can't fix that here.
-            self.logger.debug(
-                "Sorry! There seems to be an issue with the auth servers. Please try again later. Status code %s",
-                r.status_code)
-            # Return True here to prevent the app from lowering the level
-            return True
+            raise RemoteApiException(f"Token refresh request failed for {u}", r.status_code)
         elif r.status_code in [403]:
             # Log this failure in the debug logs
-            self.logger.debug('Failed to refresh access token.')
+            self.logger.info('Failed to refresh access token.')
             response = r.json()
             for message in response.get('messages', []):
-                self.logger.debug(message)
+                self.logger.info('Remote Message: %s', message)
         # Just blank the class attribute.
         # It is fine for requests to be sent with further requests.
         # User will appear to be logged out.
         self.user_access_token = None
         return False
 
+    def fetch_user_data(self):
+        # Set default level to 0
+        updated_level = 0
+        response, status_code = self.api_get('support-auth-api', 1, 'user_auth/user_info')
+        if status_code > 403:
+            # Failed to fetch data from server. Ignore this for now. Will try again later.
+            raise RemoteApiException("Failed to fetch user info from user_auth/user_info", status_code)
+        if status_code in [200, 201, 202] and response.get('success'):
+            # Get user data from response data
+            user_data = response.get('data', {}).get('user')
+            if user_data:
+                # Set name from user data
+                self.name = user_data.get("name", "Valued Supporter")
+                # Set avatar from user data
+                self.picture_uri = user_data.get("picture_uri", "/assets/global/img/avatar/avatar_placeholder.png")
+                # Set email from user data
+                self.email = user_data.get("email", "")
+                # Update level from response data (default back to 0)
+                updated_level = int(user_data.get("supporter_level", 0))
+        return updated_level
+
     def auth_user_account(self, force_checkin=False):
         # Don't bother if the user has never logged in
         if not self.user_access_token and not force_checkin:
             self.logger.debug('The user access token is not set add we are not being forced to refresh for one.')
-            return
+            return False
         # Start by verifying the token
         token_verified = self.verify_token()
         if not token_verified and force_checkin:
             # Try to fetch token if this was the initial login
             post_data = {"uuid": self.get_installation_uuid()}
             response, status_code = self.api_post('support-auth-api', 1, 'app_auth/retrieve_app_token', post_data)
             if status_code in [200, 201, 202] and response.get('success'):
+                # Store the updated access token
                 self.__update_session_auth(access_token=response.get('data', {}).get('accessToken'))
+                # Store the updated refresh token
+                self.user_refresh_token = response.get('data', {}).get('refreshToken')
                 token_verified = self.verify_token()
-        # Set default level to 0
-        updated_level = 0
+            elif status_code > 403:
+                raise RemoteApiException("Failed to fetch initial app token frp, app_auth/retrieve_app_token", status_code)
+            else:
+                self.logger.info('Failed to check in with Unmanic support auth API.')
+                for message in response.get('messages', []):
+                    self.logger.info('Remote Message: %s', message)
         # Finally, fetch user info if the token was successfully verified
         if token_verified:
-            response, status_code = self.api_get('support-auth-api', 1, 'user_auth/user_info')
-            if status_code >= 500:
-                # Failed to fetch data from server. Ignore this for now. Will try again later.
-                return
-            if status_code in [200, 201, 202] and response.get('success'):
-                # Get user data from response data
-                user_data = response.get('data', {}).get('user')
-                if user_data:
-                    # Set name from user data
-                    self.name = user_data.get("name", "Valued Supporter")
-
-                    # Set avatar from user data
-                    self.picture_uri = user_data.get("picture_uri", "/assets/global/img/avatar/avatar_placeholder.png")
-
-                    # Set email from user data
-                    self.email = user_data.get("email", "")
-
-                    # Update level from response data (default back to 0)
-                    updated_level = int(user_data.get("supporter_level", 0))
-        self.level = updated_level
+            self.level = self.fetch_user_data()
+            return True
+        else:
+            # Set default level to 0
+            self.level = 0
+        return False
+
+    def auth_trial_account(self):
+        # Check if access token is valid
+        d = {"uuid": self.get_installation_uuid()}
+        u = self.set_full_api_url('support-auth-api', 1, 'user_auth/trial_token')
+        r = self.requests_session.post(u, json=d, timeout=self.timeout)
+        if r.status_code in [202]:
+            # Token refreshed
+            # Store the updated access token
+            response = r.json()
+            self.__update_session_auth(access_token=response.get('data', {}).get('accessToken'))
+            # Fetch user data
+            self.level = self.fetch_user_data()
+            # Store the updated session cookies
+            self.__store_installation_data()
+            return True
+        elif r.status_code > 403:
+            # Issue with server... Just carry on with current access token can't fix that here.
+            raise RemoteApiException(f"Trial token verification request failed for {u}", r.status_code)
 
     def register_unmanic(self, force=False):
         """
         Register Unmanic with site.
         This sends information about the system that Unmanic is running on.
         It also sends a unique ID.
 
@@ -456,18 +503,18 @@
             return True
 
         # Set now as the last time this was run (before it was actually run
         self.last_check = time.time()
 
         # Update the session
         settings = config.Config()
-        try:
-            # Fetch the installation data prior to running a session update
-            self.__fetch_installation_data()
+        # Fetch the installation data prior to running a session update
+        self.__fetch_installation_data()
 
+        try:
             # Build post data
             from unmanic.libs.system import System
             system = System()
             system_info = system.info()
             platform_info = system_info.get("platform", None)
             if platform_info:
                 platform_info = " * ".join(platform_info)
@@ -478,31 +525,38 @@
                 "system":         {
                     "platform": platform_info,
                     "devices":  system_info.get("devices", {}),
                 }
             }
 
             # Refresh user auth
-            self.auth_user_account(force_checkin=force)
+            result = self.auth_user_account(force_checkin=force)
+            if not result:
+                # Fetch trial token
+                result = self.auth_trial_account()
 
             # Register Unmanic
             registration_response, status_code = self.api_post('unmanic-api', 1, 'installation_auth/register', post_data)
 
             # Save data
             if status_code in [200, 201, 202] and registration_response.get("success"):
                 self.__update_created_timestamp()
                 # Persist session in DB
                 self.__store_installation_data()
                 return True
+            elif status_code > 403:
+                raise RemoteApiException("Failed to register installation to installation_auth/register", status_code)
 
             # Allow an extension for the session for 7 days without an internet connection
             if self.__created_older_than_x_days(days=7):
                 # Reset the session - Unmanic should phone home once every 7 days
                 self.__reset_session_installation_data()
             return False
+        except RemoteApiException as e:
+            self.logger.error("Exception while registering Unmanic: %s", e)
         except Exception as e:
             self.logger.debug("Exception while registering Unmanic: %s", e, exc_info=True)
             if self.__check_session_valid():
                 # If the session is still valid, just return true. Perhaps the internet is down and it timed out?
                 return True
             return False
```

### Comparing `unmanic-0.2.6/unmanic/libs/singleton.py` & `unmanic-0.2.7/unmanic/libs/singleton.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/system.py` & `unmanic-0.2.7/unmanic/libs/system.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/task.py` & `unmanic-0.2.7/unmanic/libs/task.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/taskhandler.py` & `unmanic-0.2.7/unmanic/libs/taskhandler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/taskqueue.py` & `unmanic-0.2.7/unmanic/libs/taskqueue.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/uiserver.py` & `unmanic-0.2.7/unmanic/libs/uiserver.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codec_handle.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codec_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/aac.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/aac.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/ac3.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/ac3.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/audio_codecs/mp3.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/audio_codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/base_codecs.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/base_codecs.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/base_containers.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/base_containers.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/avi.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/avi.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/flv.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/flv.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/matroska.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/matroska.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mov.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mov.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mp4.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mp4.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mpeg.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mpeg.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/mpegts.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/mpegts.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/ogv.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/ogv.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/psp.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/psp.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/containers/vob.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/containers/vob.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/ffmpeg.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/exceptions/ffprobe.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/exceptions/ffprobe.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/hardware_acceleration_handle.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/hardware_acceleration_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/info.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/info.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/lib/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/lib/cli.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/lib/cli.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/lib/validation.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/lib/validation.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/ass.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/ass.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/mov_text.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/srt.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/srt.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/ssa.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/subrip.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_codecs/xsub.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/subtitle_handle.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/subtitle_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/video_codec_handle.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/video_codec_handle.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/__init__.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/h264.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/h264.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unffmpeg/video_codecs/hevc.py` & `unmanic-0.2.7/unmanic/libs/unffmpeg/video_codecs/hevc.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unlogger.py` & `unmanic-0.2.7/unmanic/libs/unlogger.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/__init__.py` & `unmanic-0.2.7/unmanic/libs/unmodels/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/completedtasks.py` & `unmanic-0.2.7/unmanic/libs/unmodels/completedtasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/completedtaskscommandlogs.py` & `unmanic-0.2.7/unmanic/libs/unmodels/completedtaskscommandlogs.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/enabledplugins.py` & `unmanic-0.2.7/unmanic/libs/unmodels/enabledplugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/installation.py` & `unmanic-0.2.7/unmanic/libs/unmodels/installation.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,9 @@
     picture_uri = TextField(null=True)
     name = TextField(null=True)
     email = TextField(null=True)
     created = DateTimeField(null=True, default=datetime.datetime.now)
 
     # Store session tokens
     user_access_token = TextField(null=True)
+    user_refresh_token = TextField(null=True)
     session_cookies = TextField(null=True)
```

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/lib/__init__.py` & `unmanic-0.2.7/unmanic/libs/unmodels/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/lib/basemodel.py` & `unmanic-0.2.7/unmanic/libs/unmodels/lib/basemodel.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/libraries.py` & `unmanic-0.2.7/unmanic/libs/unmodels/libraries.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/librarypluginflow.py` & `unmanic-0.2.7/unmanic/libs/unmodels/librarypluginflow.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/pluginrepos.py` & `unmanic-0.2.7/unmanic/libs/unmodels/pluginrepos.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/plugins.py` & `unmanic-0.2.7/unmanic/libs/unmodels/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/tags.py` & `unmanic-0.2.7/unmanic/libs/unmodels/tags.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/tasks.py` & `unmanic-0.2.7/unmanic/libs/unmodels/tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/workergroups.py` & `unmanic-0.2.7/unmanic/libs/unmodels/workergroups.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unmodels/workerschedules.py` & `unmanic-0.2.7/unmanic/libs/unmodels/workerschedules.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/executor.py` & `unmanic-0.2.7/unmanic/libs/unplugins/executor.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/panel.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/panel.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/frontend/plugin_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/library_management/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/library_management/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/library_management/file_test.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/library_management/file_test.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/plugin_type_base.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/plugin_type_base.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/file_move.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/postprocessor/task_result.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/worker/__init__.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/plugin_types/worker/process_item.py` & `unmanic-0.2.7/unmanic/libs/unplugins/plugin_types/worker/process_item.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/pluginscli.py` & `unmanic-0.2.7/unmanic/libs/unplugins/pluginscli.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/unplugins/settings.py` & `unmanic-0.2.7/unmanic/libs/unplugins/settings.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/worker_group.py` & `unmanic-0.2.7/unmanic/libs/worker_group.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/libs/workers.py` & `unmanic-0.2.7/unmanic/libs/workers.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/metadata.py` & `unmanic-0.2.7/unmanic/metadata.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py` & `unmanic-0.2.7/unmanic/migrations_v1/001_rename_ffmpeg_log_to_log.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/service.py` & `unmanic-0.2.7/unmanic/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def __init__(self):
         self.threads = []
         self.run_threads = True
         self.db_connection = None
 
         self.developer = None
-        self.dev_local_api = None
+        self.dev_api = None
 
         self.event = threading.Event()
 
     def start_handler(self, data_queues, task_queue):
         main_logger.info("Starting TaskHandler")
         handler = TaskHandler(data_queues, task_queue, self.event)
         handler.daemon = True
@@ -166,18 +166,17 @@
         scheduled_tasks_manager.start()
         self.threads.append({
             'name':   'ScheduledTasksManager',
             'thread': scheduled_tasks_manager
         })
         return scheduled_tasks_manager
 
-    @staticmethod
-    def initial_register_unmanic(dev_local_api):
+    def initial_register_unmanic(self):
         from unmanic.libs import session
-        s = session.Session(dev_local_api=dev_local_api)
+        s = session.Session(dev_api=self.dev_api)
         s.register_unmanic(s.get_installation_uuid())
 
     def start_threads(self, settings):
         # Create our data queues
         data_queues = {
             "library_scanner_triggers": queue.Queue(maxsize=1),
             "scheduledtasks":           queue.Queue(),
@@ -190,15 +189,15 @@
         # Clear cache directory
         main_logger.info("Clearing previous cache")
         common.clean_files_in_cache_dir(settings.get_cache_path())
 
         main_logger.info("Starting all threads")
 
         # Register installation
-        self.initial_register_unmanic(self.dev_local_api)
+        self.initial_register_unmanic()
 
         # Setup job queue
         task_queue = TaskQueue(data_queues)
 
         # Setup post-processor thread
         self.start_post_processor(data_queues, task_queue)
 
@@ -277,17 +276,16 @@
     parser.add_argument('--version', action='version',
                         version='%(prog)s {version}'.format(version=metadata.read_version_string('long')))
     parser.add_argument('--manage_plugins', action='store_true',
                         help='manage installed plugins')
     parser.add_argument('--dev',
                         action='store_true',
                         help='Enable developer mode')
-    parser.add_argument('--dev-local-api',
-                        action='store_true',
-                        help='Enable development against local unmanic support api')
+    parser.add_argument('--dev-api', nargs='?',
+                        help='Enable development against another unmanic support api')
     parser.add_argument('--port', nargs='?',
                         help='Specify the port to run the webserver on')
     # parser.add_argument('--unmanic_path', nargs='?',
     #                    help='Specify the unmanic configuration path instead of ~/.unmanic')
     args = parser.parse_args()
 
     # Configure application from args
@@ -310,13 +308,13 @@
         while not db_connection.is_stopped():
             time.sleep(.2)
             continue
     else:
         # Run the main Unmanic service
         service = Service()
         service.developer = args.dev
-        service.dev_local_api = args.dev_local_api
+        service.dev_api = args.dev_api
         service.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `unmanic-0.2.6/unmanic/webserver/__init__.py` & `unmanic-0.2.7/unmanic/webserver/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_request_router.py` & `unmanic-0.2.7/unmanic/webserver/api_request_router.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/__init__.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/base_api_handler.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/filebrowser_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/filebrowser_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/history_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/history_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/pending_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/pending_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/plugins_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/plugins_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v1/session_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v1/session_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/README.md` & `unmanic-0.2.7/unmanic/webserver/api_v2/README.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/__init__.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/base_api_handler.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/base_api_handler.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/docs_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/docs_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/filebrowser_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/filebrowser_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/history_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/history_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/notifications_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/notifications_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/pending_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/pending_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/plugins_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/plugins_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/schema/__init__.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/schema/schemas.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/schema/schemas.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/schema/swagger.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/schema/unmanic.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/schema/unmanic.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/session_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/session_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/settings_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/settings_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/upload_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/upload_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/version_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/version_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/api_v2/workers_api.py` & `unmanic-0.2.7/unmanic/webserver/api_v2/workers_api.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/docs/api_schema_v2.json` & `unmanic-0.2.7/unmanic/webserver/docs/api_schema_v2.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/docs/api_schema_v2.yaml` & `unmanic-0.2.7/unmanic/webserver/docs/api_schema_v2.yaml`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/docs/privacy_policy.md` & `unmanic-0.2.7/unmanic/webserver/docs/privacy_policy.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/downloads.py` & `unmanic-0.2.7/unmanic/webserver/downloads.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/.eslintrc.js` & `unmanic-0.2.7/unmanic/webserver/frontend/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/LICENSE` & `unmanic-0.2.7/unmanic/webserver/frontend/LICENSE`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/README.md` & `unmanic-0.2.7/unmanic/webserver/frontend/README.md`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/jsconfig.json` & `unmanic-0.2.7/unmanic/webserver/frontend/jsconfig.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/package-lock.json` & `unmanic-0.2.7/unmanic/webserver/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/package.json` & `unmanic-0.2.7/unmanic/webserver/frontend/package.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/public/favicon.ico` & `unmanic-0.2.7/unmanic/webserver/frontend/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-128x128.png` & `unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-16x16.png` & `unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-32x32.png` & `unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/public/icons/favicon-96x96.png` & `unmanic-0.2.7/unmanic/webserver/frontend/public/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/quasar.conf.js` & `unmanic-0.2.7/unmanic/webserver/frontend/quasar.conf.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/scripts/translate.sh` & `unmanic-0.2.7/unmanic/webserver/frontend/scripts/translate.sh`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/App.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/App.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/bg-md1.jpg` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/bg-md1.jpg`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/coffee-btn-image.png` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/coffee-btn-image.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/logo-lg.png` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/logo-lg.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/logo.png` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/logo.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/quasar-logo-vertical.svg`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png` & `unmanic-0.2.7/unmanic/webserver/frontend/src/assets/unmanic-logo-white.png`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/boot/axios.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/boot/axios.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/boot/i18n.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/boot/i18n.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTaskLogDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTasks.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTasks.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/CompletedTasksTable.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DirectoryBrowserDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerAvatar.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerAvatar.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerDataPanelsNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerMainNav.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerMainNav.vue`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
       <q-separator spaced/>
 
 
       <q-item-label header>{{ $t('navigation.account') }}:</q-item-label>
       <!--START LOGOUT-->
       <q-item
-        v-if="unmanicSession && unmanicSession.level && unmanicSession.level > 0"
+        v-if="unmanicSession && unmanicSession.level && unmanicSession.level > 0 && unmanicSession.level !== 9"
         clickable
         @click="logoutSubmit"
         v-ripple>
         <q-item-section avatar>
           <q-icon name="logout"/>
         </q-item-section>
         <q-item-section>
@@ -70,15 +70,15 @@
         <q-item-section avatar>
           <q-icon name="login"/>
         </q-item-section>
         <q-item-section>
           {{ $t('navigation.login') }}
         </q-item-section>
       </q-item>
-      <!--END LOGOUT-->
+      <!--END LOGIN-->
 
       <q-separator spaced/>
 
 
       <q-item-label header>{{ $t('navigation.interface') }}:</q-item-label>
       <!--START LANGUAGE SELECT-->
       <q-item clickable v-ripple>
```

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerNotifications.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerNotifications.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/DrawerSettingsNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/EssentialLink.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/EssentialLink.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/FooterData.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/FooterData.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/JsonImportExportDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/LanguageSwitch.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/LanguageSwitch.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/LibraryConfigurePluginFlowList.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/LinkConfigureDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/LoginDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/LoginDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/MarkdownDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/MarkdownDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/MobileSettingsQuickNav.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/PendingTasks.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/PendingTasks.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/PendingTasksTable.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/PendingTasksTable.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginInstallerManageRepos.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginSelectorDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/PluginsInstalledTable.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/ReleaseNotesDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/ThemeSwitch.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/ThemeSwitch.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerEventCreateDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerGroupConfigureDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgress.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgress.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgressLog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/WorkerProgressStatus.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/dialogs/ConfigDrawerDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/dialogs/PluginInfoDialog.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/forms/LibraryConfigForm.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/components/forms/PluginInstallerForm.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/css/markdown-admonitions.css` & `unmanic-0.2.7/unmanic/webserver/frontend/src/css/markdown-admonitions.css`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/css/quasar.variables.scss` & `unmanic-0.2.7/unmanic/webserver/frontend/src/css/quasar.variables.scss`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/index.template.html` & `unmanic-0.2.7/unmanic/webserver/frontend/src/index.template.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/js/dateTools.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/js/dateTools.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/js/markupParser.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/js/markupParser.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/js/unmanicGlobals.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/js/unmanicGlobals.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/js/unmanicWebsocket.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/js/unmanicWebsocket.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/de.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/de.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/en.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/en.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/es.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/es.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/fr.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/fr.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/it.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/it.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/ja.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/ja.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/mi.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/mi.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/nl.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/nl.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/pl.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/pl.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/pt-br.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/pt-br.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/ru.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/ru.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/sv.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/sv.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/language/zh.json` & `unmanic-0.2.7/unmanic/webserver/frontend/src/language/zh.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/layouts/MainLayout.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/layouts/MainLayout.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/ActionTrigger.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/ActionTrigger.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/DataPanels.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/DataPanels.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/ErrorNotFound.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/ErrorNotFound.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/MainDashboard.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/MainDashboard.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsLibrary.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsLink.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsLink.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsPlugins.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsSupport.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsSupport.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue` & `unmanic-0.2.7/unmanic/webserver/frontend/src/pages/SettingsWorkers.vue`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/router/index.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/router/index.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/frontend/src/router/routes.js` & `unmanic-0.2.7/unmanic/webserver/frontend/src/router/routes.js`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/__init__.py` & `unmanic-0.2.7/unmanic/webserver/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/completed_tasks.py` & `unmanic-0.2.7/unmanic/webserver/helpers/completed_tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/documents.py` & `unmanic-0.2.7/unmanic/webserver/helpers/documents.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/filebrowser.py` & `unmanic-0.2.7/unmanic/webserver/helpers/filebrowser.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/pending_tasks.py` & `unmanic-0.2.7/unmanic/webserver/helpers/pending_tasks.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/plugins.py` & `unmanic-0.2.7/unmanic/webserver/helpers/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/settings.py` & `unmanic-0.2.7/unmanic/webserver/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/helpers/workers.py` & `unmanic-0.2.7/unmanic/webserver/helpers/workers.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/main.py` & `unmanic-0.2.7/unmanic/webserver/main.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/package-lock.json` & `unmanic-0.2.7/unmanic/webserver/package-lock.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/package.json` & `unmanic-0.2.7/unmanic/webserver/package.json`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/plugins.py` & `unmanic-0.2.7/unmanic/webserver/plugins.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/templates/global/insufficient-permissions.html` & `unmanic-0.2.7/unmanic/webserver/templates/global/insufficient-permissions.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/templates/global/login-popup.html` & `unmanic-0.2.7/unmanic/webserver/templates/global/login-popup.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/templates/global/support-future-development.html` & `unmanic-0.2.7/unmanic/webserver/templates/global/support-future-development.html`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic/webserver/websocket.py` & `unmanic-0.2.7/unmanic/webserver/websocket.py`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/unmanic.egg-info/PKG-INFO` & `unmanic-0.2.7/unmanic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unmanic
-Version: 0.2.6
+Version: 0.2.7
 Summary: A simple tool for optimising your video library to a single format
 Home-page: https://github.com/Josh5/unmanic
 Author: Josh.5
 Author-email: jsunnex@gmail.com
 Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com
 License: GPLv3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unmanic Version: 0.2.6 Summary: A simple tool for
+Metadata-Version: 2.1 Name: unmanic Version: 0.2.7 Summary: A simple tool for
 optimising your video library to a single format Home-page: https://github.com/
 Josh5/unmanic Author: Josh.5 Author-email: jsunnex@gmail.com Maintainer: Josh.5
 Maintainer-email: jsunnex@gmail.com License: GPLv3 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `unmanic-0.2.6/unmanic.egg-info/SOURCES.txt` & `unmanic-0.2.7/unmanic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unmanic-0.2.6/versioninfo.py` & `unmanic-0.2.7/versioninfo.py`

 * *Files identical despite different names*

