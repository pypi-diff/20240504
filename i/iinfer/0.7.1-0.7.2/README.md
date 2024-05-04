# Comparing `tmp/iinfer-0.7.1.tar.gz` & `tmp/iinfer-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.7.1.tar", last modified: Fri May  3 09:31:47 2024, max compression
+gzip compressed data, was "iinfer-0.7.2.tar", last modified: Sat May  4 14:25:37 2024, max compression
```

## Comparing `iinfer-0.7.1.tar` & `iinfer-0.7.2.tar`

### file list

```diff
@@ -1,213 +1,217 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.314041 iinfer-0.7.1/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.1/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-05-03 09:31:47.312451 iinfer-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.824564 iinfer-0.7.1/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.944697 iinfer-0.7.1/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.1/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    50217 2024-05-03 09:09:11.000000 iinfer-0.7.1/iinfer/app/app.py
--rw-rw-rw-   0        0        0    34473 2024-05-03 08:22:57.000000 iinfer-0.7.1/iinfer/app/client.py
--rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.1/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.955222 iinfer-0.7.1/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.1/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7466 2024-05-03 09:25:05.000000 iinfer-0.7.1/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0     3613 2024-05-03 05:30:54.000000 iinfer-0.7.1/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.1/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.117723 iinfer-0.7.1/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.1/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.1/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.1/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.1/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.1/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.1/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.1/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.1/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.7.1/iinfer/app/install.py
--rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.1/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.329360 iinfer-0.7.1/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.1/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.1/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.1/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.1/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.1/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.1/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.407932 iinfer-0.7.1/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.7.1/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.7.1/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-05-03 05:32:49.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_San.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    51835 2024-05-03 06:22:29.000000 iinfer-0.7.1/iinfer/app/server.py
--rw-rw-rw-   0        0        0    76670 2024-05-03 07:50:31.000000 iinfer-0.7.1/iinfer/app/web.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.455043 iinfer-0.7.1/iinfer/docker/
--rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.7.1/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.726621 iinfer-0.7.1/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.726096 iinfer-0.7.1/iinfer/extensions/configs/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.475101 iinfer-0.7.1/iinfer/extensions/configs/mmdet/
--rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
--rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tta.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.501672 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/
--rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
--rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
--rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.557196 iinfer-0.7.1/iinfer/extensions/configs/mmseg/
--rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
--rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
--rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
--rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:45.592200 iinfer-0.7.1/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.1/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.1/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.1/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.1/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.1/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.1/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.1/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.1/iinfer/extensions/injection/before_gray_injection.json
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.828969 iinfer-0.7.1/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.1/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.1/iinfer/logconf_web.yml
--rw-rw-rw-   0        0        0     1009 2024-05-03 09:30:13.000000 iinfer-0.7.1/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.839969 iinfer-0.7.1/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.735800 iinfer-0.7.1/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:46.898106 iinfer-0.7.1/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.017638 iinfer-0.7.1/iinfer/web/assets/iinfer/
--rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/filer_modal.js
--rw-rw-rw-   0        0        0    16585 2024-04-30 13:36:02.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/list_cmd.js
--rw-rw-rw-   0        0        0     6537 2024-04-30 13:37:34.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/list_pipe.js
--rw-rw-rw-   0        0        0     5958 2024-05-01 13:45:13.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/main.js
--rw-rw-rw-   0        0        0      421 2024-04-30 13:38:58.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/open_capture.js
--rw-rw-rw-   0        0        0      441 2024-04-30 13:39:09.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/open_output_json.js
--rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.css
--rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.js
--rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/view_raw.js
--rw-rw-rw-   0        0        0     6154 2024-05-02 12:27:53.000000 iinfer-0.7.1/iinfer/web/assets/iinfer/view_result.js
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.041919 iinfer-0.7.1/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.049921 iinfer-0.7.1/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.164118 iinfer-0.7.1/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.214746 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.734650 iinfer-0.7.1/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.228307 iinfer-0.7.1/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.259333 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.273337 iinfer-0.7.1/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.736657 iinfer-0.7.1/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.280334 iinfer-0.7.1/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.297258 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:47.310782 iinfer-0.7.1/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.1/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    31056 2024-05-02 03:04:28.000000 iinfer-0.7.1/iinfer/web/gui.html
-drwxrwxrwx   0        0        0        0 2024-05-03 09:31:44.871292 iinfer-0.7.1/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8562 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 09:31:44.000000 iinfer-0.7.1/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 09:31:47.314550 iinfer-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.497782 iinfer-0.7.2/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-05-04 14:25:37.496655 iinfer-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.792142 iinfer-0.7.2/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.837139 iinfer-0.7.2/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.7.2/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    51232 2024-05-04 02:38:57.000000 iinfer-0.7.2/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    34473 2024-05-03 08:22:57.000000 iinfer-0.7.2/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    14034 2024-05-03 09:11:44.000000 iinfer-0.7.2/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.845140 iinfer-0.7.2/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.7.2/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7868 2024-05-04 02:31:10.000000 iinfer-0.7.2/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0     3613 2024-05-03 05:30:54.000000 iinfer-0.7.2/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.7.2/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.875142 iinfer-0.7.2/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.7.2/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.7.2/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6735 2024-05-02 03:57:31.000000 iinfer-0.7.2/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.7.2/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.7.2/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.7.2/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.7.2/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.7.2/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    15606 2024-05-04 00:27:42.000000 iinfer-0.7.2/iinfer/app/install.py
+-rw-rw-rw-   0        0        0   157090 2024-05-04 14:14:31.000000 iinfer-0.7.2/iinfer/app/options.py
+-rw-rw-rw-   0        0        0     5309 2024-05-02 02:25:26.000000 iinfer-0.7.2/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.910142 iinfer-0.7.2/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.7.2/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.7.2/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.7.2/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.7.2/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.7.2/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6082 2024-05-03 06:19:11.000000 iinfer-0.7.2/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.951140 iinfer-0.7.2/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     3511 2024-05-04 02:00:36.000000 iinfer-0.7.2/iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
+-rw-rw-rw-   0        0        0     7618 2024-05-04 02:00:29.000000 iinfer-0.7.2/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-05-04 02:00:22.000000 iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-05-04 02:00:25.000000 iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-05-04 02:00:14.000000 iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-05-04 02:00:18.000000 iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-05-04 02:00:10.000000 iinfer-0.7.2/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-05-04 02:00:06.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      377 2024-05-02 14:44:28.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_San.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    51835 2024-05-04 00:33:11.000000 iinfer-0.7.2/iinfer/app/server.py
+-rw-rw-rw-   0        0        0    25891 2024-05-04 13:34:13.000000 iinfer-0.7.2/iinfer/app/web.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.967141 iinfer-0.7.2/iinfer/docker/
+-rw-rw-rw-   0        0        0      835 2024-05-03 11:17:19.000000 iinfer-0.7.2/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.976140 iinfer-0.7.2/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.737139 iinfer-0.7.2/iinfer/extensions/configs/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.997139 iinfer-0.7.2/iinfer/extensions/configs/mmdet/
+-rw-rw-rw-   0        0        0      273 2024-05-03 08:33:49.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     7908 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1883 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
+-rw-rw-rw-   0        0        0     1276 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tta.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.014143 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/
+-rw-rw-rw-   0        0        0      252 2024-05-03 08:36:21.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      253 2024-05-03 08:36:59.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
+-rw-rw-rw-   0        0        0      231 2024-05-03 08:35:35.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
+-rw-rw-rw-   0        0        0      236 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/configs/mmpretrain/swin-tiny_16xb64_in1k.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.059145 iinfer-0.7.2/iinfer/extensions/configs/mmseg/
+-rw-rw-rw-   0        0        0      139 2024-03-16 14:01:11.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r101-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      277 2024-03-11 12:50:08.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r18-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0      299 2024-03-11 13:57:39.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/pspnet_r50-d8_4xb2-80k_cityscapes-512x1024.py
+-rw-rw-rw-   0        0        0     2543 2024-05-03 02:44:50.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0     1065 2024-05-02 14:40:03.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py
+-rw-rw-rw-   0        0        0      614 2024-03-30 02:18:25.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      361 2024-03-30 02:17:37.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in22k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0      501 2024-03-23 13:10:40.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-small-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+-rw-rw-rw-   0        0        0     1752 2024-03-23 13:24:30.000000 iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.093141 iinfer-0.7.2/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.2/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.7.2/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      149 2024-05-02 13:46:36.000000 iinfer-0.7.2/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.7.2/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.7.2/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      106 2024-05-02 14:15:04.000000 iinfer-0.7.2/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.7.2/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.7.2/iinfer/extensions/injection/before_gray_injection.json
+-rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/label_coco.txt
+-rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/extensions/label_voc.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.342355 iinfer-0.7.2/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.7.2/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0      630 2024-04-25 10:56:07.000000 iinfer-0.7.2/iinfer/logconf_web.yml
+-rw-rw-rw-   0        0        0     1009 2024-05-04 14:24:26.000000 iinfer-0.7.2/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.344875 iinfer-0.7.2/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.744139 iinfer-0.7.2/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.365879 iinfer-0.7.2/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.391820 iinfer-0.7.2/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5664 2024-04-23 14:00:17.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    16699 2024-05-04 14:05:33.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6537 2024-04-30 13:37:34.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     5958 2024-05-01 13:45:13.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      421 2024-04-30 13:38:58.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      441 2024-04-30 13:39:09.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      127 2024-04-18 14:57:44.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    24976 2024-04-23 14:07:35.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1246 2024-04-23 14:07:58.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     6154 2024-05-02 12:27:53.000000 iinfer-0.7.2/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.394844 iinfer-0.7.2/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.397842 iinfer-0.7.2/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.432508 iinfer-0.7.2/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.459640 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.743140 iinfer-0.7.2/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.461936 iinfer-0.7.2/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.476307 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.480754 iinfer-0.7.2/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.745139 iinfer-0.7.2/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.483598 iinfer-0.7.2/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.492071 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:37.494480 iinfer-0.7.2/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.7.2/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    31056 2024-05-02 03:04:28.000000 iinfer-0.7.2/iinfer/web/gui.html
+drwxrwxrwx   0        0        0        0 2024-05-04 14:25:36.806139 iinfer-0.7.2/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8706 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-04 14:25:36.000000 iinfer-0.7.2/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-04 14:25:37.498305 iinfer-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     2181 2024-05-03 08:40:54.000000 iinfer-0.7.2/setup.py
```

### Comparing `iinfer-0.7.1/LICENSE` & `iinfer-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/PKG-INFO` & `iinfer-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.1
+Version: 0.7.2
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.1/README.md` & `iinfer-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/app.py` & `iinfer-0.7.2/iinfer/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         parser.add_argument('-s', '--saveopt', help=f'save options file. with --useopt option.', action='store_true')
         parser.add_argument('-f', '--format', help='Setting the cmd format.', action='store_true')
         parser.add_argument('-m', '--mode', help='Setting the boot mode.', choices=['redis', 'install', 'server', 'client', 'postprocess', 'gui', 'web'])
         parser.add_argument('--data', help='Setting the data directory.', default=common.HOME_DIR / ".iinfer")
         parser.add_argument('-n', '--name', help='Setting the cmd name.')
         parser.add_argument('--timeout', help='Setting the cmd timeout.', type=int, default=60)
         parser.add_argument('-c', '--cmd', help='Setting the cmd type.',
-                            choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', # install mode
+                            choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', 'diffusers', # install mode
                                     'docker_run', 'docker_stop', # redis mode
                                     'start', 'stop', # server or client or gui mode or web mode
                                     'list' , # server mode
                                     'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
                                     'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove', # client mode
                                     'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
                                     ])
@@ -65,15 +65,15 @@
                             choices=list(common.BASE_AFTER_INJECTIONS.keys()))
         parser.add_argument('--after_injection_conf', help='Setting the cmd deploy after_injection_conf file.')
         parser.add_argument('--after_injection_py', help='Setting the cmd deploy after_injection_py file.', action='append')
         parser.add_argument('--overwrite', help='Setting the cmd deploy overwrite save.', action='store_true')
 
         parser.add_argument('--model_provider', help='Setting the cmd start model_provider.',
                             choices=['CPUExecutionProvider','CUDAExecutionProvider','TensorrtExecutionProvider'], default='CPUExecutionProvider')
-        parser.add_argument('--gpuid', help='Setting the cmd start gpuid.', type=int, default=None)
+        parser.add_argument('--gpuid', help='Setting the cmd start gpuid.', type=str, default=None)
         parser.add_argument('-i', '--input_file', help='Setting the cmd input file.', default=None)
         parser.add_argument('--output_image', help='Setting the cmd output image file.', default=None)
         parser.add_argument('-o', '--output_json', help='Setting the cmd output json file.', default=None)
         parser.add_argument('-a', '--output_json_append', help='Setting append the cmd output json file.', action='store_true')
         parser.add_argument('-P', '--output_preview', help='Setting the output preview.', action='store_true')
         parser.add_argument('--stdin', help='Setting the cmd stdin.', action='store_true')
         parser.add_argument('--nodraw', help='Setting the cmd predict nodraw.', action='store_true')
@@ -126,14 +126,15 @@
         parser.add_argument('--install_iinfer', help='Setting the install server install_iinfer.', type=str, default='iinfer')
         parser.add_argument('--install_onnx', help='Setting the install server install_onnx.', action='store_true')
         parser.add_argument('--install_mmdet', help='Setting the install server install_mmdet.', action='store_true')
         parser.add_argument('--install_mmseg', help='Setting the install server install_mmseg.', action='store_true')
         parser.add_argument('--install_mmcls', help='Setting the install server install_mmcls.', action='store_true')
         parser.add_argument('--install_mmpretrain', help='Setting the install server install_mmpretrain.', action='store_true')
         parser.add_argument('--install_insightface', help='Setting the install server install_insightface.', action='store_true')
+        parser.add_argument('--install_diffusers', help='Setting the install server install_diffusers.', action='store_true')
         parser.add_argument('--install_tag', help='Setting the install server install_tag.', type=str, default=None)
         parser.add_argument('--install_use_gpu', help='Setting the install use gpu.', action='store_true')
 
         parser.add_argument('--allow_host', help='Setting the web mode allow_host.', type=str, default='0.0.0.0')
         parser.add_argument('--listen_port', help='Setting the web mode listen_port.', type=int, default=8081)
 
         argcomplete.autocomplete(parser)
@@ -234,14 +235,15 @@
         install_iinfer = common.getopt(opt, 'install_iinfer', preval=args_dict, withset=True)
         install_onnx = common.getopt(opt, 'install_onnx', preval=args_dict, withset=True)
         install_mmdet = common.getopt(opt, 'install_mmdet', preval=args_dict, withset=True)
         install_mmseg = common.getopt(opt, 'install_mmseg', preval=args_dict, withset=True)
         install_mmcls = common.getopt(opt, 'install_mmcls', preval=args_dict, withset=True)
         install_mmpretrain = common.getopt(opt, 'install_mmpretrain', preval=args_dict, withset=True)
         install_insightface = common.getopt(opt, 'install_insightface', preval=args_dict, withset=True)
+        install_diffusers = common.getopt(opt, 'install_diffusers', preval=args_dict, withset=True)
         install_tag = common.getopt(opt, 'install_tag', preval=args_dict, withset=True)
         install_use_gpu = common.getopt(opt, 'install_use_gpu', preval=args_dict, withset=True)
 
         allow_host = common.getopt(opt, 'allow_host', preval=args_dict, withset=True)
         listen_port = common.getopt(opt, 'listen_port', preval=args_dict, withset=True)
 
         tm = time.perf_counter()
@@ -458,15 +460,16 @@
                 ret = self.cl.file_remove(svpath, timeout=timeout)
                 common.print_format(ret, format, tm, output_json, output_json_append)
                 if 'success' not in ret:
                     return 1, ret
 
             elif cmd == 'predict_type_list':
                 type_list = [dict(predict_type=key, site=val['site'], image_width=val['image_width'], image_height=val['image_height'],
-                                required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight']) for key,val in common.BASE_MODELS.items()]
+                                required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight'],
+                                model_type=f"{val['model_type'].__module__}.{val['model_type'].__name__}") for key,val in common.BASE_MODELS.items()]
                 type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None, required_model_conf=None, required_model_weight=None))
                 ret = dict(success=type_list)
                 common.print_format(ret, format, tm, output_json, output_json_append)
 
             elif cmd == 'capture':
                 count = 0
                 append = False
@@ -673,34 +676,36 @@
             if cmd == 'redis':
                 ret = self.inst.redis()
                 common.print_format(ret, format, tm, output_json, output_json_append)
                 if 'success' not in ret:
                     return 1, ret
 
             elif cmd == 'server':
-                install_set = not (install_onnx or install_mmdet or install_mmseg or install_mmcls or install_mmpretrain or install_insightface)
+                install_set = not (install_onnx or install_mmdet or install_mmseg or install_mmcls or \
+                                   install_mmpretrain or install_insightface or install_diffusers)
                 onnx = install_set
                 mmdet = install_set
                 mmseg = install_set
                 mmcls = False
                 mmpretrain = install_set
                 insightface = install_set
+                diffusers = install_set
                 onnx = install_onnx if install_onnx else onnx
                 mmdet = install_mmdet if install_mmdet else mmdet
                 mmseg = install_mmseg if install_mmseg else mmseg
                 mmcls = install_mmcls if install_mmcls else mmcls
                 mmpretrain = install_mmpretrain if install_mmpretrain else mmpretrain
                 insightface = install_insightface if install_insightface else insightface
                 if data is None:
                     msg = {"warn":f"Please specify the --data option."}
                     common.print_format(msg, format, tm, output_json, output_json_append)
                     return 1, msg
                 ret = self.inst.server(Path(data), install_iinfer, install_onnx=onnx,
                                 install_mmdet=mmdet, install_mmseg=mmseg, install_mmcls=mmcls, install_mmpretrain=mmpretrain,
-                                install_insightface=insightface, install_tag=install_tag, install_use_gpu=install_use_gpu)
+                                install_insightface=insightface, install_diffusers=diffusers, install_tag=install_tag, install_use_gpu=install_use_gpu)
                 common.print_format(ret, format, tm, output_json, output_json_append)
                 if 'success' not in ret:
                     return 1, ret
 
             elif cmd == 'onnx':
                 ret = self.inst.onnx(install_use_gpu=install_use_gpu)
                 common.print_format(ret, format, tm, output_json, output_json_append)
@@ -748,14 +753,24 @@
                     msg = {"warn":f"Please specify the --data option."}
                     common.print_format(msg, format, tm, output_json, output_json_append)
                     return 1, msg
                 ret = self.inst.insightface(Path(data), install_use_gpu=install_use_gpu)
                 common.print_format(ret, format, tm, output_json, output_json_append)
                 if 'success' not in ret:
                     return 1, ret
+            
+            elif cmd == 'diffusers':
+                if data is None:
+                    msg = {"warn":f"Please specify the --data option."}
+                    common.print_format(msg, format, tm, output_json, output_json_append)
+                    return 1, msg
+                ret = self.inst.diffusers(Path(data), install_use_gpu=install_use_gpu)
+                common.print_format(ret, format, tm, output_json, output_json_append)
+                if 'success' not in ret:
+                    return 1, ret
 
             else:
                 msg = {"warn":f"Unkown command."}
                 common.print_format(msg, format, tm, output_json, output_json_append)
                 return 1, msg
 
         else:
```

### Comparing `iinfer-0.7.1/iinfer/app/client.py` & `iinfer-0.7.2/iinfer/app/client.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/common.py` & `iinfer-0.7.2/iinfer/app/common.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/commons/convert.py` & `iinfer-0.7.2/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/commons/module.py` & `iinfer-0.7.2/iinfer/app/commons/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from iinfer.app import common, predict, injection
 from pathlib import Path
 from typing import List, Dict, Any
 import importlib.util
 import inspect
+import iinfer
 import logging
 import pkgutil
 
+import iinfer.app
+import iinfer.app.predict
+
 
 def load_custom_predict(custom_predict_py:Path, logger:logging.Logger) -> predict.Predict:
     """
     カスタム予測オブジェクトを読み込みます。
 
     Args:
         custom_predict_py (Path): カスタム予測オブジェクトのパス
@@ -160,23 +164,30 @@
 for mod in get_module_list('iinfer.app.predicts'):
     if mod.startswith('__'):
         continue
     m = importlib.import_module("iinfer.app.predicts." + mod)
     site = None
     width = None
     height = None
+    model_type = iinfer.app.predict.Predict
     required_model_conf = False
     required_model_weight = False
     for f in dir(m):
+        members = inspect.getmembers(m, inspect.isclass)
+        for name, cls in members:
+            if issubclass(cls, iinfer.app.predict.Predict):
+                model_type = cls
+                break
         if f == 'SITE': site = getattr(m, f)
         elif f == 'IMAGE_WIDTH': width = getattr(m, f)
         elif f == 'IMAGE_HEIGHT': height = getattr(m, f)
+        elif f == 'MODEL_TYPE': model_type = getattr(m, f)
         elif f == 'REQUIREd_MODEL_CONF': required_model_conf = getattr(m, f)
         elif f == 'REQUIREd_MODEL_WEIGHT': required_model_weight = getattr(m, f)
-    common.BASE_MODELS[mod] = dict(site=site, image_width=width, image_height=height,
+    common.BASE_MODELS[mod] = dict(site=site, image_width=width, image_height=height, model_type=model_type,
                                    required_model_conf=required_model_conf, required_model_weight=required_model_weight)
 
 for mod in get_module_list('iinfer.app.injections'):
     if mod.startswith('__'):
         continue
     try:
         load_before_injection_type([mod], dict(), None)
```

### Comparing `iinfer-0.7.1/iinfer/app/gui.py` & `iinfer-0.7.2/iinfer/app/gui.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injection.py` & `iinfer-0.7.2/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_det_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_http_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.7.2/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.7.2/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/install.py` & `iinfer-0.7.2/iinfer/app/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
             return {"success": f"Success to install redis-server."}
 
         else:
             return {"warn":f"Unsupported platform."}
 
     def server(self, data:Path, install_iinfer:str='iinfer', install_onnx:bool=True,
                install_mmdet:bool=True, install_mmseg:bool=True, install_mmcls:bool=False, install_mmpretrain:bool=True,
-               install_insightface=False, install_tag:str=None, install_use_gpu:bool=False):
+               install_insightface=False, install_diffusers=True,
+               install_tag:str=None, install_use_gpu:bool=False):
         if platform.system() == 'Windows':
             return {"warn": f"Build server command is Unsupported in windows platform."}
         from importlib.resources import read_text
         user = getpass.getuser()
         install_tag = f"_{install_tag}" if install_tag is not None else ''
         with open('Dockerfile', 'w', encoding='utf-8') as fp:
             text = read_text(f'{common.APP_ID}.docker', 'Dockerfile')
@@ -62,14 +63,15 @@
             text = text.replace('#{INSTALL_IINFER}', install_iinfer)
             text = text.replace('#{INSTALL_ONNX}', f'RUN iinfer -m install -c onnx --data /home/{user}/.iinfer {install_use_gpu}' if install_onnx else '')
             text = text.replace('#{INSTALL_MMDET}', f'RUN iinfer -m install -c mmdet --data /home/{user}/.iinfer {install_use_gpu}' if install_mmdet else '')
             text = text.replace('#{INSTALL_MMSEG}', f'RUN iinfer -m install -c mmseg --data /home/{user}/.iinfer {install_use_gpu}' if install_mmseg else '')
             text = text.replace('#{INSTALL_MMCLS}', f'RUN iinfer -m install -c mmcls --data /home/{user}/.iinfer {install_use_gpu}' if install_mmcls else '')
             text = text.replace('#{INSTALL_MMPRETRAIN}', f'RUN iinfer -m install -c mmpretrain --data /home/{user}/.iinfer {install_use_gpu}' if install_mmpretrain else '')
             text = text.replace('#{INSTALL_INSIGHTFACE}', f'RUN iinfer -m install -c insightface --data /home/{user}/.iinfer {install_use_gpu}' if install_insightface else '')
+            text = text.replace('#{INSTALL_DIFFUSERS}', f'RUN iinfer -m install -c diffusers --data /home/{user}/.iinfer {install_use_gpu}' if install_diffusers else '')
             fp.write(text)
         docker_compose_path = Path('docker-compose.yml')
         if not docker_compose_path.exists():
             with open(docker_compose_path, 'w', encoding='utf-8') as fp:
                 text = read_text(f'{common.APP_ID}.docker', 'docker-compose.yml')
                 fp.write(text)
         with open(f'docker-compose.yml', 'r+', encoding='utf-8') as fp:
@@ -172,14 +174,21 @@
         else:
             returncode, _ = common.cmd('mim install mmcv>=2.0.0', logger=self.logger)
         if returncode != 0:
             self.logger.error(f"Failed to install mmcv.")
             return {"error": f"Failed to install mmcv."}
         return {"success": f"Success to install mmcv."}
 
+    def _transformers(self, install_use_gpu:bool=False):
+        returncode, _ = common.cmd('pip install accelerate transformers', logger=self.logger)
+        if returncode != 0:
+            self.logger.error(f"Failed to install accelerate transformers.")
+            return {"error": f"Failed to install accelerate transformers."}
+        return {"success": f"Success to install accelerate transformers."}
+
     def mmdet(self, data_dir:Path, install_use_gpu:bool=False):
         returncode, _ = common.cmd(f'git clone https://github.com/open-mmlab/mmdetection.git', logger=self.logger)
         if returncode != 0:
             self.logger.error(f"Failed to git clone mmdetection.")
             return {"error": f"Failed to git clone mmdetection."}
         srcdir = Path('.') / 'mmdetection'
         shutil.copytree(srcdir, data_dir / 'mmdetection', dirs_exist_ok=True, ignore=shutil.ignore_patterns('.git'))
@@ -272,7 +281,20 @@
         if ret != 0:
             self.logger.error(f"Failed to install mmpretrain.")
             return {"error": f"Failed to install mmpretrain."}
 
         if srcdir.exists():
             return {"success": f"Please remove '{srcdir}' manually."}
         return {"success": f"Success to install mmpretrain."}
+
+    def diffusers(self, data_dir:Path, install_use_gpu:bool=False):
+        ret = self._torch(install_use_gpu)
+        if "error" in ret: return ret
+        ret = self._transformers(install_use_gpu)
+        if "error" in ret: return ret
+
+        ret, _ = common.cmd('pip install diffusers', logger=self.logger)
+        if ret != 0:
+            self.logger.error(f"Failed to install diffusers.")
+            return {"error": f"Failed to install diffusers."}
+
+        return {"success": f"Success to install diffusers."}
```

### Comparing `iinfer-0.7.1/iinfer/app/postprocess.py` & `iinfer-0.7.2/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.7.2/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/csv.py` & `iinfer-0.7.2/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.7.2/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.7.2/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.7.2/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.7.2/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.7.2/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.7.2/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.7.2/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predict.py` & `iinfer-0.7.2/iinfer/app/predict.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/insightface_det.py` & `iinfer-0.7.2/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.7.2/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.7.2/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.7.2/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.7.2/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.7.2/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.7.2/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.7.2/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/redis.py` & `iinfer-0.7.2/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/app/server.py` & `iinfer-0.7.2/iinfer/app/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
             self.logger.warn(f"{name} is not deployed.")
             self.responce(reskey, {"warn": f"{name} is not deployed."})
             return self.RESP_WARN
         common.rmdirs(deploy_dir)
         self.responce(reskey, {"success": f"Undeployed {name}. {str(deploy_dir)}"})
         return self.RESP_SCCESS
 
-    def start(self, reskey:str, name:str, model_provider:str, use_track:bool, gpuid:int):
+    def start(self, reskey:str, name:str, model_provider:str, use_track:bool, gpuid:str):
         """
         モデルを読み込み、処理が実行できるようにする
 
         Args:
             reskey (str): レスポンスキー
             name (str): モデル名
             model_provider (str, optional): 推論実行時のモデルプロバイダー。デフォルトは'CPUExecutionProvider'。
```

### Comparing `iinfer-0.7.1/iinfer/docker/Dockerfile` & `iinfer-0.7.2/iinfer/docker/Dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 #{INSTALL_ONNX}
 #{INSTALL_MMDET}
 #{INSTALL_MMSEG}
 #{INSTALL_MMCLS}
 #{INSTALL_MMPRETRAIN}
 #{INSTALL_INSIGHTFACE}
+#{INSTALL_DIFFUSERS}
 RUN mkdir -p /home/${MKUSER}/.iinfer && chown -R ${MKUSER}:${MKUSER} /home/${MKUSER}/.iinfer
 
 ENV REDIS_HOST=redis
 ENV REDIS_PORT=6379
 ENV REDIS_PASSWORD=password
 ENV SVNAME=server#{INSTALL_TAG}
```

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmdet/yolox_tta.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmdet/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-b16_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmseg/san-vit-l14_coco-stuff164k-640x640.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-base-patch4-window12-in1k-384x384-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py` & `iinfer-0.7.2/iinfer/extensions/configs/mmseg/swin-tiny-patch4-window7-in1k-pre_upernet_8xb2-160k_ade20k-512x512.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.7.2/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/licenses/files.txt` & `iinfer-0.7.2/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_client.yml` & `iinfer-0.7.2/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_gui.yml` & `iinfer-0.7.2/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_install.yml` & `iinfer-0.7.2/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_postprocess.yml` & `iinfer-0.7.2/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_redis.yml` & `iinfer-0.7.2/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_server.yml` & `iinfer-0.7.2/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/logconf_web.yml` & `iinfer-0.7.2/iinfer/logconf_web.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/version.py` & `iinfer-0.7.2/iinfer/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 5, 3)
+dt_now = datetime.datetime(2024, 5, 4)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.7.2/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/filer_modal.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/filer_modal.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/list_cmd.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/list_cmd.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -117,14 +117,15 @@
                             '</svg>');
                         input_elem.parent().append(btn_t);
                         btn_t.click(mk_func(input_elem.parent().parent(), row));
                     }
                 }
                 title = elem.find('.row_content_template_title');
                 title.html('');
+                title.attr('title', window.navigator.language == 'ja' ? row['discription_ja'] : row['discription_en'])
                 if (row['required']) {
                     title.append('<span class="text-danger">*</span>');
                 }
                 title.append(`<span>${row['opt']}</span>`);
                 if (row['hide']) {
                     elem.addClass('row_content_hide');
                 } else {
```

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/list_pipe.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/list_pipe.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/main.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/main.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/svfiler.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/svfiler.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/view_raw.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/view_raw.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/iinfer/view_result.js` & `iinfer-0.7.2/iinfer/web/assets/iinfer/view_result.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.7.2/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.7.2/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.7.2/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.7.2/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.7.2/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.7.2/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.7.2/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.7.2/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer/web/gui.html` & `iinfer-0.7.2/iinfer/web/gui.html`

 * *Files identical despite different names*

### Comparing `iinfer-0.7.1/iinfer.egg-info/PKG-INFO` & `iinfer-0.7.2/iinfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.7.1
+Version: 0.7.2
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.7.1/iinfer.egg-info/SOURCES.txt` & `iinfer-0.7.2/iinfer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 iinfer/app/__init__.py
 iinfer/app/app.py
 iinfer/app/client.py
 iinfer/app/common.py
 iinfer/app/gui.py
 iinfer/app/injection.py
 iinfer/app/install.py
+iinfer/app/options.py
 iinfer/app/postprocess.py
 iinfer/app/predict.py
 iinfer/app/redis.py
 iinfer/app/server.py
 iinfer/app/web.py
 iinfer/app/commons/convert.py
 iinfer/app/commons/module.py
@@ -46,14 +47,15 @@
 iinfer/app/postprocesses/det_face_store.py
 iinfer/app/postprocesses/det_filter.py
 iinfer/app/postprocesses/det_jadge.py
 iinfer/app/postprocesses/httpreq.py
 iinfer/app/postprocesses/seg_bbox.py
 iinfer/app/postprocesses/seg_filter.py
 iinfer/app/predicts/__init__.py
+iinfer/app/predicts/diffusers_stablediffusion_txt2img.py
 iinfer/app/predicts/insightface_det.py
 iinfer/app/predicts/mmdet_det_YoloX.py
 iinfer/app/predicts/mmdet_det_YoloX_Lite.py
 iinfer/app/predicts/mmpretrain_cls_swin.py
 iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
 iinfer/app/predicts/mmrotate_det_ReDet.py
 iinfer/app/predicts/mmseg_seg_PSPNet.py
@@ -64,14 +66,16 @@
 iinfer/app/predicts/onnx_det_YoloV3.py
 iinfer/app/predicts/onnx_det_YoloX.py
 iinfer/app/predicts/onnx_det_YoloX_Lite.py
 iinfer/docker/Dockerfile
 iinfer/docker/__init__.py
 iinfer/docker/build.sh
 iinfer/docker/docker-compose.yml
+iinfer/extensions/label_coco.txt
+iinfer/extensions/label_voc.txt
 iinfer/extensions/configs/mmdet/yolox_l_8xb8-300e_coco.py
 iinfer/extensions/configs/mmdet/yolox_s_8xb8-300e_coco.py
 iinfer/extensions/configs/mmdet/yolox_tiny_8xb8-300e_coco.py
 iinfer/extensions/configs/mmdet/yolox_tta.py
 iinfer/extensions/configs/mmpretrain/swin-base_16xb64_in1k-384px.py
 iinfer/extensions/configs/mmpretrain/swin-large_16xb64_in1k-384px.py
 iinfer/extensions/configs/mmpretrain/swin-small_16xb64_in1k.py
```

### Comparing `iinfer-0.7.1/setup.py` & `iinfer-0.7.2/setup.py`

 * *Files identical despite different names*

