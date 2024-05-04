# Comparing `tmp/freegenius-0.2.5.tar.gz` & `tmp/freegenius-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.2.5.tar", last modified: Sat May  4 14:07:32 2024, max compression
+gzip compressed data, was "freegenius-0.2.6.tar", last modified: Sat May  4 15:13:09 2024, max compression
```

## Comparing `freegenius-0.2.5.tar` & `freegenius-0.2.6.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.357829 freegenius-0.2.5/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 14:07:32.357829 freegenius-0.2.5/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.329830 freegenius-0.2.5/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-04 14:07:31.000000 freegenius-0.2.5/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.5/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.329830 freegenius-0.2.5/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.5/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.5/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.5/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.5/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.5/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.5/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.5/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.5/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.5/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.5/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:31.000000 freegenius-0.2.5/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.5/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.329830 freegenius-0.2.5/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.5/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.5/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.5/freegenius/geminiprovision.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6513 2024-05-02 21:45:33.000000 freegenius-0.2.5/freegenius/groqchat.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.329830 freegenius-0.2.5/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.5/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.5/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.329830 freegenius-0.2.5/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.5/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.341830 freegenius-0.2.5/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.5/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.5/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.5/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.5/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.5/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.5/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.325830 freegenius-0.2.5/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.321830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.325830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.345830 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.5/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.5/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-04 14:07:31.000000 freegenius-0.2.5/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.5/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.353829 freegenius-0.2.5/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.5/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.5/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.5/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.5/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.5/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.5/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.5/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.5/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.5/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2563 2024-05-02 19:23:00.000000 freegenius-0.2.5/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.5/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.5/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.5/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.5/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.5/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.5/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.5/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.5/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.5/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.5/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.5/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.5/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.5/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.5/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.5/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.5/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.5/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.5/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.5/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.5/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.5/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1165 2024-05-02 19:22:09.000000 freegenius-0.2.5/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.5/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.5/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.5/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.5/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.5/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.5/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.5/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.5/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.5/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-05-04 11:11:55.000000 freegenius-0.2.5/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.5/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.5/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.353829 freegenius-0.2.5/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.5/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.357829 freegenius-0.2.5/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   113329 2024-05-04 14:06:08.000000 freegenius-0.2.5/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    30152 2024-05-03 15:57:52.000000 freegenius-0.2.5/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17682 2024-05-03 15:59:20.000000 freegenius-0.2.5/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21380 2024-05-03 15:52:00.000000 freegenius-0.2.5/freegenius/utils/call_groq.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    25047 2024-05-03 16:02:40.000000 freegenius-0.2.5/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.5/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19102 2024-05-03 16:04:26.000000 freegenius-0.2.5/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18528 2024-05-04 13:26:06.000000 freegenius-0.2.5/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.5/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.5/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.5/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4976 2024-05-04 08:21:49.000000 freegenius-0.2.5/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.5/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.5/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.5/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.5/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.5/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    51559 2024-05-04 10:54:38.000000 freegenius-0.2.5/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.5/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.5/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.5/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.5/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.5/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.5/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.5/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.5/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11304 2024-05-04 13:53:35.000000 freegenius-0.2.5/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9014 2024-05-04 13:26:35.000000 freegenius-0.2.5/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4721 2024-05-04 10:56:37.000000 freegenius-0.2.5/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 14:07:32.357829 freegenius-0.2.5/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-04 14:07:32.000000 freegenius-0.2.5/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-04 14:07:32.357829 freegenius-0.2.5/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10573 2024-05-04 14:06:20.000000 freegenius-0.2.5/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.326496 freegenius-0.2.6/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 15:13:09.326496 freegenius-0.2.6/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.294497 freegenius-0.2.6/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11707 2024-05-04 15:13:08.000000 freegenius-0.2.6/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.2.6/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.298497 freegenius-0.2.6/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.2.6/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.2.6/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.2.6/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.2.6/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7006 2024-04-28 21:17:47.000000 freegenius-0.2.6/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.2.6/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11081 2024-04-28 21:19:22.000000 freegenius-0.2.6/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.2.6/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.2.6/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.2.6/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:08.000000 freegenius-0.2.6/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.2.6/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.298497 freegenius-0.2.6/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.2.6/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.2.6/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.2.6/freegenius/geminiprovision.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6513 2024-05-02 21:45:33.000000 freegenius-0.2.6/freegenius/groqchat.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.298497 freegenius-0.2.6/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.2.6/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.2.6/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.298497 freegenius-0.2.6/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.2.6/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.310496 freegenius-0.2.6/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.2.6/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.2.6/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.2.6/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.2.6/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.2.6/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.2.6/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.310496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.310496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.290497 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.314496 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.2.6/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.2.6/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-05-04 15:13:08.000000 freegenius-0.2.6/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.2.6/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.322496 freegenius-0.2.6/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.2.6/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.2.6/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.2.6/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.2.6/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.2.6/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7437 2024-04-27 13:00:33.000000 freegenius-0.2.6/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.2.6/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4677 2024-04-27 13:03:55.000000 freegenius-0.2.6/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.2.6/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2563 2024-05-02 19:23:00.000000 freegenius-0.2.6/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.2.6/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.2.6/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.2.6/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5160 2024-04-27 13:04:35.000000 freegenius-0.2.6/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.2.6/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.2.6/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.2.6/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.2.6/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.2.6/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.2.6/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.2.6/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.2.6/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.2.6/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.2.6/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.2.6/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.2.6/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8646 2024-04-27 13:03:30.000000 freegenius-0.2.6/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.2.6/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.2.6/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.2.6/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5906 2024-04-27 11:30:39.000000 freegenius-0.2.6/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1165 2024-05-02 19:22:09.000000 freegenius-0.2.6/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.2.6/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.2.6/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.2.6/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.2.6/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.2.6/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.2.6/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.2.6/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.2.6/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.2.6/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      840 2024-05-04 11:11:55.000000 freegenius-0.2.6/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.2.6/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7714 2024-04-27 15:10:04.000000 freegenius-0.2.6/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.322496 freegenius-0.2.6/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.2.6/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.326496 freegenius-0.2.6/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   113355 2024-05-04 15:03:01.000000 freegenius-0.2.6/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    30152 2024-05-03 15:57:52.000000 freegenius-0.2.6/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17682 2024-05-03 15:59:20.000000 freegenius-0.2.6/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21380 2024-05-03 15:52:00.000000 freegenius-0.2.6/freegenius/utils/call_groq.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    25047 2024-05-03 16:02:40.000000 freegenius-0.2.6/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8528 2024-04-27 07:40:12.000000 freegenius-0.2.6/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19102 2024-05-03 16:04:26.000000 freegenius-0.2.6/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18528 2024-05-04 13:26:06.000000 freegenius-0.2.6/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.2.6/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.2.6/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.2.6/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4976 2024-05-04 08:21:49.000000 freegenius-0.2.6/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.2.6/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.2.6/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.2.6/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.2.6/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.2.6/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    51559 2024-05-04 10:54:38.000000 freegenius-0.2.6/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.2.6/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.2.6/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.2.6/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.2.6/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.2.6/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.2.6/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.2.6/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4353 2024-05-02 17:22:30.000000 freegenius-0.2.6/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11304 2024-05-04 13:53:35.000000 freegenius-0.2.6/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9015 2024-05-04 15:02:12.000000 freegenius-0.2.6/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4721 2024-05-04 10:56:37.000000 freegenius-0.2.6/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-05-04 15:13:09.326496 freegenius-0.2.6/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    14884 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5909 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      841 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-05-04 15:13:09.000000 freegenius-0.2.6/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-05-04 15:13:09.326496 freegenius-0.2.6/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10460 2024-05-04 15:03:22.000000 freegenius-0.2.6/setup.py
```

### Comparing `freegenius-0.2.5/PKG-INFO` & `freegenius-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.5
+Version: 0.2.6
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.2.5/freegenius/README.md` & `freegenius-0.2.6/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/__init__.py` & `freegenius-0.2.6/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/audio/notification1.mp3` & `freegenius-0.2.6/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/audio/notification1_mild.mp3` & `freegenius-0.2.6/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/audio/notification2.mp3` & `freegenius-0.2.6/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/audio/notification2_mild.mp3` & `freegenius-0.2.6/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/autoassist.py` & `freegenius-0.2.6/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/autobuilder.py` & `freegenius-0.2.6/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/autoretriever.py` & `freegenius-0.2.6/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/chatgpt.py` & `freegenius-0.2.6/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/codey.py` & `freegenius-0.2.6/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/commandprompt.py` & `freegenius-0.2.6/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/eTextEdit.py` & `freegenius-0.2.6/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/geminipro.py` & `freegenius-0.2.6/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/geminiprovision.py` & `freegenius-0.2.6/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/groqchat.py` & `freegenius-0.2.6/freegenius/groqchat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/gui/chatgui.py` & `freegenius-0.2.6/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/gui/worker.py` & `freegenius-0.2.6/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/icons/FreeGenius.ico` & `freegenius-0.2.6/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/icons/FreeGenius.png` & `freegenius-0.2.6/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/icons/FreeGenius_original.png` & `freegenius-0.2.6/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/icons/ai.png` & `freegenius-0.2.6/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/icons/ai_original.png` & `freegenius-0.2.6/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/llamacpp.py` & `freegenius-0.2.6/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.2.6/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/main.py` & `freegenius-0.2.6/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/ollamachat.py` & `freegenius-0.2.6/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/palm2.py` & `freegenius-0.2.6/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.2.6/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.2.6/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/000_check_vlc.py` & `freegenius-0.2.6/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/add calendar event.py` & `freegenius-0.2.6/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/aliases.py` & `freegenius-0.2.6/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/analyze audio.py` & `freegenius-0.2.6/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/analyze files.py` & `freegenius-0.2.6/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/analyze images.py` & `freegenius-0.2.6/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/analyze web content.py` & `freegenius-0.2.6/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/auto correct python code.py` & `freegenius-0.2.6/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/awesome prompts.py` & `freegenius-0.2.6/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/character analysis.py` & `freegenius-0.2.6/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/chat.py` & `freegenius-0.2.6/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/contexts.py` & `freegenius-0.2.6/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/counselling.py` & `freegenius-0.2.6/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/create ai assistants.py` & `freegenius-0.2.6/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/create images.py` & `freegenius-0.2.6/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/create maps.py` & `freegenius-0.2.6/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/create qrcode.py` & `freegenius-0.2.6/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/create statistical graphics.py` & `freegenius-0.2.6/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/dates and times.py` & `freegenius-0.2.6/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/download youtube or web content.py` & `freegenius-0.2.6/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/edit text.py` & `freegenius-0.2.6/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/execute computing tasks.py` & `freegenius-0.2.6/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/execute termux command.py` & `freegenius-0.2.6/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/global finance.py` & `freegenius-0.2.6/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/improve British English.py` & `freegenius-0.2.6/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/input suggestions.py` & `freegenius-0.2.6/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/install python package.py` & `freegenius-0.2.6/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/integrate google searches.py` & `freegenius-0.2.6/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/memory.py` & `freegenius-0.2.6/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/modify images.py` & `freegenius-0.2.6/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/open web browser.py` & `freegenius-0.2.6/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/pronounce words.py` & `freegenius-0.2.6/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/remove image background.py` & `freegenius-0.2.6/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/search chat records.py` & `freegenius-0.2.6/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/search financial data.py` & `freegenius-0.2.6/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/search latest news.py` & `freegenius-0.2.6/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/search sqlite.py` & `freegenius-0.2.6/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/search weather info.py` & `freegenius-0.2.6/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/send email.py` & `freegenius-0.2.6/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/send tweet.py` & `freegenius-0.2.6/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.2.6/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.2.6/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/rag.py` & `freegenius-0.2.6/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/requirements.txt` & `freegenius-0.2.6/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/servers.py` & `freegenius-0.2.6/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/systemtray.py` & `freegenius-0.2.6/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/assistant.py` & `freegenius-0.2.6/freegenius/utils/assistant.py`

 * *Files 0% similar despite different names*

```diff
@@ -4997,2088 +4997,2089 @@
 00013840: 6578 742d 746f 2d53 7065 6563 6820 2841  ext-to-Speech (A
 00013850: 5049 2922 2c20 2245 6c65 7665 6e4c 6162  PI)", "ElevenLab
 00013860: 7320 2841 5049 2922 2c20 2243 7573 746f  s (API)", "Custo
 00013870: 6d20 5465 7874 2d74 6f2d 5370 6565 6368  m Text-to-Speech
 00013880: 2043 6f6d 6d61 6e64 205b 6164 7661 6e63   Command [advanc
 00013890: 6564 5d22 5d0a 2020 2020 2020 2020 6966  ed]"].        if
 000138a0: 2063 6f6e 6669 672e 7468 6973 506c 6174   config.thisPlat
-000138b0: 666f 726d 203d 3d20 224c 696e 7578 223a  form == "Linux":
-000138c0: 0a20 2020 2020 2020 2020 2020 206f 7074  .            opt
-000138d0: 696f 6e73 2e69 6e73 6572 7428 302c 2022  ions.insert(0, "
-000138e0: 7069 7065 7222 290a 2020 2020 2020 2020  piper").        
-000138f0: 2020 2020 6465 7363 7269 7074 696f 6e73      descriptions
-00013900: 2e69 6e73 6572 7428 302c 2022 5069 7065  .insert(0, "Pipe
-00013910: 7220 284f 6666 6c69 6e65 2922 290a 2020  r (Offline)").  
-00013920: 2020 2020 2020 7474 7350 6c61 7466 6f72        ttsPlatfor
-00013930: 6d20 3d20 7365 6c66 2e64 6961 6c6f 6773  m = self.dialogs
-00013940: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
-00013950: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
-00013960: 7469 6f6e 733d 6f70 7469 6f6e 732c 0a20  tions=options,. 
-00013970: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00013980: 6970 7469 6f6e 733d 6465 7363 7269 7074  iptions=descript
-00013990: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-000139a0: 2020 7469 746c 653d 2254 6578 742d 746f    title="Text-to
-000139b0: 2d53 7065 6563 6820 436f 6e66 6967 7572  -Speech Configur
-000139c0: 6174 696f 6e73 222c 0a20 2020 2020 2020  ations",.       
-000139d0: 2020 2020 2074 6578 743d 2253 656c 6563       text="Selec
-000139e0: 7420 6120 7465 7874 2d74 6f2d 7370 6565  t a text-to-spee
-000139f0: 6368 2070 6c61 7466 6f72 6d3a 222c 0a20  ch platform:",. 
-00013a00: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-00013a10: 6c74 3d63 6f6e 6669 672e 7474 7350 6c61  lt=config.ttsPla
-00013a20: 7466 6f72 6d2c 0a20 2020 2020 2020 2029  tform,.        )
-00013a30: 0a20 2020 2020 2020 2069 6620 7474 7350  .        if ttsP
-00013a40: 6c61 7466 6f72 6d3a 0a20 2020 2020 2020  latform:.       
-00013a50: 2020 2020 2069 6620 7474 7350 6c61 7466       if ttsPlatf
-00013a60: 6f72 6d20 3d3d 2022 676f 6f67 6c65 636c  orm == "googlecl
-00013a70: 6f75 6422 2061 6e64 206e 6f74 2028 6f73  oud" and not (os
-00013a80: 2e65 6e76 6972 6f6e 5b22 474f 4f47 4c45  .environ["GOOGLE
-00013a90: 5f41 5050 4c49 4341 5449 4f4e 5f43 5245  _APPLICATION_CRE
-00013aa0: 4445 4e54 4941 4c53 225d 2061 6e64 2022  DENTIALS"] and "
-00013ab0: 5465 7874 2d74 6f2d 5370 6565 6368 2220  Text-to-Speech" 
-00013ac0: 696e 2063 6f6e 6669 672e 656e 6162 6c65  in config.enable
-00013ad0: 6447 6f6f 676c 6541 5049 7329 3a0a 2020  dGoogleAPIs):.  
-00013ae0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00013af0: 696e 7432 2822 476f 6f67 6c65 2043 6c6f  int2("Google Clo
-00013b00: 7564 2054 6578 742d 746f 2d53 7065 6563  ud Text-to-Speec
-00013b10: 6820 6665 6174 7572 6520 6973 206e 6f74  h feature is not
-00013b20: 2065 6e61 626c 6564 2122 290a 2020 2020   enabled!").    
-00013b30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00013b40: 7433 2822 5265 6164 3a20 6874 7470 733a  t3("Read: https:
-00013b50: 2f2f 6769 7468 7562 2e63 6f6d 2f65 6c69  //github.com/eli
-00013b60: 7261 6e77 6f6e 672f 6c65 746d 6564 6f69  ranwong/letmedoi
-00013b70: 742f 7769 6b69 2f47 6f6f 676c 652d 4150  t/wiki/Google-AP
-00013b80: 492d 5365 7475 7022 290a 2020 2020 2020  I-Setup").      
-00013b90: 2020 2020 2020 2020 2020 7072 696e 7433            print3
-00013ba0: 2822 5465 7874 2d74 6f2d 5370 6565 6368  ("Text-to-Speech
-00013bb0: 2070 6c61 7466 6f72 6d20 6368 616e 6765   platform change
-00013bc0: 6420 746f 3a20 476f 6f67 6c65 2054 6578  d to: Google Tex
-00013bd0: 742d 746f 2d53 7065 6563 6820 2847 656e  t-to-Speech (Gen
-00013be0: 6572 6963 2922 290a 2020 2020 2020 2020  eric)").        
-00013bf0: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
-00013c00: 7473 506c 6174 666f 726d 203d 2022 676f  tsPlatform = "go
-00013c10: 6f67 6c65 220a 2020 2020 2020 2020 2020  ogle".          
-00013c20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00013c30: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
-00013c40: 7473 506c 6174 666f 726d 203d 2074 7473  tsPlatform = tts
-00013c50: 506c 6174 666f 726d 0a20 2020 2020 2020  Platform.       
-00013c60: 2023 2066 7572 7468 6572 206f 7074 696f   # further optio
-00013c70: 6e73 0a20 2020 2020 2020 2069 6620 636f  ns.        if co
-00013c80: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
-00013c90: 203d 3d20 2267 6f6f 676c 6522 3a0a 2020   == "google":.  
-00013ca0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00013cb0: 6574 4774 7473 4c61 6e67 7561 6765 2829  etGttsLanguage()
-00013cc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013cd0: 662e 7365 7441 7564 696f 506c 6179 6261  f.setAudioPlayba
-00013ce0: 636b 546f 6f6c 2829 0a20 2020 2020 2020  ckTool().       
-00013cf0: 2020 2020 2073 656c 662e 7365 7456 6c63       self.setVlc
-00013d00: 5370 6565 6428 290a 2020 2020 2020 2020  Speed().        
-00013d10: 656c 6966 2063 6f6e 6669 672e 7474 7350  elif config.ttsP
-00013d20: 6c61 7466 6f72 6d20 3d3d 2022 676f 6f67  latform == "goog
-00013d30: 6c65 636c 6f75 6422 3a0a 2020 2020 2020  lecloud":.      
-00013d40: 2020 2020 2020 7365 6c66 2e73 6574 4763        self.setGc
-00013d50: 7474 734c 616e 6775 6167 6528 290a 2020  ttsLanguage().  
-00013d60: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00013d70: 6574 4763 7474 7353 7065 6564 2829 0a20  etGcttsSpeed(). 
-00013d80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013d90: 7365 7441 7564 696f 506c 6179 6261 636b  setAudioPlayback
-00013da0: 546f 6f6c 2829 0a20 2020 2020 2020 2020  Tool().         
-00013db0: 2020 2073 656c 662e 7365 7456 6c63 5370     self.setVlcSp
-00013dc0: 6565 6428 290a 2020 2020 2020 2020 6966  eed().        if
-00013dd0: 2063 6f6e 6669 672e 7474 7350 6c61 7466   config.ttsPlatf
-00013de0: 6f72 6d20 3d3d 2022 7069 7065 7222 3a0a  orm == "piper":.
-00013df0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013e00: 2e73 6574 5069 7065 7256 6f69 6365 2829  .setPiperVoice()
-00013e10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013e20: 662e 7365 7441 7564 696f 506c 6179 6261  f.setAudioPlayba
-00013e30: 636b 546f 6f6c 2829 0a20 2020 2020 2020  ckTool().       
-00013e40: 2020 2020 2073 656c 662e 7365 7456 6c63       self.setVlc
-00013e50: 5370 6565 6428 290a 2020 2020 2020 2020  Speed().        
-00013e60: 656c 6966 2063 6f6e 6669 672e 7474 7350  elif config.ttsP
-00013e70: 6c61 7466 6f72 6d20 3d3d 2022 656c 6576  latform == "elev
-00013e80: 656e 6c61 6273 223a 0a20 2020 2020 2020  enlabs":.       
-00013e90: 2020 2020 2069 6620 6e6f 7420 636f 6e66       if not conf
-00013ea0: 6967 2e65 6c65 7665 6e6c 6162 7341 7069  ig.elevenlabsApi
-00013eb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013ec0: 2020 7365 6c66 2e63 6861 6e67 6545 6c65    self.changeEle
-00013ed0: 7665 6e6c 6162 7341 7069 2829 0a20 2020  venlabsApi().   
-00013ee0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00013ef0: 636f 6e66 6967 2e65 6c65 7665 6e6c 6162  config.elevenlab
-00013f00: 7341 7069 3a0a 2020 2020 2020 2020 2020  sApi:.          
-00013f10: 2020 2020 2020 7072 696e 7431 2822 456c        print1("El
-00013f20: 6576 656e 4c61 6273 2041 5049 206b 6579  evenLabs API key
-00013f30: 206e 6f74 2066 6f75 6e64 2122 290a 2020   not found!").  
-00013f40: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00013f50: 696e 7433 2822 5465 7874 2d74 6f2d 5370  int3("Text-to-Sp
-00013f60: 6565 6368 2070 6c61 7466 6f72 6d20 6368  eech platform ch
-00013f70: 616e 6765 6420 746f 3a20 476f 6f67 6c65  anged to: Google
-00013f80: 2054 6578 742d 746f 2d53 7065 6563 6820   Text-to-Speech 
-00013f90: 2847 656e 6572 6963 2922 290a 2020 2020  (Generic)").    
-00013fa0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00013fb0: 6967 2e74 7473 506c 6174 666f 726d 203d  ig.ttsPlatform =
-00013fc0: 2022 676f 6f67 6c65 220a 2020 2020 2020   "google".      
-00013fd0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00013fe0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00013ff0: 2e73 6574 456c 6576 656e 6c61 6273 566f  .setElevenlabsVo
-00014000: 6963 6528 290a 2020 2020 2020 2020 656c  ice().        el
-00014010: 6966 2063 6f6e 6669 672e 7474 7350 6c61  if config.ttsPla
-00014020: 7466 6f72 6d20 3d3d 2022 6375 7374 6f6d  tform == "custom
-00014030: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-00014040: 656c 662e 6465 6669 6e65 5474 7343 6f6d  elf.defineTtsCom
-00014050: 6d61 6e64 2829 0a20 2020 2020 2020 2023  mand().        #
-00014060: 2073 6176 6520 636f 6e66 6967 730a 2020   save configs.  
-00014070: 2020 2020 2020 636f 6e66 6967 2e73 6176        config.sav
-00014080: 6543 6f6e 6669 6728 290a 0a20 2020 2064  eConfig()..    d
-00014090: 6566 2073 6574 566f 6963 6554 7970 696e  ef setVoiceTypin
-000140a0: 6743 6f6e 6669 6728 7365 6c66 293a 0a20  gConfig(self):. 
-000140b0: 2020 2020 2020 2076 6f69 6365 5479 7069         voiceTypi
-000140c0: 6e67 506c 6174 666f 726d 203d 2073 656c  ngPlatform = sel
-000140d0: 662e 6469 616c 6f67 732e 6765 7456 616c  f.dialogs.getVal
-000140e0: 6964 4f70 7469 6f6e 7328 0a20 2020 2020  idOptions(.     
-000140f0: 2020 2020 2020 206f 7074 696f 6e73 3d28         options=(
-00014100: 2267 6f6f 676c 6522 2c20 2267 6f6f 676c  "google", "googl
-00014110: 6563 6c6f 7564 222c 2022 7768 6973 7065  ecloud", "whispe
-00014120: 7222 292c 0a20 2020 2020 2020 2020 2020  r"),.           
-00014130: 2064 6573 6372 6970 7469 6f6e 733d 2822   descriptions=("
-00014140: 476f 6f67 6c65 2053 7065 6563 682d 746f  Google Speech-to
-00014150: 2d54 6578 7420 2847 656e 6572 6963 2920  -Text (Generic) 
-00014160: 5b6f 6e6c 696e 655d 222c 2022 476f 6f67  [online]", "Goog
-00014170: 6c65 2053 7065 6563 682d 746f 2d54 6578  le Speech-to-Tex
-00014180: 7420 2841 5049 2920 5b6f 6e6c 696e 655d  t (API) [online]
-00014190: 222c 2022 4f70 656e 4149 2057 6869 7370  ", "OpenAI Whisp
-000141a0: 6572 205b 6f66 666c 696e 653b 2073 6c6f  er [offline; slo
-000141b0: 7765 7220 7769 7468 206e 6f6e 2d45 6e67  wer with non-Eng
-000141c0: 6c69 7368 2076 6f69 6365 735d 2229 2c0a  lish voices]"),.
-000141d0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-000141e0: 653d 2256 6f69 6365 2054 7970 696e 6720  e="Voice Typing 
-000141f0: 436f 6e66 6967 7572 6174 696f 6e73 222c  Configurations",
-00014200: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00014210: 743d 2253 656c 6563 7420 6120 766f 6963  t="Select a voic
-00014220: 6520 7479 7069 6e67 2070 6c61 7466 6f72  e typing platfor
-00014230: 6d3a 222c 0a20 2020 2020 2020 2020 2020  m:",.           
-00014240: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
-00014250: 766f 6963 6554 7970 696e 6750 6c61 7466  voiceTypingPlatf
-00014260: 6f72 6d2c 0a20 2020 2020 2020 2029 0a20  orm,.        ). 
-00014270: 2020 2020 2020 2069 6620 766f 6963 6554         if voiceT
-00014280: 7970 696e 6750 6c61 7466 6f72 6d3a 0a20  ypingPlatform:. 
-00014290: 2020 2020 2020 2020 2020 2069 6620 766f             if vo
-000142a0: 6963 6554 7970 696e 6750 6c61 7466 6f72  iceTypingPlatfor
-000142b0: 6d20 3d3d 2022 676f 6f67 6c65 636c 6f75  m == "googleclou
-000142c0: 6422 2061 6e64 206e 6f74 2028 6f73 2e65  d" and not (os.e
-000142d0: 6e76 6972 6f6e 5b22 474f 4f47 4c45 5f41  nviron["GOOGLE_A
-000142e0: 5050 4c49 4341 5449 4f4e 5f43 5245 4445  PPLICATION_CREDE
-000142f0: 4e54 4941 4c53 225d 2061 6e64 2022 5370  NTIALS"] and "Sp
-00014300: 6565 6368 2d74 6f2d 5465 7874 2220 696e  eech-to-Text" in
-00014310: 2063 6f6e 6669 672e 656e 6162 6c65 6447   config.enabledG
-00014320: 6f6f 676c 6541 5049 7329 3a0a 2020 2020  oogleAPIs):.    
-00014330: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00014340: 7432 2822 476f 6f67 6c65 2043 6c6f 7564  t2("Google Cloud
-00014350: 2053 7065 6563 682d 746f 2d54 6578 7420   Speech-to-Text 
-00014360: 6665 6174 7572 6520 6973 206e 6f74 2065  feature is not e
-00014370: 6e61 626c 6564 2122 290a 2020 2020 2020  nabled!").      
-00014380: 2020 2020 2020 2020 2020 7072 696e 7433            print3
-00014390: 2822 5265 6164 3a20 6874 7470 733a 2f2f  ("Read: https://
-000143a0: 6769 7468 7562 2e63 6f6d 2f65 6c69 7261  github.com/elira
-000143b0: 6e77 6f6e 672f 6c65 746d 6564 6f69 742f  nwong/letmedoit/
-000143c0: 7769 6b69 2f47 6f6f 676c 652d 4150 492d  wiki/Google-API-
-000143d0: 5365 7475 7022 290a 2020 2020 2020 2020  Setup").        
-000143e0: 2020 2020 2020 2020 7072 696e 7433 2822          print3("
-000143f0: 566f 6963 6520 7479 7069 6e67 2070 6c61  Voice typing pla
-00014400: 7466 6f72 6d20 6368 616e 6765 6420 746f  tform changed to
-00014410: 3a20 476f 6f67 6c65 2053 7065 6563 682d  : Google Speech-
-00014420: 746f 2d54 6578 7420 2847 656e 6572 6963  to-Text (Generic
-00014430: 2922 290a 2020 2020 2020 2020 2020 2020  )").            
-00014440: 2020 2020 636f 6e66 6967 2e76 6f69 6365      config.voice
-00014450: 5479 7069 6e67 506c 6174 666f 726d 203d  TypingPlatform =
-00014460: 2022 676f 6f67 6c65 220a 2020 2020 2020   "google".      
-00014470: 2020 2020 2020 656c 6966 2076 6f69 6365        elif voice
-00014480: 5479 7069 6e67 506c 6174 666f 726d 203d  TypingPlatform =
-00014490: 3d20 2277 6869 7370 6572 2220 616e 6420  = "whisper" and 
-000144a0: 6e6f 7420 6973 436f 6d6d 616e 6449 6e73  not isCommandIns
-000144b0: 7461 6c6c 6564 2822 6666 6d70 6567 2229  talled("ffmpeg")
-000144c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000144d0: 2020 7072 696e 7432 2822 496e 7374 616c    print2("Instal
-000144e0: 6c20 2766 666d 7065 6727 2066 6972 7374  l 'ffmpeg' first
-000144f0: 2074 6f20 7573 6520 6f66 666c 696e 6520   to use offline 
-00014500: 6f70 656e 6169 2077 6869 7370 6572 206d  openai whisper m
-00014510: 6f64 656c 2122 290a 2020 2020 2020 2020  odel!").        
-00014520: 2020 2020 2020 2020 7072 696e 7433 2822          print3("
-00014530: 5265 6164 3a20 6874 7470 733a 2f2f 6769  Read: https://gi
-00014540: 7468 7562 2e63 6f6d 2f6f 7065 6e61 692f  thub.com/openai/
-00014550: 7768 6973 7065 7223 7365 7475 7022 290a  whisper#setup").
-00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 7072 696e 7433 2822 566f 6963 6520 7479  print3("Voice ty
-00014580: 7069 6e67 2070 6c61 7466 6f72 6d20 6368  ping platform ch
-00014590: 616e 6765 6420 746f 3a20 476f 6f67 6c65  anged to: Google
-000145a0: 2053 7065 6563 682d 746f 2d54 6578 7420   Speech-to-Text 
-000145b0: 2847 656e 6572 6963 2922 290a 2020 2020  (Generic)").    
-000145c0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000145d0: 6967 2e76 6f69 6365 5479 7069 6e67 506c  ig.voiceTypingPl
-000145e0: 6174 666f 726d 203d 2022 676f 6f67 6c65  atform = "google
-000145f0: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
-00014600: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014610: 2020 2020 636f 6e66 6967 2e76 6f69 6365      config.voice
-00014620: 5479 7069 6e67 506c 6174 666f 726d 203d  TypingPlatform =
-00014630: 2076 6f69 6365 5479 7069 6e67 506c 6174   voiceTypingPlat
-00014640: 666f 726d 0a20 2020 2020 2020 2023 206c  form.        # l
-00014650: 616e 6775 6167 650a 2020 2020 2020 2020  anguage.        
-00014660: 7365 6c66 2e73 6574 5370 6565 6368 546f  self.setSpeechTo
-00014670: 5465 7874 4c61 6e67 7561 6765 2829 0a20  TextLanguage(). 
-00014680: 2020 2020 2020 2023 2063 6f6e 6669 6775         # configu
-00014690: 7265 2063 6f6e 6669 672e 766f 6963 6554  re config.voiceT
-000146a0: 7970 696e 6741 646a 7573 7441 6d62 6965  ypingAdjustAmbie
-000146b0: 6e74 4e6f 6973 650a 2020 2020 2020 2020  ntNoise.        
-000146c0: 766f 6963 6554 7970 696e 6741 646a 7573  voiceTypingAdjus
-000146d0: 7441 6d62 6965 6e74 4e6f 6973 6520 3d20  tAmbientNoise = 
-000146e0: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
-000146f0: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
-00014700: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
-00014710: 733d 2822 5965 7322 2c20 224e 6f22 292c  s=("Yes", "No"),
-00014720: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00014730: 6372 6970 7469 6f6e 733d 2822 5965 7320  criptions=("Yes 
-00014740: 5b73 6c6f 7765 725d 222c 2022 4e6f 2229  [slower]", "No")
-00014750: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00014760: 746c 653d 2241 646a 7573 7420 416d 6269  tle="Adjust Ambi
-00014770: 656e 7420 4e6f 6973 6522 2c0a 2020 2020  ent Noise",.    
-00014780: 2020 2020 2020 2020 7465 7874 3d22 446f          text="Do
-00014790: 2079 6f75 2077 616e 7420 746f 2061 646a   you want to adj
-000147a0: 7573 7420 616d 6269 656e 7420 6e6f 6973  ust ambient nois
-000147b0: 653f 222c 0a20 2020 2020 2020 2020 2020  e?",.           
-000147c0: 2064 6566 6175 6c74 3d22 5965 7322 2069   default="Yes" i
-000147d0: 6620 636f 6e66 6967 2e76 6f69 6365 5479  f config.voiceTy
-000147e0: 7069 6e67 4164 6a75 7374 416d 6269 656e  pingAdjustAmbien
-000147f0: 744e 6f69 7365 2065 6c73 6520 224e 6f22  tNoise else "No"
-00014800: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-00014810: 2020 2020 6966 2076 6f69 6365 5479 7069      if voiceTypi
-00014820: 6e67 4164 6a75 7374 416d 6269 656e 744e  ngAdjustAmbientN
-00014830: 6f69 7365 3a0a 2020 2020 2020 2020 2020  oise:.          
-00014840: 2020 636f 6e66 6967 2e76 6f69 6365 5479    config.voiceTy
-00014850: 7069 6e67 4164 6a75 7374 416d 6269 656e  pingAdjustAmbien
-00014860: 744e 6f69 7365 203d 2054 7275 6520 6966  tNoise = True if
-00014870: 2076 6f69 6365 5479 7069 6e67 4164 6a75   voiceTypingAdju
-00014880: 7374 416d 6269 656e 744e 6f69 7365 203d  stAmbientNoise =
-00014890: 3d20 2259 6573 2220 656c 7365 2046 616c  = "Yes" else Fal
-000148a0: 7365 0a20 2020 2020 2020 2023 2061 7564  se.        # aud
-000148b0: 696f 206e 6f74 6966 6963 6174 696f 6e0a  io notification.
-000148c0: 2020 2020 2020 2020 766f 6963 6554 7970          voiceTyp
-000148d0: 696e 674e 6f74 6966 6963 6174 696f 6e20  ingNotification 
-000148e0: 3d20 7365 6c66 2e64 6961 6c6f 6773 2e67  = self.dialogs.g
-000148f0: 6574 5661 6c69 644f 7074 696f 6e73 280a  etValidOptions(.
-00014900: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00014910: 6f6e 733d 2822 5965 7322 2c20 224e 6f22  ons=("Yes", "No"
-00014920: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
-00014930: 6974 6c65 3d22 4175 6469 6f20 4e6f 7469  itle="Audio Noti
-00014940: 6669 6361 7469 6f6e 222c 0a20 2020 2020  fication",.     
-00014950: 2020 2020 2020 2074 6578 743d 2244 6f20         text="Do 
-00014960: 796f 7520 7761 6e74 2061 7564 696f 206e  you want audio n
-00014970: 6f74 6966 6963 6174 696f 6e20 7768 656e  otification when
-00014980: 2079 6f75 2075 7365 206d 6963 726f 7068   you use microph
-00014990: 6f6e 653f 222c 0a20 2020 2020 2020 2020  one?",.         
-000149a0: 2020 2064 6566 6175 6c74 3d22 5965 7322     default="Yes"
-000149b0: 2069 6620 636f 6e66 6967 2e76 6f69 6365   if config.voice
-000149c0: 5479 7069 6e67 4e6f 7469 6669 6361 7469  TypingNotificati
-000149d0: 6f6e 2065 6c73 6520 224e 6f22 2c0a 2020  on else "No",.  
-000149e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000149f0: 6966 2076 6f69 6365 5479 7069 6e67 4e6f  if voiceTypingNo
-00014a00: 7469 6669 6361 7469 6f6e 3a0a 2020 2020  tification:.    
-00014a10: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
-00014a20: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
-00014a30: 6361 7469 6f6e 203d 2054 7275 6520 6966  cation = True if
-00014a40: 2076 6f69 6365 5479 7069 6e67 4e6f 7469   voiceTypingNoti
-00014a50: 6669 6361 7469 6f6e 203d 3d20 2259 6573  fication == "Yes
-00014a60: 2220 656c 7365 2046 616c 7365 0a20 2020  " else False.   
-00014a70: 2020 2020 2023 2061 7574 6f20 636f 6d70       # auto comp
-00014a80: 6c65 7469 6f6e 3a20 766f 6963 6554 7970  letion: voiceTyp
-00014a90: 696e 6741 7574 6f43 6f6d 706c 6574 650a  ingAutoComplete.
-00014aa0: 2020 2020 2020 2020 766f 6963 6554 7970          voiceTyp
-00014ab0: 696e 6741 7574 6f43 6f6d 706c 6574 6520  ingAutoComplete 
-00014ac0: 3d20 7365 6c66 2e64 6961 6c6f 6773 2e67  = self.dialogs.g
-00014ad0: 6574 5661 6c69 644f 7074 696f 6e73 280a  etValidOptions(.
-00014ae0: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00014af0: 6f6e 733d 2822 5965 7322 2c20 224e 6f22  ons=("Yes", "No"
-00014b00: 292c 0a20 2020 2020 2020 2020 2020 2074  ),.            t
-00014b10: 6974 6c65 3d22 4175 6469 6f20 456e 7472  itle="Audio Entr
-00014b20: 7920 4175 746f 2043 6f6d 706c 6574 696f  y Auto Completio
-00014b30: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00014b40: 7465 7874 3d22 446f 2079 6f75 2077 616e  text="Do you wan
-00014b50: 7420 746f 2061 7574 6f6d 6174 6963 616c  t to automatical
-00014b60: 6c79 2063 6f6d 706c 6574 6520 796f 7572  ly complete your
-00014b70: 2065 6e74 7279 2077 6865 6e20 6d69 6372   entry when micr
-00014b80: 6f70 686f 6e65 2073 746f 7073 3f22 2c0a  ophone stops?",.
-00014b90: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-00014ba0: 756c 743d 2259 6573 2220 6966 2063 6f6e  ult="Yes" if con
-00014bb0: 6669 672e 766f 6963 6554 7970 696e 6741  fig.voiceTypingA
-00014bc0: 7574 6f43 6f6d 706c 6574 6520 656c 7365  utoComplete else
-00014bd0: 2022 4e6f 222c 0a20 2020 2020 2020 2029   "No",.        )
-00014be0: 0a20 2020 2020 2020 2069 6620 766f 6963  .        if voic
-00014bf0: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
-00014c00: 6574 653a 0a20 2020 2020 2020 2020 2020  ete:.           
-00014c10: 2063 6f6e 6669 672e 766f 6963 6554 7970   config.voiceTyp
-00014c20: 696e 6741 7574 6f43 6f6d 706c 6574 6520  ingAutoComplete 
-00014c30: 3d20 5472 7565 2069 6620 766f 6963 6554  = True if voiceT
-00014c40: 7970 696e 6741 7574 6f43 6f6d 706c 6574  ypingAutoComplet
-00014c50: 6520 3d3d 2022 5965 7322 2065 6c73 6520  e == "Yes" else 
-00014c60: 4661 6c73 650a 2020 2020 2020 2020 2320  False.        # 
-00014c70: 6e6f 7469 6679 0a20 2020 2020 2020 2070  notify.        p
-00014c80: 7269 6e74 2822 2229 0a20 2020 2020 2020  rint("").       
-00014c90: 2070 7269 6e74 3328 6622 566f 6963 6520   print3(f"Voice 
-00014ca0: 5479 7069 6e67 204d 6f64 656c 3a20 7b63  Typing Model: {c
-00014cb0: 6f6e 6669 672e 766f 6963 6554 7970 696e  onfig.voiceTypin
-00014cc0: 6750 6c61 7466 6f72 6d7d 2229 0a20 2020  gPlatform}").   
-00014cd0: 2020 2020 2070 7269 6e74 3328 6622 566f       print3(f"Vo
-00014ce0: 6963 6520 5479 7069 6e67 204c 616e 6775  ice Typing Langu
-00014cf0: 6167 653a 207b 636f 6e66 6967 2e76 6f69  age: {config.voi
-00014d00: 6365 5479 7069 6e67 4c61 6e67 7561 6765  ceTypingLanguage
-00014d10: 7d22 290a 2020 2020 2020 2020 7072 696e  }").        prin
-00014d20: 7433 2866 2241 6d62 6965 6e74 204e 6f69  t3(f"Ambient Noi
-00014d30: 7365 2041 646a 7573 746d 656e 743a 207b  se Adjustment: {
-00014d40: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
-00014d50: 6e67 4164 6a75 7374 416d 6269 656e 744e  ngAdjustAmbientN
-00014d60: 6f69 7365 7d22 290a 2020 2020 2020 2020  oise}").        
-00014d70: 7072 696e 7433 2866 2241 7564 696f 204e  print3(f"Audio N
-00014d80: 6f74 6966 6963 6174 696f 6e3a 207b 636f  otification: {co
-00014d90: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
-00014da0: 4e6f 7469 6669 6361 7469 6f6e 7d22 290a  Notification}").
-00014db0: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-00014dc0: 2241 7574 6f20 436f 6d70 6c65 7469 6f6e  "Auto Completion
-00014dd0: 3a20 7b63 6f6e 6669 672e 766f 6963 6554  : {config.voiceT
-00014de0: 7970 696e 6741 7574 6f43 6f6d 706c 6574  ypingAutoComplet
-00014df0: 657d 2229 0a20 2020 2020 2020 2023 2073  e}").        # s
-00014e00: 6176 6520 636f 6e66 6967 730a 2020 2020  ave configs.    
-00014e10: 2020 2020 636f 6e66 6967 2e73 6176 6543      config.saveC
-00014e20: 6f6e 6669 6728 290a 0a20 2020 2064 6566  onfig()..    def
-00014e30: 2073 6176 6543 6861 7428 7365 6c66 2c20   saveChat(self, 
-00014e40: 6d65 7373 6167 6573 293a 0a20 2020 2020  messages):.     
-00014e50: 2020 206d 6573 7361 6765 7343 6f70 7920     messagesCopy 
-00014e60: 3d20 636f 7079 2e64 6565 7063 6f70 7928  = copy.deepcopy(
-00014e70: 6d65 7373 6167 6573 290a 0a20 2020 2020  messages)..     
-00014e80: 2020 2069 6620 636f 6e66 6967 2e63 6f6e     if config.con
-00014e90: 7665 7273 6174 696f 6e53 7461 7274 6564  versationStarted
-00014ea0: 3a0a 2020 2020 2020 2020 2020 2020 7469  :.            ti
-00014eb0: 6d65 7374 616d 7020 3d20 6765 7443 7572  mestamp = getCur
-00014ec0: 7265 6e74 4461 7465 5469 6d65 2829 0a0a  rentDateTime()..
-00014ed0: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-00014ee0: 6173 6174 7472 2863 6f6e 6669 672c 2022  asattr(config, "
-00014ef0: 7361 7665 5f63 6861 745f 7265 636f 7264  save_chat_record
-00014f00: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00014f10: 2020 2020 2320 7768 656e 2070 6c75 6769      # when plugi
-00014f20: 6e20 2273 6176 6520 6368 6174 2072 6563  n "save chat rec
-00014f30: 6f72 6473 2220 6973 2065 6e61 626c 6564  ords" is enabled
-00014f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f50: 206d 6573 7361 6765 4c65 6e67 7468 203d   messageLength =
-00014f60: 206c 656e 286d 6573 7361 6765 7343 6f70   len(messagesCop
-00014f70: 7929 0a20 2020 2020 2020 2020 2020 2020  y).             
-00014f80: 2020 2066 6f72 206f 7264 6572 2c20 6920     for order, i 
-00014f90: 696e 2065 6e75 6d65 7261 7465 286d 6573  in enumerate(mes
-00014fa0: 7361 6765 7343 6f70 7929 3a0a 2020 2020  sagesCopy):.    
-00014fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fc0: 6973 4c61 7374 4974 656d 203d 2028 6f72  isLastItem = (or
-00014fd0: 6465 7220 3d3d 2028 6d65 7373 6167 654c  der == (messageL
-00014fe0: 656e 6774 6820 2d20 3129 290a 2020 2020  ength - 1)).    
-00014ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015000: 6966 2063 6f6e 6669 672e 6c6c 6d49 6e74  if config.llmInt
-00015010: 6572 6661 6365 2069 6e20 2822 6368 6174  erface in ("chat
-00015020: 6770 7422 2c20 226c 6574 6d65 646f 6974  gpt", "letmedoit
-00015030: 222c 2022 6772 6f71 2229 2061 6e64 206e  ", "groq") and n
-00015040: 6f74 2069 734c 6173 7449 7465 6d20 616e  ot isLastItem an
-00015050: 6420 692e 6765 7428 2272 6f6c 6522 2c20  d i.get("role", 
-00015060: 2222 2920 3d3d 2022 7573 6572 2220 616e  "") == "user" an
-00015070: 6420 2266 756e 6374 696f 6e5f 6361 6c6c  d "function_call
-00015080: 2220 696e 206d 6573 7361 6765 7343 6f70  " in messagesCop
-00015090: 795b 6f72 6465 722b 315d 3a0a 2020 2020  y[order+1]:.    
-000150a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150b0: 2020 2020 695b 2274 6f6f 6c22 5d20 3d20      i["tool"] = 
-000150c0: 6d65 7373 6167 6573 436f 7079 5b6f 7264  messagesCopy[ord
-000150d0: 6572 2b31 5d5b 2266 756e 6374 696f 6e5f  er+1]["function_
-000150e0: 6361 6c6c 225d 2e67 6574 2822 6e61 6d65  call"].get("name
-000150f0: 222c 2022 2229 0a20 2020 2020 2020 2020  ", "").         
-00015100: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00015110: 672e 7361 7665 5f63 6861 745f 7265 636f  g.save_chat_reco
-00015120: 7264 2874 696d 6573 7461 6d70 2c20 6f72  rd(timestamp, or
-00015130: 6465 722c 2069 290a 0a20 2020 2020 2020  der, i)..       
-00015140: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00015150: 2020 2020 2020 2020 2020 666f 6c64 6572            folder
-00015160: 5061 7468 203d 206f 732e 7061 7468 2e6a  Path = os.path.j
-00015170: 6f69 6e28 636f 6e66 6967 2e6c 6f63 616c  oin(config.local
-00015180: 5374 6f72 6167 652c 2022 6368 6174 7322  Storage, "chats"
-00015190: 2c20 7265 2e73 7562 2822 5e28 5b30 2d39  , re.sub("^([0-9
-000151a0: 5d2b 3f5c 2d5b 302d 395d 2b3f 295c 2d2e  ]+?\-[0-9]+?)\-.
-000151b0: 2a3f 2422 2c20 7222 5c31 222c 2074 696d  *?$", r"\1", tim
-000151c0: 6573 7461 6d70 2929 0a20 2020 2020 2020  estamp)).       
-000151d0: 2020 2020 2020 2020 2050 6174 6828 666f           Path(fo
-000151e0: 6c64 6572 5061 7468 292e 6d6b 6469 7228  lderPath).mkdir(
-000151f0: 7061 7265 6e74 733d 5472 7565 2c20 6578  parents=True, ex
-00015200: 6973 745f 6f6b 3d54 7275 6529 0a20 2020  ist_ok=True).   
-00015210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015220: 6f73 2e70 6174 682e 6973 6469 7228 666f  os.path.isdir(fo
-00015230: 6c64 6572 5061 7468 293a 0a20 2020 2020  lderPath):.     
-00015240: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00015250: 6861 7446 696c 6520 3d20 6f73 2e70 6174  hatFile = os.pat
-00015260: 682e 6a6f 696e 2866 6f6c 6465 7250 6174  h.join(folderPat
-00015270: 682c 2066 227b 7469 6d65 7374 616d 707d  h, f"{timestamp}
-00015280: 2e74 7874 2229 0a20 2020 2020 2020 2020  .txt").         
-00015290: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-000152a0: 6f70 656e 2863 6861 7446 696c 652c 2022  open(chatFile, "
-000152b0: 7722 2c20 656e 636f 6469 6e67 3d22 7574  w", encoding="ut
-000152c0: 662d 3822 2920 6173 2066 696c 654f 626a  f-8") as fileObj
-000152d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000152e0: 2020 2020 2020 2020 2020 6669 6c65 4f62            fileOb
-000152f0: 6a2e 7772 6974 6528 7070 7269 6e74 2e70  j.write(pprint.p
-00015300: 666f 726d 6174 286d 6573 7361 6765 7343  format(messagesC
-00015310: 6f70 7929 290a 2020 2020 2020 2020 2020  opy)).          
-00015320: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00015330: 2020 2020 2020 2020 2020 7072 696e 7432            print2
-00015340: 2822 4661 696c 6564 2074 6f20 7361 7665  ("Failed to save
-00015350: 2063 6861 7421 5c6e 2229 0a20 2020 2020   chat!\n").     
-00015360: 2020 2020 2020 2020 2020 2073 686f 7745             showE
-00015370: 7272 6f72 7328 290a 0a20 2020 2064 6566  rrors()..    def
-00015380: 2065 7870 6f72 7443 6861 7428 7365 6c66   exportChat(self
-00015390: 2c20 6d65 7373 6167 6573 2c20 6f70 656e  , messages, open
-000153a0: 4669 6c65 3d54 7275 6529 3a0a 2020 2020  File=True):.    
-000153b0: 2020 2020 6966 2063 6f6e 6669 672e 636f      if config.co
-000153c0: 6e76 6572 7361 7469 6f6e 5374 6172 7465  nversationStarte
-000153d0: 643a 0a20 2020 2020 2020 2020 2020 2070  d:.            p
-000153e0: 6c61 696e 5465 7874 203d 2022 220a 2020  lainText = "".  
-000153f0: 2020 2020 2020 2020 2020 7469 6d65 7374            timest
-00015400: 616d 7020 3d20 6765 7443 7572 7265 6e74  amp = getCurrent
-00015410: 4461 7465 5469 6d65 2829 0a0a 2020 2020  DateTime()..    
-00015420: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00015430: 206d 6573 7361 6765 733a 0a20 2020 2020   messages:.     
-00015440: 2020 2020 2020 2020 2020 2069 6620 695b             if i[
-00015450: 2272 6f6c 6522 5d20 3d3d 2022 7573 6572  "role"] == "user
-00015460: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00015470: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00015480: 2069 5b22 636f 6e74 656e 7422 5d0a 2020   i["content"].  
-00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154a0: 2020 706c 6169 6e54 6578 7420 2b3d 2066    plainText += f
-000154b0: 223e 3e3e 207b 636f 6e74 656e 747d 220a  ">>> {content}".
-000154c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000154d0: 6966 2069 5b22 726f 6c65 225d 203d 3d20  if i["role"] == 
-000154e0: 2266 756e 6374 696f 6e22 3a0a 2020 2020  "function":.    
-000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015500: 6966 2070 6c61 696e 5465 7874 3a0a 2020  if plainText:.  
-00015510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015520: 2020 2020 2020 706c 6169 6e54 6578 7420        plainText 
-00015530: 2b3d 2022 5c6e 5c6e 220a 2020 2020 2020  += "\n\n".      
-00015540: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00015550: 6d65 203d 2069 5b22 6e61 6d65 225d 0a20  me = i["name"]. 
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2020 2070 6c61 696e 5465 7874 202b 3d20     plainText += 
-00015580: 6622 6060 605c 6e7b 6e61 6d65 7d5c 6e60  f"```\n{name}\n`
-00015590: 6060 220a 2020 2020 2020 2020 2020 2020  ``".            
-000155a0: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-000155b0: 3d20 695b 2263 6f6e 7465 6e74 225d 0a20  = i["content"]. 
-000155c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155d0: 2020 2070 6c61 696e 5465 7874 202b 3d20     plainText += 
-000155e0: 6622 5c6e 5c6e 7b63 6f6e 7465 6e74 7d5c  f"\n\n{content}\
-000155f0: 6e5c 6e22 0a20 2020 2020 2020 2020 2020  n\n".           
-00015600: 2020 2020 2065 6c69 6620 695b 2272 6f6c       elif i["rol
-00015610: 6522 5d20 3d3d 2022 6173 7369 7374 616e  e"] == "assistan
-00015620: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
-00015630: 2020 2020 2020 2020 636f 6e74 656e 7420          content 
-00015640: 3d20 695b 2263 6f6e 7465 6e74 225d 0a20  = i["content"]. 
-00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015660: 2020 2069 6620 636f 6e74 656e 7420 6973     if content is
-00015670: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00015680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015690: 2020 2069 6620 706c 6169 6e54 6578 743a     if plainText:
-000156a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156b0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000156c0: 696e 5465 7874 202b 3d20 225c 6e5c 6e22  inText += "\n\n"
-000156d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156e0: 2020 2020 2020 2020 2070 6c61 696e 5465           plainTe
-000156f0: 7874 202b 3d20 6622 7b63 6f6e 7465 6e74  xt += f"{content
-00015700: 7d5c 6e5c 6e22 0a20 2020 2020 2020 2020  }\n\n".         
-00015710: 2020 2070 6c61 696e 5465 7874 203d 2070     plainText = p
-00015720: 6c61 696e 5465 7874 2e73 7472 6970 2829  lainText.strip()
-00015730: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00015740: 636f 6e66 6967 2e74 6572 6d69 6e61 6c45  config.terminalE
-00015750: 6e61 626c 6554 6572 6d75 7841 5049 3a0a  nableTermuxAPI:.
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 7079 646f 632e 7069 7065 7061 6765 7228  pydoc.pipepager(
-00015780: 706c 6169 6e54 6578 742c 2063 6d64 3d22  plainText, cmd="
-00015790: 7465 726d 7578 2d73 6861 7265 202d 6120  termux-share -a 
-000157a0: 7365 6e64 2229 0a20 2020 2020 2020 2020  send").         
-000157b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000157c0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-000157d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157e0: 2020 666f 6c64 6572 5061 7468 203d 206f    folderPath = o
-000157f0: 732e 7061 7468 2e6a 6f69 6e28 636f 6e66  s.path.join(conf
-00015800: 6967 2e6c 6f63 616c 5374 6f72 6167 652c  ig.localStorage,
-00015810: 2022 6368 6174 7322 2c20 2265 7870 6f72   "chats", "expor
-00015820: 7422 290a 2020 2020 2020 2020 2020 2020  t").            
-00015830: 2020 2020 2020 2020 5061 7468 2866 6f6c          Path(fol
-00015840: 6465 7250 6174 6829 2e6d 6b64 6972 2870  derPath).mkdir(p
-00015850: 6172 656e 7473 3d54 7275 652c 2065 7869  arents=True, exi
-00015860: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
-00015870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015880: 6966 206f 732e 7061 7468 2e69 7364 6972  if os.path.isdir
-00015890: 2866 6f6c 6465 7250 6174 6829 3a0a 2020  (folderPath):.  
-000158a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158b0: 2020 2020 2020 6368 6174 4669 6c65 203d        chatFile =
-000158c0: 206f 732e 7061 7468 2e6a 6f69 6e28 666f   os.path.join(fo
-000158d0: 6c64 6572 5061 7468 2c20 6622 7b74 696d  lderPath, f"{tim
-000158e0: 6573 7461 6d70 7d2e 7478 7422 290a 2020  estamp}.txt").  
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015900: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00015910: 6368 6174 4669 6c65 2c20 2277 222c 2065  chatFile, "w", e
-00015920: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-00015930: 2061 7320 6669 6c65 4f62 6a3a 0a20 2020   as fileObj:.   
-00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015950: 2020 2020 2020 2020 2066 696c 654f 626a           fileObj
-00015960: 2e77 7269 7465 2870 6c61 696e 5465 7874  .write(plainText
-00015970: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015980: 2020 2020 2020 2020 2020 6966 206f 7065            if ope
-00015990: 6e46 696c 6520 616e 6420 6f73 2e70 6174  nFile and os.pat
-000159a0: 682e 6973 6669 6c65 2863 6861 7446 696c  h.isfile(chatFil
-000159b0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-000159c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159d0: 6f73 2e73 7973 7465 6d28 6627 2727 7b63  os.system(f'''{c
-000159e0: 6f6e 6669 672e 6f70 656e 7d20 227b 6368  onfig.open} "{ch
-000159f0: 6174 4669 6c65 7d22 2727 2729 0a20 2020  atFile}"''').   
-00015a00: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-00015a10: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-00015a20: 2020 2020 2020 2020 2070 7269 6e74 3228           print2(
-00015a30: 2246 6169 6c65 6420 746f 2073 6176 6520  "Failed to save 
-00015a40: 6368 6174 215c 6e22 290a 2020 2020 2020  chat!\n").      
-00015a50: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00015a60: 6f77 4572 726f 7273 2829 0a0a 2020 2020  owErrors()..    
-00015a70: 6465 6620 7275 6e49 6e73 7472 7563 7469  def runInstructi
-00015a80: 6f6e 2873 656c 6629 3a0a 2020 2020 2020  on(self):.      
-00015a90: 2020 696e 7374 7275 6374 696f 6e73 203d    instructions =
-00015aa0: 206c 6973 7428 636f 6e66 6967 2e70 7265   list(config.pre
-00015ab0: 6465 6669 6e65 6449 6e73 7472 7563 7469  definedInstructi
-00015ac0: 6f6e 732e 6b65 7973 2829 290a 2020 2020  ons.keys()).    
-00015ad0: 2020 2020 696e 7374 7275 6374 696f 6e20      instruction 
-00015ae0: 3d20 7365 6c66 2e64 6961 6c6f 6773 2e67  = self.dialogs.g
-00015af0: 6574 5661 6c69 644f 7074 696f 6e73 280a  etValidOptions(.
-00015b00: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
-00015b10: 6f6e 733d 696e 7374 7275 6374 696f 6e73  ons=instructions
-00015b20: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00015b30: 746c 653d 2250 7265 6465 6669 6e65 6420  tle="Predefined 
-00015b40: 496e 7374 7275 6374 696f 6e73 222c 0a20  Instructions",. 
-00015b50: 2020 2020 2020 2020 2020 2074 6578 743d             text=
-00015b60: 2253 656c 6563 7420 616e 2069 6e73 7472  "Select an instr
-00015b70: 7563 7469 6f6e 3a22 2c0a 2020 2020 2020  uction:",.      
-00015b80: 2020 290a 2020 2020 2020 2020 6966 2069    ).        if i
-00015b90: 6e73 7472 7563 7469 6f6e 3a0a 2020 2020  nstruction:.    
-00015ba0: 2020 2020 2020 2020 636f 6e66 6967 2e64          config.d
-00015bb0: 6566 6175 6c74 456e 7472 7920 3d20 636f  efaultEntry = co
-00015bc0: 6e66 6967 2e70 7265 6465 6669 6e65 6449  nfig.predefinedI
-00015bd0: 6e73 7472 7563 7469 6f6e 735b 696e 7374  nstructions[inst
-00015be0: 7275 6374 696f 6e5d 0a20 2020 2020 2020  ruction].       
-00015bf0: 2020 2020 2063 6f6e 6669 672e 6163 6365       config.acce
-00015c00: 7074 5f64 6566 6175 6c74 203d 2054 7275  pt_default = Tru
-00015c10: 650a 0a20 2020 2064 6566 2063 6861 6e67  e..    def chang
-00015c20: 6543 6f6e 7465 7874 2873 656c 6629 3a0a  eContext(self):.
-00015c30: 2020 2020 2020 2020 636f 6e74 6578 7473          contexts
-00015c40: 203d 206c 6973 7428 636f 6e66 6967 2e70   = list(config.p
-00015c50: 7265 6465 6669 6e65 6443 6f6e 7465 7874  redefinedContext
-00015c60: 732e 6b65 7973 2829 290a 2020 2020 2020  s.keys()).      
-00015c70: 2020 7072 6564 6566 696e 6564 436f 6e74    predefinedCont
-00015c80: 6578 7420 3d20 7365 6c66 2e64 6961 6c6f  ext = self.dialo
-00015c90: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
-00015ca0: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
-00015cb0: 6f70 7469 6f6e 733d 636f 6e74 6578 7473  options=contexts
-00015cc0: 2c0a 2020 2020 2020 2020 2020 2020 7469  ,.            ti
-00015cd0: 746c 653d 2250 7265 6465 6669 6e65 6420  tle="Predefined 
-00015ce0: 436f 6e74 6578 7473 222c 0a20 2020 2020  Contexts",.     
-00015cf0: 2020 2020 2020 2064 6566 6175 6c74 3d63         default=c
-00015d00: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
-00015d10: 436f 6e74 6578 742c 0a20 2020 2020 2020  Context,.       
-00015d20: 2020 2020 2074 6578 743d 2253 656c 6563       text="Selec
-00015d30: 7420 6120 636f 6e74 6578 743a 222c 0a20  t a context:",. 
-00015d40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00015d50: 2069 6620 7072 6564 6566 696e 6564 436f   if predefinedCo
-00015d60: 6e74 6578 743a 0a20 2020 2020 2020 2020  ntext:.         
-00015d70: 2020 2063 6f6e 6669 672e 7072 6564 6566     config.predef
-00015d80: 696e 6564 436f 6e74 6578 7420 3d20 7072  inedContext = pr
-00015d90: 6564 6566 696e 6564 436f 6e74 6578 740a  edefinedContext.
-00015da0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00015db0: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
-00015dc0: 436f 6e74 6578 7420 3d3d 2022 5b63 7573  Context == "[cus
-00015dd0: 746f 6d5d 223a 0a20 2020 2020 2020 2020  tom]":.         
-00015de0: 2020 2020 2020 2070 7269 6e74 3128 2245         print1("E
-00015df0: 6469 7420 6375 7374 6f6d 2063 6f6e 7465  dit custom conte
-00015e00: 7874 2062 656c 6f77 3a22 290a 2020 2020  xt below:").    
-00015e10: 2020 2020 2020 2020 2020 2020 6375 7374              cust
-00015e20: 6f6d 436f 6e74 6578 7420 3d20 7365 6c66  omContext = self
-00015e30: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
-00015e40: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
-00015e50: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
-00015e60: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
-00015e70: 6f6e 6669 672e 6375 7374 6f6d 5072 6564  onfig.customPred
-00015e80: 6566 696e 6564 436f 6e74 6578 7429 0a20  efinedContext). 
-00015e90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015ea0: 6620 6375 7374 6f6d 436f 6e74 6578 7420  f customContext 
-00015eb0: 616e 6420 6e6f 7420 6375 7374 6f6d 436f  and not customCo
-00015ec0: 6e74 6578 742e 7374 7269 7028 292e 6c6f  ntext.strip().lo
-00015ed0: 7765 7228 2920 3d3d 2063 6f6e 6669 672e  wer() == config.
-00015ee0: 6578 6974 5f65 6e74 7279 3a0a 2020 2020  exit_entry:.    
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f00: 636f 6e66 6967 2e63 7573 746f 6d50 7265  config.customPre
-00015f10: 6465 6669 6e65 6443 6f6e 7465 7874 203d  definedContext =
-00015f20: 2063 7573 746f 6d43 6f6e 7465 7874 2e73   customContext.s
-00015f30: 7472 6970 2829 0a20 2020 2020 2020 2065  trip().        e
-00015f40: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00015f50: 2023 2061 2077 6179 2074 6f20 7175 6963   # a way to quic
-00015f60: 6b6c 7920 636c 6561 6e20 7570 2063 6f6e  kly clean up con
-00015f70: 7465 7874 0a20 2020 2020 2020 2020 2020  text.           
-00015f80: 2063 6f6e 6669 672e 7072 6564 6566 696e   config.predefin
-00015f90: 6564 436f 6e74 6578 7420 3d20 225b 6e6f  edContext = "[no
-00015fa0: 6e65 5d22 0a20 2020 2020 2020 2063 6f6e  ne]".        con
-00015fb0: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
-00015fc0: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
-00015fd0: 6f77 4375 7272 656e 7443 6f6e 7465 7874  owCurrentContext
-00015fe0: 2829 0a0a 2020 2020 6465 6620 6765 7444  ()..    def getD
-00015ff0: 6972 6563 746f 7279 4c69 7374 2873 656c  irectoryList(sel
-00016000: 6629 3a0a 2020 2020 2020 2020 6469 7265  f):.        dire
-00016010: 6374 6f72 794c 6973 7420 3d20 5b5d 0a20  ctoryList = []. 
-00016020: 2020 2020 2020 2066 6f72 2066 2069 6e20         for f in 
-00016030: 6f73 2e6c 6973 7464 6972 2827 2e27 293a  os.listdir('.'):
-00016040: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00016050: 6f73 2e70 6174 682e 6973 6469 7228 6629  os.path.isdir(f)
-00016060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00016070: 2020 7365 7061 7261 746f 7220 3d20 225c    separator = "\
-00016080: 5c22 2069 6620 636f 6e66 6967 2e74 6869  \" if config.thi
-00016090: 7350 6c61 7466 6f72 6d20 3d3d 2022 5769  sPlatform == "Wi
-000160a0: 6e64 6f77 7322 2065 6c73 6520 222f 220a  ndows" else "/".
-000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000160c0: 6469 7265 6374 6f72 794c 6973 742e 6170  directoryList.ap
-000160d0: 7065 6e64 2866 227b 667d 7b73 6570 6172  pend(f"{f}{separ
-000160e0: 6174 6f72 7d22 290a 2020 2020 2020 2020  ator}").        
-000160f0: 2020 2020 656c 6966 206f 732e 7061 7468      elif os.path
-00016100: 2e69 7366 696c 6528 6629 3a0a 2020 2020  .isfile(f):.    
-00016110: 2020 2020 2020 2020 2020 2020 6469 7265              dire
-00016120: 6374 6f72 794c 6973 742e 6170 7065 6e64  ctoryList.append
-00016130: 2866 290a 2020 2020 2020 2020 7265 7475  (f).        retu
-00016140: 726e 2064 6972 6563 746f 7279 4c69 7374  rn directoryList
-00016150: 0a0a 2020 2020 6465 6620 7368 6f77 4c6f  ..    def showLo
-00016160: 676f 2873 656c 6629 3a0a 2020 2020 2020  go(self):.      
-00016170: 2020 6170 704e 616d 6520 3d20 636f 6e66    appName = conf
-00016180: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
-00016190: 616d 652e 7370 6c69 7428 295b 305d 2e75  ame.split()[0].u
-000161a0: 7070 6572 2829 0a20 2020 2020 2020 2074  pper().        t
-000161b0: 6572 6d69 6e61 6c5f 7769 6474 6820 3d20  erminal_width = 
-000161c0: 7368 7574 696c 2e67 6574 5f74 6572 6d69  shutil.get_termi
-000161d0: 6e61 6c5f 7369 7a65 2829 2e63 6f6c 756d  nal_size().colum
-000161e0: 6e73 0a20 2020 2020 2020 2074 7279 3a0a  ns.        try:.
-000161f0: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-00016200: 2061 7274 2069 6d70 6f72 7420 7465 7874   art import text
-00016210: 3261 7274 0a20 2020 2020 2020 2020 2020  2art.           
-00016220: 2069 6620 7465 726d 696e 616c 5f77 6964   if terminal_wid
-00016230: 7468 203e 3d20 3332 3a0a 2020 2020 2020  th >= 32:.      
-00016240: 2020 2020 2020 2020 2020 6c6f 676f 203d            logo =
-00016250: 2074 6578 7432 6172 7428 6170 704e 616d   text2art(appNam
-00016260: 652c 2066 6f6e 743d 2263 7962 6572 6d65  e, font="cyberme
-00016270: 6475 6d22 290a 2020 2020 2020 2020 2020  dum").          
-00016280: 2020 656c 6966 2074 6572 6d69 6e61 6c5f    elif terminal_
-00016290: 7769 6474 6820 3e3d 2032 303a 0a20 2020  width >= 20:.   
-000162a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000162b0: 6f20 3d20 7465 7874 3261 7274 2822 2022  o = text2art(" "
-000162c0: 2e6a 6f69 6e28 6170 704e 616d 6529 202b  .join(appName) +
-000162d0: 2022 2022 2c20 666f 6e74 3d22 7768 6974   " ", font="whit
-000162e0: 655f 6275 6262 6c65 2229 0a20 2020 2020  e_bubble").     
-000162f0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00016300: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00016310: 6f20 3d20 636f 6e66 6967 2e66 7265 6547  o = config.freeG
-00016320: 656e 6975 7341 494e 616d 650a 2020 2020  eniusAIName.    
-00016330: 2020 2020 2020 2020 6c6f 676f 203d 206c          logo = l
-00016340: 6f67 6f5b 3a2d 315d 2023 2072 656d 6f76  ogo[:-1] # remov
-00016350: 6520 7468 6520 6c69 6e65 6272 6561 6b20  e the linebreak 
-00016360: 6174 2074 6865 2065 6e64 0a20 2020 2020  at the end.     
-00016370: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-00016380: 2020 2020 2020 206c 6f67 6f20 3d20 636f         logo = co
-00016390: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
-000163a0: 494e 616d 650a 2020 2020 2020 2020 7072  IName.        pr
-000163b0: 696e 745f 666f 726d 6174 7465 645f 7465  int_formatted_te
-000163c0: 7874 2848 544d 4c28 6622 3c7b 636f 6e66  xt(HTML(f"<{conf
-000163d0: 6967 2e74 6572 6d69 6e61 6c43 6f6d 6d61  ig.terminalComma
-000163e0: 6e64 456e 7472 7943 6f6c 6f72 327d 3e7b  ndEntryColor2}>{
-000163f0: 6c6f 676f 7d3c 2f7b 636f 6e66 6967 2e74  logo}</{config.t
-00016400: 6572 6d69 6e61 6c43 6f6d 6d61 6e64 456e  erminalCommandEn
-00016410: 7472 7943 6f6c 6f72 327d 3e22 2929 0a0a  tryColor2}>"))..
-00016420: 2020 2020 6465 6620 7275 6e50 7974 686f      def runPytho
-00016430: 6e53 6372 6970 7428 7365 6c66 2c20 7363  nScript(self, sc
-00016440: 7269 7074 293a 0a20 2020 2020 2020 2073  ript):.        s
-00016450: 6372 6970 7420 3d20 7363 7269 7074 2e73  cript = script.s
-00016460: 7472 6970 2829 5b33 3a2d 335d 0a20 2020  trip()[3:-3].   
-00016470: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00016480: 2020 2020 2020 6578 6563 2873 6372 6970        exec(scrip
-00016490: 742c 2067 6c6f 6261 6c73 2829 290a 2020  t, globals()).  
-000164a0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-000164b0: 2020 2020 2020 2020 2020 7472 6163 6520            trace 
-000164c0: 3d20 7472 6163 6562 6163 6b2e 666f 726d  = traceback.form
-000164d0: 6174 5f65 7863 2829 0a20 2020 2020 2020  at_exc().       
-000164e0: 2020 2020 2070 7269 6e74 2874 7261 6365       print(trace
-000164f0: 2069 6620 636f 6e66 6967 2e64 6576 656c   if config.devel
-00016500: 6f70 6572 2065 6c73 6520 2245 7272 6f72  oper else "Error
-00016510: 2065 6e63 6f75 6e74 6572 6564 2122 290a   encountered!").
-00016520: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016530: 7431 2863 6f6e 6669 672e 6469 7669 6465  t1(config.divide
-00016540: 7229 0a20 2020 2020 2020 2020 2020 2069  r).            i
-00016550: 6620 636f 6e66 6967 2e6d 6178 5f63 6f6e  f config.max_con
-00016560: 7365 6375 7469 7665 5f61 7574 6f5f 636f  secutive_auto_co
-00016570: 7272 6563 7469 6f6e 203e 2030 3a0a 2020  rrection > 0:.  
-00016580: 2020 2020 2020 2020 2020 2020 2020 4361                Ca
-00016590: 6c6c 4c4c 4d2e 6175 746f 436f 7272 6563  llLLM.autoCorrec
-000165a0: 7450 7974 686f 6e43 6f64 6528 7363 7269  tPythonCode(scri
-000165b0: 7074 2c20 7472 6163 6529 0a0a 2020 2020  pt, trace)..    
-000165c0: 6465 6620 7374 6172 7443 6861 7473 2873  def startChats(s
-000165d0: 656c 6629 3a0a 2020 2020 2020 2020 746f  elf):.        to
-000165e0: 6b65 6e56 616c 6964 6174 6f72 203d 2054  kenValidator = T
-000165f0: 6f6b 656e 5661 6c69 6461 746f 7228 290a  okenValidator().
-00016600: 2020 2020 2020 2020 6465 6620 6765 7444          def getD
-00016610: 796e 616d 6963 546f 6f6c 4261 7228 293a  ynamicToolBar():
-00016620: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016630: 7572 6e20 636f 6e66 6967 2e64 796e 616d  urn config.dynam
-00016640: 6963 546f 6f6c 4261 7254 6578 740a 2020  icToolBarText.  
-00016650: 2020 2020 2020 6465 6620 7374 6172 7443        def startC
-00016660: 6861 7428 293a 0a20 2020 2020 2020 2020  hat():.         
-00016670: 2020 2063 6c65 6172 2829 0a20 2020 2020     clear().     
-00016680: 2020 2020 2020 2070 7269 6e74 3128 7365         print1(se
-00016690: 6c66 2e64 6976 6964 6572 290a 2020 2020  lf.divider).    
-000166a0: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-000166b0: 774c 6f67 6f28 290a 2020 2020 2020 2020  wLogo().        
-000166c0: 2020 2020 7365 6c66 2e73 686f 7743 7572      self.showCur
-000166d0: 7265 6e74 436f 6e74 6578 7428 290a 2020  rentContext().  
-000166e0: 2020 2020 2020 2020 2020 2320 676f 2074            # go t
-000166f0: 6f20 7374 6172 7475 7020 6469 7265 6374  o startup direct
-00016700: 6f72 790a 2020 2020 2020 2020 2020 2020  ory.            
-00016710: 7374 6f72 6167 6564 6972 6563 746f 7279  storagedirectory
-00016720: 203d 2063 6f6e 6669 672e 6c6f 6361 6c53   = config.localS
-00016730: 746f 7261 6765 0a20 2020 2020 2020 2020  torage.         
-00016740: 2020 206f 732e 6368 6469 7228 7374 6f72     os.chdir(stor
-00016750: 6167 6564 6972 6563 746f 7279 290a 2020  agedirectory).  
-00016760: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00016770: 6573 203d 2043 616c 6c4c 4c4d 2e72 6573  es = CallLLM.res
-00016780: 6574 4d65 7373 6167 6573 2829 0a20 2020  etMessages().   
-00016790: 2020 2020 2020 2020 2023 7072 696e 7431           #print1
-000167a0: 2866 2273 7461 7274 7570 2064 6972 6563  (f"startup direc
-000167b0: 746f 7279 3a5c 6e7b 7374 6f72 6167 6564  tory:\n{storaged
-000167c0: 6972 6563 746f 7279 7d22 290a 2020 2020  irectory}").    
-000167d0: 2020 2020 2020 2020 7072 696e 745f 666f          print_fo
-000167e0: 726d 6174 7465 645f 7465 7874 2848 544d  rmatted_text(HTM
-000167f0: 4c28 6622 3c7b 636f 6e66 6967 2e74 6572  L(f"<{config.ter
-00016800: 6d69 6e61 6c50 726f 6d70 7449 6e64 6963  minalPromptIndic
-00016810: 6174 6f72 436f 6c6f 7232 7d3e 4469 7265  atorColor2}>Dire
-00016820: 6374 6f72 793a 3c2f 7b63 6f6e 6669 672e  ctory:</{config.
-00016830: 7465 726d 696e 616c 5072 6f6d 7074 496e  terminalPromptIn
-00016840: 6469 6361 746f 7243 6f6c 6f72 327d 3e20  dicatorColor2}> 
-00016850: 7b73 746f 7261 6765 6469 7265 6374 6f72  {storagedirector
-00016860: 797d 2229 290a 2020 2020 2020 2020 2020  y}")).          
-00016870: 2020 7072 696e 7431 2873 656c 662e 6469    print1(self.di
-00016880: 7669 6465 7229 0a0a 2020 2020 2020 2020  vider)..        
-00016890: 2020 2020 636f 6e66 6967 2e63 6f6e 7665      config.conve
-000168a0: 7273 6174 696f 6e53 7461 7274 6564 203d  rsationStarted =
-000168b0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-000168c0: 2020 2072 6574 7572 6e20 2873 746f 7261     return (stora
-000168d0: 6765 6469 7265 6374 6f72 792c 206d 6573  gedirectory, mes
-000168e0: 7361 6765 7329 0a20 2020 2020 2020 2073  sages).        s
-000168f0: 746f 7261 6765 6469 7265 6374 6f72 792c  toragedirectory,
-00016900: 2063 6f6e 6669 672e 6375 7272 656e 744d   config.currentM
-00016910: 6573 7361 6765 7320 3d20 7374 6172 7443  essages = startC
-00016920: 6861 7428 290a 2020 2020 2020 2020 636f  hat().        co
-00016930: 6e66 6967 2e6d 756c 7469 6c69 6e65 496e  nfig.multilineIn
-00016940: 7075 7420 3d20 4661 6c73 650a 2020 2020  put = False.    
-00016950: 2020 2020 6665 6174 7572 6573 4c6f 7765      featuresLowe
-00016960: 7220 3d20 6c69 7374 2873 656c 662e 6163  r = list(self.ac
-00016970: 7469 6f6e 732e 6b65 7973 2829 2920 2b20  tions.keys()) + 
-00016980: 5b22 2e2e 2e22 5d0a 2020 2020 2020 2020  ["..."].        
-00016990: 2320 696e 7075 7420 7375 6767 6573 7469  # input suggesti
-000169a0: 6f6e 730a 2020 2020 2020 2020 636f 6e66  ons.        conf
-000169b0: 6967 2e69 6e70 7574 5375 6767 6573 7469  ig.inputSuggesti
-000169c0: 6f6e 7320 2b3d 2066 6561 7475 7265 734c  ons += featuresL
-000169d0: 6f77 6572 0a20 2020 2020 2020 2063 6f6d  ower.        com
-000169e0: 706c 6574 6572 203d 2046 757a 7a79 436f  pleter = FuzzyCo
-000169f0: 6d70 6c65 7465 7228 576f 7264 436f 6d70  mpleter(WordComp
-00016a00: 6c65 7465 7228 636f 6e66 6967 2e69 6e70  leter(config.inp
-00016a10: 7574 5375 6767 6573 7469 6f6e 732c 2069  utSuggestions, i
-00016a20: 676e 6f72 655f 6361 7365 3d54 7275 6529  gnore_case=True)
-00016a30: 2920 6966 2063 6f6e 6669 672e 696e 7075  ) if config.inpu
-00016a40: 7453 7567 6765 7374 696f 6e73 2065 6c73  tSuggestions els
-00016a50: 6520 4e6f 6e65 0a20 2020 2020 2020 2063  e None.        c
-00016a60: 6f6d 706c 6574 6572 5f64 6576 656c 6f70  ompleter_develop
-00016a70: 6572 203d 2046 757a 7a79 436f 6d70 6c65  er = FuzzyComple
-00016a80: 7465 7228 576f 7264 436f 6d70 6c65 7465  ter(WordComplete
-00016a90: 7228 636f 6e66 6967 2e69 6e70 7574 5375  r(config.inputSu
-00016aa0: 6767 6573 7469 6f6e 735b 3a5d 202b 205b  ggestions[:] + [
-00016ab0: 6622 636f 6e66 6967 2e7b 697d 2220 666f  f"config.{i}" fo
-00016ac0: 7220 6920 696e 2064 6972 2863 6f6e 6669  r i in dir(confi
-00016ad0: 6729 2069 6620 6e6f 7420 692e 7374 6172  g) if not i.star
-00016ae0: 7473 7769 7468 2822 5f5f 2229 5d20 2b20  tswith("__")] + 
-00016af0: 7365 6c66 2e67 6574 4469 7265 6374 6f72  self.getDirector
-00016b00: 794c 6973 7428 292c 2069 676e 6f72 655f  yList(), ignore_
-00016b10: 6361 7365 3d54 7275 6529 290a 2020 2020  case=True)).    
-00016b20: 2020 2020 7768 696c 6520 5472 7565 3a0a      while True:.
-00016b30: 2020 2020 2020 2020 2020 2020 2320 6465              # de
-00016b40: 6661 756c 7420 746f 6f6c 6261 7220 7465  fault toolbar te
-00016b50: 7874 0a20 2020 2020 2020 2020 2020 2063  xt.            c
-00016b60: 6f6e 6669 672e 6479 6e61 6d69 6354 6f6f  onfig.dynamicToo
-00016b70: 6c42 6172 5465 7874 203d 2066 2222 2220  lBarText = f""" 
-00016b80: 7b73 7472 2863 6f6e 6669 672e 686f 746b  {str(config.hotk
-00016b90: 6579 5f65 7869 7429 2e72 6570 6c61 6365  ey_exit).replace
-00016ba0: 2822 2722 2c20 2222 297d 2065 7869 7420  ("'", "")} exit 
-00016bb0: 7b73 7472 2863 6f6e 6669 672e 686f 746b  {str(config.hotk
-00016bc0: 6579 5f64 6973 706c 6179 5f6b 6579 5f63  ey_display_key_c
-00016bd0: 6f6d 626f 292e 7265 706c 6163 6528 2227  ombo).replace("'
-00016be0: 222c 2022 2229 7d20 7368 6f72 7463 7574  ", "")} shortcut
-00016bf0: 7320 2222 220a 2020 2020 2020 2020 2020  s """.          
-00016c00: 2020 2320 6469 7370 6c61 7920 6375 7272    # display curr
-00016c10: 656e 7420 6469 7265 6374 6f72 7920 6966  ent directory if
-00016c20: 2063 6861 6e67 6564 0a20 2020 2020 2020   changed.       
-00016c30: 2020 2020 2063 7572 7265 6e74 4469 7265       currentDire
-00016c40: 6374 6f72 7920 3d20 6f73 2e67 6574 6377  ctory = os.getcw
-00016c50: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-00016c60: 6966 206e 6f74 2063 7572 7265 6e74 4469  if not currentDi
-00016c70: 7265 6374 6f72 7920 3d3d 2073 746f 7261  rectory == stora
-00016c80: 6765 6469 7265 6374 6f72 793a 0a20 2020  gedirectory:.   
-00016c90: 2020 2020 2020 2020 2020 2020 2023 7072               #pr
-00016ca0: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00016cb0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00016cc0: 2020 2070 7269 6e74 3328 6622 4375 7272     print3(f"Curr
-00016cd0: 656e 7420 6469 7265 6374 6f72 793a 207b  ent directory: {
-00016ce0: 6375 7272 656e 7444 6972 6563 746f 7279  currentDirectory
-00016cf0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00016d00: 2020 2020 7072 696e 7431 2873 656c 662e      print1(self.
-00016d10: 6469 7669 6465 7229 0a20 2020 2020 2020  divider).       
-00016d20: 2020 2020 2020 2020 2073 746f 7261 6765           storage
-00016d30: 6469 7265 6374 6f72 7920 3d20 6375 7272  directory = curr
-00016d40: 656e 7444 6972 6563 746f 7279 0a20 2020  entDirectory.   
-00016d50: 2020 2020 2020 2020 2023 2064 6566 6175           # defau
-00016d60: 6c74 2069 6e70 7574 2065 6e74 7279 0a20  lt input entry. 
-00016d70: 2020 2020 2020 2020 2020 2061 6363 6570             accep
-00016d80: 745f 6465 6661 756c 7420 3d20 636f 6e66  t_default = conf
-00016d90: 6967 2e61 6363 6570 745f 6465 6661 756c  ig.accept_defaul
-00016da0: 740a 2020 2020 2020 2020 2020 2020 636f  t.            co
-00016db0: 6e66 6967 2e61 6363 6570 745f 6465 6661  nfig.accept_defa
-00016dc0: 756c 7420 3d20 4661 6c73 650a 2020 2020  ult = False.    
-00016dd0: 2020 2020 2020 2020 6465 6661 756c 7445          defaultE
-00016de0: 6e74 7279 203d 2063 6f6e 6669 672e 6465  ntry = config.de
-00016df0: 6661 756c 7445 6e74 7279 0a20 2020 2020  faultEntry.     
-00016e00: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-00016e10: 682e 6973 6669 6c65 2864 6566 6175 6c74  h.isfile(default
-00016e20: 456e 7472 7929 3a0a 2020 2020 2020 2020  Entry):.        
-00016e30: 2020 2020 2020 2020 6465 6661 756c 7445          defaultE
-00016e40: 6e74 7279 203d 2066 2746 696c 653a 2022  ntry = f'File: "
-00016e50: 7b64 6566 6175 6c74 456e 7472 797d 225c  {defaultEntry}"\
-00016e60: 6e27 0a20 2020 2020 2020 2020 2020 2065  n'.            e
-00016e70: 6c69 6620 6f73 2e70 6174 682e 6973 6469  lif os.path.isdi
-00016e80: 7228 6465 6661 756c 7445 6e74 7279 293a  r(defaultEntry):
-00016e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ea0: 2064 6566 6175 6c74 456e 7472 7920 3d20   defaultEntry = 
-00016eb0: 6627 466f 6c64 6572 3a20 227b 6465 6661  f'Folder: "{defa
-00016ec0: 756c 7445 6e74 7279 7d22 5c6e 270a 2020  ultEntry}"\n'.  
-00016ed0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00016ee0: 2e64 6566 6175 6c74 456e 7472 7920 3d20  .defaultEntry = 
-00016ef0: 2222 0a0a 2020 2020 2020 2020 2020 2020  ""..            
-00016f00: 2320 7573 6572 2069 6e70 7574 0a20 2020  # user input.   
-00016f10: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
-00016f20: 7574 203d 2073 656c 662e 7072 6f6d 7074  ut = self.prompt
-00016f30: 732e 7369 6d70 6c65 5072 6f6d 7074 2870  s.simplePrompt(p
-00016f40: 726f 6d70 7453 6573 7369 6f6e 3d73 656c  romptSession=sel
-00016f50: 662e 7465 726d 696e 616c 5f63 6861 745f  f.terminal_chat_
-00016f60: 7365 7373 696f 6e2c 2063 6f6d 706c 6574  session, complet
-00016f70: 6572 3d63 6f6d 706c 6574 6572 5f64 6576  er=completer_dev
-00016f80: 656c 6f70 6572 2069 6620 636f 6e66 6967  eloper if config
-00016f90: 2e64 6576 656c 6f70 6572 2065 6c73 6520  .developer else 
-00016fa0: 636f 6d70 6c65 7465 722c 2064 6566 6175  completer, defau
-00016fb0: 6c74 3d64 6566 6175 6c74 456e 7472 792c  lt=defaultEntry,
-00016fc0: 2061 6363 6570 745f 6465 6661 756c 743d   accept_default=
-00016fd0: 6163 6365 7074 5f64 6566 6175 6c74 2c20  accept_default, 
-00016fe0: 7661 6c69 6461 746f 723d 746f 6b65 6e56  validator=tokenV
-00016ff0: 616c 6964 6174 6f72 2c20 626f 7474 6f6d  alidator, bottom
-00017000: 5f74 6f6f 6c62 6172 3d67 6574 4479 6e61  _toolbar=getDyna
-00017010: 6d69 6354 6f6f 6c42 6172 290a 2020 2020  micToolBar).    
-00017020: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00017030: 2020 2020 2023 2075 7064 6174 6520 7379       # update sy
-00017040: 7374 656d 206d 6573 7361 6765 2077 6865  stem message whe
-00017050: 6e20 7573 6572 2065 6e74 6572 2061 206e  n user enter a n
-00017060: 6577 2069 6e70 7574 0a20 2020 2020 2020  ew input.       
-00017070: 2020 2020 2063 6f6e 6669 672e 6375 7272       config.curr
-00017080: 656e 744d 6573 7361 6765 7320 3d20 7365  entMessages = se
-00017090: 6c66 2e75 7064 6174 6553 7973 7465 6d4d  lf.updateSystemM
-000170a0: 6573 7361 6765 2863 6f6e 6669 672e 6375  essage(config.cu
-000170b0: 7272 656e 744d 6573 7361 6765 7329 0a20  rrentMessages). 
-000170c0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-000170d0: 2020 2020 2020 2020 2320 6469 7370 6c61          # displa
-000170e0: 7920 6f70 7469 6f6e 7320 7768 656e 2065  y options when e
-000170f0: 6d70 7479 2073 7472 696e 6720 6973 2065  mpty string is e
-00017100: 6e74 6572 6564 0a20 2020 2020 2020 2020  ntered.         
-00017110: 2020 2075 7365 7249 6e70 7574 4c6f 7765     userInputLowe
-00017120: 7220 3d20 7573 6572 496e 7075 742e 6c6f  r = userInput.lo
-00017130: 7765 7228 290a 2020 2020 2020 2020 2020  wer().          
-00017140: 2020 6966 2063 6f6e 6669 672e 6164 6450    if config.addP
-00017150: 6174 6841 7420 6973 206e 6f74 204e 6f6e  athAt is not Non
-00017160: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00017170: 2020 2070 7265 6669 7820 3d20 7573 6572     prefix = user
-00017180: 496e 7075 745b 3a63 6f6e 6669 672e 6164  Input[:config.ad
-00017190: 6450 6174 6841 745d 0a20 2020 2020 2020  dPathAt].       
-000171a0: 2020 2020 2020 2020 2070 7265 6669 7853           prefixS
-000171b0: 706c 6974 203d 2070 7265 6669 782e 7273  plit = prefix.rs
-000171c0: 706c 6974 2822 2022 2c20 3129 0a20 2020  plit(" ", 1).   
-000171d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000171e0: 6c65 6e28 7072 6566 6978 5370 6c69 7429  len(prefixSplit)
-000171f0: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
-00017200: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-00017210: 7420 3d20 7072 6566 6978 5370 6c69 745b  t = prefixSplit[
-00017220: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
-00017230: 2020 2020 2020 2020 7072 6566 6978 203d          prefix =
-00017240: 2066 227b 7072 6566 6978 5370 6c69 745b   f"{prefixSplit[
-00017250: 305d 7d20 220a 2020 2020 2020 2020 2020  0]} ".          
-00017260: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000138b0: 666f 726d 203d 3d20 224c 696e 7578 2220  form == "Linux" 
+000138c0: 616e 6420 7368 7574 696c 2e77 6869 6368  and shutil.which
+000138d0: 2822 7069 7065 7222 293a 0a20 2020 2020  ("piper"):.     
+000138e0: 2020 2020 2020 206f 7074 696f 6e73 2e69         options.i
+000138f0: 6e73 6572 7428 302c 2022 7069 7065 7222  nsert(0, "piper"
+00013900: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
+00013910: 7363 7269 7074 696f 6e73 2e69 6e73 6572  scriptions.inser
+00013920: 7428 302c 2022 5069 7065 7220 284f 6666  t(0, "Piper (Off
+00013930: 6c69 6e65 2922 290a 2020 2020 2020 2020  line)").        
+00013940: 7474 7350 6c61 7466 6f72 6d20 3d20 7365  ttsPlatform = se
+00013950: 6c66 2e64 6961 6c6f 6773 2e67 6574 5661  lf.dialogs.getVa
+00013960: 6c69 644f 7074 696f 6e73 280a 2020 2020  lidOptions(.    
+00013970: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
+00013980: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
+00013990: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000139a0: 733d 6465 7363 7269 7074 696f 6e73 2c0a  s=descriptions,.
+000139b0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+000139c0: 653d 2254 6578 742d 746f 2d53 7065 6563  e="Text-to-Speec
+000139d0: 6820 436f 6e66 6967 7572 6174 696f 6e73  h Configurations
+000139e0: 222c 0a20 2020 2020 2020 2020 2020 2074  ",.            t
+000139f0: 6578 743d 2253 656c 6563 7420 6120 7465  ext="Select a te
+00013a00: 7874 2d74 6f2d 7370 6565 6368 2070 6c61  xt-to-speech pla
+00013a10: 7466 6f72 6d3a 222c 0a20 2020 2020 2020  tform:",.       
+00013a20: 2020 2020 2064 6566 6175 6c74 3d63 6f6e       default=con
+00013a30: 6669 672e 7474 7350 6c61 7466 6f72 6d2c  fig.ttsPlatform,
+00013a40: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00013a50: 2020 2069 6620 7474 7350 6c61 7466 6f72     if ttsPlatfor
+00013a60: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
+00013a70: 6620 7474 7350 6c61 7466 6f72 6d20 3d3d  f ttsPlatform ==
+00013a80: 2022 676f 6f67 6c65 636c 6f75 6422 2061   "googlecloud" a
+00013a90: 6e64 206e 6f74 2028 6f73 2e65 6e76 6972  nd not (os.envir
+00013aa0: 6f6e 5b22 474f 4f47 4c45 5f41 5050 4c49  on["GOOGLE_APPLI
+00013ab0: 4341 5449 4f4e 5f43 5245 4445 4e54 4941  CATION_CREDENTIA
+00013ac0: 4c53 225d 2061 6e64 2022 5465 7874 2d74  LS"] and "Text-t
+00013ad0: 6f2d 5370 6565 6368 2220 696e 2063 6f6e  o-Speech" in con
+00013ae0: 6669 672e 656e 6162 6c65 6447 6f6f 676c  fig.enabledGoogl
+00013af0: 6541 5049 7329 3a0a 2020 2020 2020 2020  eAPIs):.        
+00013b00: 2020 2020 2020 2020 7072 696e 7432 2822          print2("
+00013b10: 476f 6f67 6c65 2043 6c6f 7564 2054 6578  Google Cloud Tex
+00013b20: 742d 746f 2d53 7065 6563 6820 6665 6174  t-to-Speech feat
+00013b30: 7572 6520 6973 206e 6f74 2065 6e61 626c  ure is not enabl
+00013b40: 6564 2122 290a 2020 2020 2020 2020 2020  ed!").          
+00013b50: 2020 2020 2020 7072 696e 7433 2822 5265        print3("Re
+00013b60: 6164 3a20 6874 7470 733a 2f2f 6769 7468  ad: https://gith
+00013b70: 7562 2e63 6f6d 2f65 6c69 7261 6e77 6f6e  ub.com/eliranwon
+00013b80: 672f 6c65 746d 6564 6f69 742f 7769 6b69  g/letmedoit/wiki
+00013b90: 2f47 6f6f 676c 652d 4150 492d 5365 7475  /Google-API-Setu
+00013ba0: 7022 290a 2020 2020 2020 2020 2020 2020  p").            
+00013bb0: 2020 2020 7072 696e 7433 2822 5465 7874      print3("Text
+00013bc0: 2d74 6f2d 5370 6565 6368 2070 6c61 7466  -to-Speech platf
+00013bd0: 6f72 6d20 6368 616e 6765 6420 746f 3a20  orm changed to: 
+00013be0: 476f 6f67 6c65 2054 6578 742d 746f 2d53  Google Text-to-S
+00013bf0: 7065 6563 6820 2847 656e 6572 6963 2922  peech (Generic)"
+00013c00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00013c10: 2020 636f 6e66 6967 2e74 7473 506c 6174    config.ttsPlat
+00013c20: 666f 726d 203d 2022 676f 6f67 6c65 220a  form = "google".
+00013c30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00013c40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013c50: 2020 636f 6e66 6967 2e74 7473 506c 6174    config.ttsPlat
+00013c60: 666f 726d 203d 2074 7473 506c 6174 666f  form = ttsPlatfo
+00013c70: 726d 0a20 2020 2020 2020 2023 2066 7572  rm.        # fur
+00013c80: 7468 6572 206f 7074 696f 6e73 0a20 2020  ther options.   
+00013c90: 2020 2020 2069 6620 636f 6e66 6967 2e74       if config.t
+00013ca0: 7473 506c 6174 666f 726d 203d 3d20 2267  tsPlatform == "g
+00013cb0: 6f6f 676c 6522 3a0a 2020 2020 2020 2020  oogle":.        
+00013cc0: 2020 2020 7365 6c66 2e73 6574 4774 7473      self.setGtts
+00013cd0: 4c61 6e67 7561 6765 2829 0a20 2020 2020  Language().     
+00013ce0: 2020 2020 2020 2073 656c 662e 7365 7441         self.setA
+00013cf0: 7564 696f 506c 6179 6261 636b 546f 6f6c  udioPlaybackTool
+00013d00: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00013d10: 656c 662e 7365 7456 6c63 5370 6565 6428  elf.setVlcSpeed(
+00013d20: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
+00013d30: 6f6e 6669 672e 7474 7350 6c61 7466 6f72  onfig.ttsPlatfor
+00013d40: 6d20 3d3d 2022 676f 6f67 6c65 636c 6f75  m == "googleclou
+00013d50: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
+00013d60: 7365 6c66 2e73 6574 4763 7474 734c 616e  self.setGcttsLan
+00013d70: 6775 6167 6528 290a 2020 2020 2020 2020  guage().        
+00013d80: 2020 2020 7365 6c66 2e73 6574 4763 7474      self.setGctt
+00013d90: 7353 7065 6564 2829 0a20 2020 2020 2020  sSpeed().       
+00013da0: 2020 2020 2073 656c 662e 7365 7441 7564       self.setAud
+00013db0: 696f 506c 6179 6261 636b 546f 6f6c 2829  ioPlaybackTool()
+00013dc0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013dd0: 662e 7365 7456 6c63 5370 6565 6428 290a  f.setVlcSpeed().
+00013de0: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
+00013df0: 672e 7474 7350 6c61 7466 6f72 6d20 3d3d  g.ttsPlatform ==
+00013e00: 2022 7069 7065 7222 3a0a 2020 2020 2020   "piper":.      
+00013e10: 2020 2020 2020 7365 6c66 2e73 6574 5069        self.setPi
+00013e20: 7065 7256 6f69 6365 2829 0a20 2020 2020  perVoice().     
+00013e30: 2020 2020 2020 2073 656c 662e 7365 7441         self.setA
+00013e40: 7564 696f 506c 6179 6261 636b 546f 6f6c  udioPlaybackTool
+00013e50: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+00013e60: 656c 662e 7365 7456 6c63 5370 6565 6428  elf.setVlcSpeed(
+00013e70: 290a 2020 2020 2020 2020 656c 6966 2063  ).        elif c
+00013e80: 6f6e 6669 672e 7474 7350 6c61 7466 6f72  onfig.ttsPlatfor
+00013e90: 6d20 3d3d 2022 656c 6576 656e 6c61 6273  m == "elevenlabs
+00013ea0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
+00013eb0: 6620 6e6f 7420 636f 6e66 6967 2e65 6c65  f not config.ele
+00013ec0: 7665 6e6c 6162 7341 7069 3a0a 2020 2020  venlabsApi:.    
+00013ed0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00013ee0: 2e63 6861 6e67 6545 6c65 7665 6e6c 6162  .changeElevenlab
+00013ef0: 7341 7069 2829 0a20 2020 2020 2020 2020  sApi().         
+00013f00: 2020 2069 6620 6e6f 7420 636f 6e66 6967     if not config
+00013f10: 2e65 6c65 7665 6e6c 6162 7341 7069 3a0a  .elevenlabsApi:.
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f30: 7072 696e 7431 2822 456c 6576 656e 4c61  print1("ElevenLa
+00013f40: 6273 2041 5049 206b 6579 206e 6f74 2066  bs API key not f
+00013f50: 6f75 6e64 2122 290a 2020 2020 2020 2020  ound!").        
+00013f60: 2020 2020 2020 2020 7072 696e 7433 2822          print3("
+00013f70: 5465 7874 2d74 6f2d 5370 6565 6368 2070  Text-to-Speech p
+00013f80: 6c61 7466 6f72 6d20 6368 616e 6765 6420  latform changed 
+00013f90: 746f 3a20 476f 6f67 6c65 2054 6578 742d  to: Google Text-
+00013fa0: 746f 2d53 7065 6563 6820 2847 656e 6572  to-Speech (Gener
+00013fb0: 6963 2922 290a 2020 2020 2020 2020 2020  ic)").          
+00013fc0: 2020 2020 2020 636f 6e66 6967 2e74 7473        config.tts
+00013fd0: 506c 6174 666f 726d 203d 2022 676f 6f67  Platform = "goog
+00013fe0: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
+00013ff0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00014000: 2020 2020 2020 7365 6c66 2e73 6574 456c        self.setEl
+00014010: 6576 656e 6c61 6273 566f 6963 6528 290a  evenlabsVoice().
+00014020: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
+00014030: 6669 672e 7474 7350 6c61 7466 6f72 6d20  fig.ttsPlatform 
+00014040: 3d3d 2022 6375 7374 6f6d 223a 0a20 2020  == "custom":.   
+00014050: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
+00014060: 6669 6e65 5474 7343 6f6d 6d61 6e64 2829  fineTtsCommand()
+00014070: 0a20 2020 2020 2020 2023 2073 6176 6520  .        # save 
+00014080: 636f 6e66 6967 730a 2020 2020 2020 2020  configs.        
+00014090: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
+000140a0: 6728 290a 0a20 2020 2064 6566 2073 6574  g()..    def set
+000140b0: 566f 6963 6554 7970 696e 6743 6f6e 6669  VoiceTypingConfi
+000140c0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
+000140d0: 2076 6f69 6365 5479 7069 6e67 506c 6174   voiceTypingPlat
+000140e0: 666f 726d 203d 2073 656c 662e 6469 616c  form = self.dial
+000140f0: 6f67 732e 6765 7456 616c 6964 4f70 7469  ogs.getValidOpti
+00014100: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
+00014110: 206f 7074 696f 6e73 3d28 2267 6f6f 676c   options=("googl
+00014120: 6522 2c20 2267 6f6f 676c 6563 6c6f 7564  e", "googlecloud
+00014130: 222c 2022 7768 6973 7065 7222 292c 0a20  ", "whisper"),. 
+00014140: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00014150: 6970 7469 6f6e 733d 2822 476f 6f67 6c65  iptions=("Google
+00014160: 2053 7065 6563 682d 746f 2d54 6578 7420   Speech-to-Text 
+00014170: 2847 656e 6572 6963 2920 5b6f 6e6c 696e  (Generic) [onlin
+00014180: 655d 222c 2022 476f 6f67 6c65 2053 7065  e]", "Google Spe
+00014190: 6563 682d 746f 2d54 6578 7420 2841 5049  ech-to-Text (API
+000141a0: 2920 5b6f 6e6c 696e 655d 222c 2022 4f70  ) [online]", "Op
+000141b0: 656e 4149 2057 6869 7370 6572 205b 6f66  enAI Whisper [of
+000141c0: 666c 696e 653b 2073 6c6f 7765 7220 7769  fline; slower wi
+000141d0: 7468 206e 6f6e 2d45 6e67 6c69 7368 2076  th non-English v
+000141e0: 6f69 6365 735d 2229 2c0a 2020 2020 2020  oices]"),.      
+000141f0: 2020 2020 2020 7469 746c 653d 2256 6f69        title="Voi
+00014200: 6365 2054 7970 696e 6720 436f 6e66 6967  ce Typing Config
+00014210: 7572 6174 696f 6e73 222c 0a20 2020 2020  urations",.     
+00014220: 2020 2020 2020 2074 6578 743d 2253 656c         text="Sel
+00014230: 6563 7420 6120 766f 6963 6520 7479 7069  ect a voice typi
+00014240: 6e67 2070 6c61 7466 6f72 6d3a 222c 0a20  ng platform:",. 
+00014250: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+00014260: 6c74 3d63 6f6e 6669 672e 766f 6963 6554  lt=config.voiceT
+00014270: 7970 696e 6750 6c61 7466 6f72 6d2c 0a20  ypingPlatform,. 
+00014280: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00014290: 2069 6620 766f 6963 6554 7970 696e 6750   if voiceTypingP
+000142a0: 6c61 7466 6f72 6d3a 0a20 2020 2020 2020  latform:.       
+000142b0: 2020 2020 2069 6620 766f 6963 6554 7970       if voiceTyp
+000142c0: 696e 6750 6c61 7466 6f72 6d20 3d3d 2022  ingPlatform == "
+000142d0: 676f 6f67 6c65 636c 6f75 6422 2061 6e64  googlecloud" and
+000142e0: 206e 6f74 2028 6f73 2e65 6e76 6972 6f6e   not (os.environ
+000142f0: 5b22 474f 4f47 4c45 5f41 5050 4c49 4341  ["GOOGLE_APPLICA
+00014300: 5449 4f4e 5f43 5245 4445 4e54 4941 4c53  TION_CREDENTIALS
+00014310: 225d 2061 6e64 2022 5370 6565 6368 2d74  "] and "Speech-t
+00014320: 6f2d 5465 7874 2220 696e 2063 6f6e 6669  o-Text" in confi
+00014330: 672e 656e 6162 6c65 6447 6f6f 676c 6541  g.enabledGoogleA
+00014340: 5049 7329 3a0a 2020 2020 2020 2020 2020  PIs):.          
+00014350: 2020 2020 2020 7072 696e 7432 2822 476f        print2("Go
+00014360: 6f67 6c65 2043 6c6f 7564 2053 7065 6563  ogle Cloud Speec
+00014370: 682d 746f 2d54 6578 7420 6665 6174 7572  h-to-Text featur
+00014380: 6520 6973 206e 6f74 2065 6e61 626c 6564  e is not enabled
+00014390: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
+000143a0: 2020 2020 7072 696e 7433 2822 5265 6164      print3("Read
+000143b0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000143c0: 2e63 6f6d 2f65 6c69 7261 6e77 6f6e 672f  .com/eliranwong/
+000143d0: 6c65 746d 6564 6f69 742f 7769 6b69 2f47  letmedoit/wiki/G
+000143e0: 6f6f 676c 652d 4150 492d 5365 7475 7022  oogle-API-Setup"
+000143f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014400: 2020 7072 696e 7433 2822 566f 6963 6520    print3("Voice 
+00014410: 7479 7069 6e67 2070 6c61 7466 6f72 6d20  typing platform 
+00014420: 6368 616e 6765 6420 746f 3a20 476f 6f67  changed to: Goog
+00014430: 6c65 2053 7065 6563 682d 746f 2d54 6578  le Speech-to-Tex
+00014440: 7420 2847 656e 6572 6963 2922 290a 2020  t (Generic)").  
+00014450: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014460: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
+00014470: 506c 6174 666f 726d 203d 2022 676f 6f67  Platform = "goog
+00014480: 6c65 220a 2020 2020 2020 2020 2020 2020  le".            
+00014490: 656c 6966 2076 6f69 6365 5479 7069 6e67  elif voiceTyping
+000144a0: 506c 6174 666f 726d 203d 3d20 2277 6869  Platform == "whi
+000144b0: 7370 6572 2220 616e 6420 6e6f 7420 6973  sper" and not is
+000144c0: 436f 6d6d 616e 6449 6e73 7461 6c6c 6564  CommandInstalled
+000144d0: 2822 6666 6d70 6567 2229 3a0a 2020 2020  ("ffmpeg"):.    
+000144e0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000144f0: 7432 2822 496e 7374 616c 6c20 2766 666d  t2("Install 'ffm
+00014500: 7065 6727 2066 6972 7374 2074 6f20 7573  peg' first to us
+00014510: 6520 6f66 666c 696e 6520 6f70 656e 6169  e offline openai
+00014520: 2077 6869 7370 6572 206d 6f64 656c 2122   whisper model!"
+00014530: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014540: 2020 7072 696e 7433 2822 5265 6164 3a20    print3("Read: 
+00014550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00014560: 6f6d 2f6f 7065 6e61 692f 7768 6973 7065  om/openai/whispe
+00014570: 7223 7365 7475 7022 290a 2020 2020 2020  r#setup").      
+00014580: 2020 2020 2020 2020 2020 7072 696e 7433            print3
+00014590: 2822 566f 6963 6520 7479 7069 6e67 2070  ("Voice typing p
+000145a0: 6c61 7466 6f72 6d20 6368 616e 6765 6420  latform changed 
+000145b0: 746f 3a20 476f 6f67 6c65 2053 7065 6563  to: Google Speec
+000145c0: 682d 746f 2d54 6578 7420 2847 656e 6572  h-to-Text (Gener
+000145d0: 6963 2922 290a 2020 2020 2020 2020 2020  ic)").          
+000145e0: 2020 2020 2020 636f 6e66 6967 2e76 6f69        config.voi
+000145f0: 6365 5479 7069 6e67 506c 6174 666f 726d  ceTypingPlatform
+00014600: 203d 2022 676f 6f67 6c65 220a 2020 2020   = "google".    
+00014610: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00014620: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00014630: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
+00014640: 506c 6174 666f 726d 203d 2076 6f69 6365  Platform = voice
+00014650: 5479 7069 6e67 506c 6174 666f 726d 0a20  TypingPlatform. 
+00014660: 2020 2020 2020 2023 206c 616e 6775 6167         # languag
+00014670: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
+00014680: 6574 5370 6565 6368 546f 5465 7874 4c61  etSpeechToTextLa
+00014690: 6e67 7561 6765 2829 0a20 2020 2020 2020  nguage().       
+000146a0: 2023 2063 6f6e 6669 6775 7265 2063 6f6e   # configure con
+000146b0: 6669 672e 766f 6963 6554 7970 696e 6741  fig.voiceTypingA
+000146c0: 646a 7573 7441 6d62 6965 6e74 4e6f 6973  djustAmbientNois
+000146d0: 650a 2020 2020 2020 2020 766f 6963 6554  e.        voiceT
+000146e0: 7970 696e 6741 646a 7573 7441 6d62 6965  ypingAdjustAmbie
+000146f0: 6e74 4e6f 6973 6520 3d20 7365 6c66 2e64  ntNoise = self.d
+00014700: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+00014710: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+00014720: 2020 2020 6f70 7469 6f6e 733d 2822 5965      options=("Ye
+00014730: 7322 2c20 224e 6f22 292c 0a20 2020 2020  s", "No"),.     
+00014740: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00014750: 6f6e 733d 2822 5965 7320 5b73 6c6f 7765  ons=("Yes [slowe
+00014760: 725d 222c 2022 4e6f 2229 2c0a 2020 2020  r]", "No"),.    
+00014770: 2020 2020 2020 2020 7469 746c 653d 2241          title="A
+00014780: 646a 7573 7420 416d 6269 656e 7420 4e6f  djust Ambient No
+00014790: 6973 6522 2c0a 2020 2020 2020 2020 2020  ise",.          
+000147a0: 2020 7465 7874 3d22 446f 2079 6f75 2077    text="Do you w
+000147b0: 616e 7420 746f 2061 646a 7573 7420 616d  ant to adjust am
+000147c0: 6269 656e 7420 6e6f 6973 653f 222c 0a20  bient noise?",. 
+000147d0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+000147e0: 6c74 3d22 5965 7322 2069 6620 636f 6e66  lt="Yes" if conf
+000147f0: 6967 2e76 6f69 6365 5479 7069 6e67 4164  ig.voiceTypingAd
+00014800: 6a75 7374 416d 6269 656e 744e 6f69 7365  justAmbientNoise
+00014810: 2065 6c73 6520 224e 6f22 2c0a 2020 2020   else "No",.    
+00014820: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+00014830: 2076 6f69 6365 5479 7069 6e67 4164 6a75   voiceTypingAdju
+00014840: 7374 416d 6269 656e 744e 6f69 7365 3a0a  stAmbientNoise:.
+00014850: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00014860: 6967 2e76 6f69 6365 5479 7069 6e67 4164  ig.voiceTypingAd
+00014870: 6a75 7374 416d 6269 656e 744e 6f69 7365  justAmbientNoise
+00014880: 203d 2054 7275 6520 6966 2076 6f69 6365   = True if voice
+00014890: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
+000148a0: 656e 744e 6f69 7365 203d 3d20 2259 6573  entNoise == "Yes
+000148b0: 2220 656c 7365 2046 616c 7365 0a20 2020  " else False.   
+000148c0: 2020 2020 2023 2061 7564 696f 206e 6f74       # audio not
+000148d0: 6966 6963 6174 696f 6e0a 2020 2020 2020  ification.      
+000148e0: 2020 766f 6963 6554 7970 696e 674e 6f74    voiceTypingNot
+000148f0: 6966 6963 6174 696f 6e20 3d20 7365 6c66  ification = self
+00014900: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
+00014910: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
+00014920: 2020 2020 2020 6f70 7469 6f6e 733d 2822        options=("
+00014930: 5965 7322 2c20 224e 6f22 292c 0a20 2020  Yes", "No"),.   
+00014940: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
+00014950: 4175 6469 6f20 4e6f 7469 6669 6361 7469  Audio Notificati
+00014960: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00014970: 2074 6578 743d 2244 6f20 796f 7520 7761   text="Do you wa
+00014980: 6e74 2061 7564 696f 206e 6f74 6966 6963  nt audio notific
+00014990: 6174 696f 6e20 7768 656e 2079 6f75 2075  ation when you u
+000149a0: 7365 206d 6963 726f 7068 6f6e 653f 222c  se microphone?",
+000149b0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+000149c0: 6175 6c74 3d22 5965 7322 2069 6620 636f  ault="Yes" if co
+000149d0: 6e66 6967 2e76 6f69 6365 5479 7069 6e67  nfig.voiceTyping
+000149e0: 4e6f 7469 6669 6361 7469 6f6e 2065 6c73  Notification els
+000149f0: 6520 224e 6f22 2c0a 2020 2020 2020 2020  e "No",.        
+00014a00: 290a 2020 2020 2020 2020 6966 2076 6f69  ).        if voi
+00014a10: 6365 5479 7069 6e67 4e6f 7469 6669 6361  ceTypingNotifica
+00014a20: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00014a30: 2020 636f 6e66 6967 2e76 6f69 6365 5479    config.voiceTy
+00014a40: 7069 6e67 4e6f 7469 6669 6361 7469 6f6e  pingNotification
+00014a50: 203d 2054 7275 6520 6966 2076 6f69 6365   = True if voice
+00014a60: 5479 7069 6e67 4e6f 7469 6669 6361 7469  TypingNotificati
+00014a70: 6f6e 203d 3d20 2259 6573 2220 656c 7365  on == "Yes" else
+00014a80: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
+00014a90: 2061 7574 6f20 636f 6d70 6c65 7469 6f6e   auto completion
+00014aa0: 3a20 766f 6963 6554 7970 696e 6741 7574  : voiceTypingAut
+00014ab0: 6f43 6f6d 706c 6574 650a 2020 2020 2020  oComplete.      
+00014ac0: 2020 766f 6963 6554 7970 696e 6741 7574    voiceTypingAut
+00014ad0: 6f43 6f6d 706c 6574 6520 3d20 7365 6c66  oComplete = self
+00014ae0: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
+00014af0: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
+00014b00: 2020 2020 2020 6f70 7469 6f6e 733d 2822        options=("
+00014b10: 5965 7322 2c20 224e 6f22 292c 0a20 2020  Yes", "No"),.   
+00014b20: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
+00014b30: 4175 6469 6f20 456e 7472 7920 4175 746f  Audio Entry Auto
+00014b40: 2043 6f6d 706c 6574 696f 6e22 2c0a 2020   Completion",.  
+00014b50: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
+00014b60: 446f 2079 6f75 2077 616e 7420 746f 2061  Do you want to a
+00014b70: 7574 6f6d 6174 6963 616c 6c79 2063 6f6d  utomatically com
+00014b80: 706c 6574 6520 796f 7572 2065 6e74 7279  plete your entry
+00014b90: 2077 6865 6e20 6d69 6372 6f70 686f 6e65   when microphone
+00014ba0: 2073 746f 7073 3f22 2c0a 2020 2020 2020   stops?",.      
+00014bb0: 2020 2020 2020 6465 6661 756c 743d 2259        default="Y
+00014bc0: 6573 2220 6966 2063 6f6e 6669 672e 766f  es" if config.vo
+00014bd0: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
+00014be0: 706c 6574 6520 656c 7365 2022 4e6f 222c  plete else "No",
+00014bf0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00014c00: 2020 2069 6620 766f 6963 6554 7970 696e     if voiceTypin
+00014c10: 6741 7574 6f43 6f6d 706c 6574 653a 0a20  gAutoComplete:. 
+00014c20: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00014c30: 672e 766f 6963 6554 7970 696e 6741 7574  g.voiceTypingAut
+00014c40: 6f43 6f6d 706c 6574 6520 3d20 5472 7565  oComplete = True
+00014c50: 2069 6620 766f 6963 6554 7970 696e 6741   if voiceTypingA
+00014c60: 7574 6f43 6f6d 706c 6574 6520 3d3d 2022  utoComplete == "
+00014c70: 5965 7322 2065 6c73 6520 4661 6c73 650a  Yes" else False.
+00014c80: 2020 2020 2020 2020 2320 6e6f 7469 6679          # notify
+00014c90: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00014ca0: 2229 0a20 2020 2020 2020 2070 7269 6e74  ").        print
+00014cb0: 3328 6622 566f 6963 6520 5479 7069 6e67  3(f"Voice Typing
+00014cc0: 204d 6f64 656c 3a20 7b63 6f6e 6669 672e   Model: {config.
+00014cd0: 766f 6963 6554 7970 696e 6750 6c61 7466  voiceTypingPlatf
+00014ce0: 6f72 6d7d 2229 0a20 2020 2020 2020 2070  orm}").        p
+00014cf0: 7269 6e74 3328 6622 566f 6963 6520 5479  rint3(f"Voice Ty
+00014d00: 7069 6e67 204c 616e 6775 6167 653a 207b  ping Language: {
+00014d10: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
+00014d20: 6e67 4c61 6e67 7561 6765 7d22 290a 2020  ngLanguage}").  
+00014d30: 2020 2020 2020 7072 696e 7433 2866 2241        print3(f"A
+00014d40: 6d62 6965 6e74 204e 6f69 7365 2041 646a  mbient Noise Adj
+00014d50: 7573 746d 656e 743a 207b 636f 6e66 6967  ustment: {config
+00014d60: 2e76 6f69 6365 5479 7069 6e67 4164 6a75  .voiceTypingAdju
+00014d70: 7374 416d 6269 656e 744e 6f69 7365 7d22  stAmbientNoise}"
+00014d80: 290a 2020 2020 2020 2020 7072 696e 7433  ).        print3
+00014d90: 2866 2241 7564 696f 204e 6f74 6966 6963  (f"Audio Notific
+00014da0: 6174 696f 6e3a 207b 636f 6e66 6967 2e76  ation: {config.v
+00014db0: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
+00014dc0: 6361 7469 6f6e 7d22 290a 2020 2020 2020  cation}").      
+00014dd0: 2020 7072 696e 7433 2866 2241 7574 6f20    print3(f"Auto 
+00014de0: 436f 6d70 6c65 7469 6f6e 3a20 7b63 6f6e  Completion: {con
+00014df0: 6669 672e 766f 6963 6554 7970 696e 6741  fig.voiceTypingA
+00014e00: 7574 6f43 6f6d 706c 6574 657d 2229 0a20  utoComplete}"). 
+00014e10: 2020 2020 2020 2023 2073 6176 6520 636f         # save co
+00014e20: 6e66 6967 730a 2020 2020 2020 2020 636f  nfigs.        co
+00014e30: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
+00014e40: 290a 0a20 2020 2064 6566 2073 6176 6543  )..    def saveC
+00014e50: 6861 7428 7365 6c66 2c20 6d65 7373 6167  hat(self, messag
+00014e60: 6573 293a 0a20 2020 2020 2020 206d 6573  es):.        mes
+00014e70: 7361 6765 7343 6f70 7920 3d20 636f 7079  sagesCopy = copy
+00014e80: 2e64 6565 7063 6f70 7928 6d65 7373 6167  .deepcopy(messag
+00014e90: 6573 290a 0a20 2020 2020 2020 2069 6620  es)..        if 
+00014ea0: 636f 6e66 6967 2e63 6f6e 7665 7273 6174  config.conversat
+00014eb0: 696f 6e53 7461 7274 6564 3a0a 2020 2020  ionStarted:.    
+00014ec0: 2020 2020 2020 2020 7469 6d65 7374 616d          timestam
+00014ed0: 7020 3d20 6765 7443 7572 7265 6e74 4461  p = getCurrentDa
+00014ee0: 7465 5469 6d65 2829 0a0a 2020 2020 2020  teTime()..      
+00014ef0: 2020 2020 2020 6966 2068 6173 6174 7472        if hasattr
+00014f00: 2863 6f6e 6669 672c 2022 7361 7665 5f63  (config, "save_c
+00014f10: 6861 745f 7265 636f 7264 2229 3a0a 2020  hat_record"):.  
+00014f20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00014f30: 7768 656e 2070 6c75 6769 6e20 2273 6176  when plugin "sav
+00014f40: 6520 6368 6174 2072 6563 6f72 6473 2220  e chat records" 
+00014f50: 6973 2065 6e61 626c 6564 0a20 2020 2020  is enabled.     
+00014f60: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00014f70: 6765 4c65 6e67 7468 203d 206c 656e 286d  geLength = len(m
+00014f80: 6573 7361 6765 7343 6f70 7929 0a20 2020  essagesCopy).   
+00014f90: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00014fa0: 206f 7264 6572 2c20 6920 696e 2065 6e75   order, i in enu
+00014fb0: 6d65 7261 7465 286d 6573 7361 6765 7343  merate(messagesC
+00014fc0: 6f70 7929 3a0a 2020 2020 2020 2020 2020  opy):.          
+00014fd0: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
+00014fe0: 4974 656d 203d 2028 6f72 6465 7220 3d3d  Item = (order ==
+00014ff0: 2028 6d65 7373 6167 654c 656e 6774 6820   (messageLength 
+00015000: 2d20 3129 290a 2020 2020 2020 2020 2020  - 1)).          
+00015010: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
+00015020: 6669 672e 6c6c 6d49 6e74 6572 6661 6365  fig.llmInterface
+00015030: 2069 6e20 2822 6368 6174 6770 7422 2c20   in ("chatgpt", 
+00015040: 226c 6574 6d65 646f 6974 222c 2022 6772  "letmedoit", "gr
+00015050: 6f71 2229 2061 6e64 206e 6f74 2069 734c  oq") and not isL
+00015060: 6173 7449 7465 6d20 616e 6420 692e 6765  astItem and i.ge
+00015070: 7428 2272 6f6c 6522 2c20 2222 2920 3d3d  t("role", "") ==
+00015080: 2022 7573 6572 2220 616e 6420 2266 756e   "user" and "fun
+00015090: 6374 696f 6e5f 6361 6c6c 2220 696e 206d  ction_call" in m
+000150a0: 6573 7361 6765 7343 6f70 795b 6f72 6465  essagesCopy[orde
+000150b0: 722b 315d 3a0a 2020 2020 2020 2020 2020  r+1]:.          
+000150c0: 2020 2020 2020 2020 2020 2020 2020 695b                i[
+000150d0: 2274 6f6f 6c22 5d20 3d20 6d65 7373 6167  "tool"] = messag
+000150e0: 6573 436f 7079 5b6f 7264 6572 2b31 5d5b  esCopy[order+1][
+000150f0: 2266 756e 6374 696f 6e5f 6361 6c6c 225d  "function_call"]
+00015100: 2e67 6574 2822 6e61 6d65 222c 2022 2229  .get("name", "")
+00015110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015120: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+00015130: 5f63 6861 745f 7265 636f 7264 2874 696d  _chat_record(tim
+00015140: 6573 7461 6d70 2c20 6f72 6465 722c 2069  estamp, order, i
+00015150: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00015160: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00015170: 2020 2020 666f 6c64 6572 5061 7468 203d      folderPath =
+00015180: 206f 732e 7061 7468 2e6a 6f69 6e28 636f   os.path.join(co
+00015190: 6e66 6967 2e6c 6f63 616c 5374 6f72 6167  nfig.localStorag
+000151a0: 652c 2022 6368 6174 7322 2c20 7265 2e73  e, "chats", re.s
+000151b0: 7562 2822 5e28 5b30 2d39 5d2b 3f5c 2d5b  ub("^([0-9]+?\-[
+000151c0: 302d 395d 2b3f 295c 2d2e 2a3f 2422 2c20  0-9]+?)\-.*?$", 
+000151d0: 7222 5c31 222c 2074 696d 6573 7461 6d70  r"\1", timestamp
+000151e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000151f0: 2020 2050 6174 6828 666f 6c64 6572 5061     Path(folderPa
+00015200: 7468 292e 6d6b 6469 7228 7061 7265 6e74  th).mkdir(parent
+00015210: 733d 5472 7565 2c20 6578 6973 745f 6f6b  s=True, exist_ok
+00015220: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+00015230: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00015240: 682e 6973 6469 7228 666f 6c64 6572 5061  h.isdir(folderPa
+00015250: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
+00015260: 2020 2020 2020 2020 2063 6861 7446 696c           chatFil
+00015270: 6520 3d20 6f73 2e70 6174 682e 6a6f 696e  e = os.path.join
+00015280: 2866 6f6c 6465 7250 6174 682c 2066 227b  (folderPath, f"{
+00015290: 7469 6d65 7374 616d 707d 2e74 7874 2229  timestamp}.txt")
+000152a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000152b0: 2020 2020 2077 6974 6820 6f70 656e 2863       with open(c
+000152c0: 6861 7446 696c 652c 2022 7722 2c20 656e  hatFile, "w", en
+000152d0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+000152e0: 6173 2066 696c 654f 626a 3a0a 2020 2020  as fileObj:.    
+000152f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015300: 2020 2020 6669 6c65 4f62 6a2e 7772 6974      fileObj.writ
+00015310: 6528 7070 7269 6e74 2e70 666f 726d 6174  e(pprint.pformat
+00015320: 286d 6573 7361 6765 7343 6f70 7929 290a  (messagesCopy)).
+00015330: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00015340: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00015350: 2020 2020 7072 696e 7432 2822 4661 696c      print2("Fail
+00015360: 6564 2074 6f20 7361 7665 2063 6861 7421  ed to save chat!
+00015370: 5c6e 2229 0a20 2020 2020 2020 2020 2020  \n").           
+00015380: 2020 2020 2073 686f 7745 7272 6f72 7328       showErrors(
+00015390: 290a 0a20 2020 2064 6566 2065 7870 6f72  )..    def expor
+000153a0: 7443 6861 7428 7365 6c66 2c20 6d65 7373  tChat(self, mess
+000153b0: 6167 6573 2c20 6f70 656e 4669 6c65 3d54  ages, openFile=T
+000153c0: 7275 6529 3a0a 2020 2020 2020 2020 6966  rue):.        if
+000153d0: 2063 6f6e 6669 672e 636f 6e76 6572 7361   config.conversa
+000153e0: 7469 6f6e 5374 6172 7465 643a 0a20 2020  tionStarted:.   
+000153f0: 2020 2020 2020 2020 2070 6c61 696e 5465           plainTe
+00015400: 7874 203d 2022 220a 2020 2020 2020 2020  xt = "".        
+00015410: 2020 2020 7469 6d65 7374 616d 7020 3d20      timestamp = 
+00015420: 6765 7443 7572 7265 6e74 4461 7465 5469  getCurrentDateTi
+00015430: 6d65 2829 0a0a 2020 2020 2020 2020 2020  me()..          
+00015440: 2020 666f 7220 6920 696e 206d 6573 7361    for i in messa
+00015450: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+00015460: 2020 2020 2069 6620 695b 2272 6f6c 6522       if i["role"
+00015470: 5d20 3d3d 2022 7573 6572 223a 0a20 2020  ] == "user":.   
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2063 6f6e 7465 6e74 203d 2069 5b22 636f   content = i["co
+000154a0: 6e74 656e 7422 5d0a 2020 2020 2020 2020  ntent"].        
+000154b0: 2020 2020 2020 2020 2020 2020 706c 6169              plai
+000154c0: 6e54 6578 7420 2b3d 2066 223e 3e3e 207b  nText += f">>> {
+000154d0: 636f 6e74 656e 747d 220a 2020 2020 2020  content}".      
+000154e0: 2020 2020 2020 2020 2020 6966 2069 5b22            if i["
+000154f0: 726f 6c65 225d 203d 3d20 2266 756e 6374  role"] == "funct
+00015500: 696f 6e22 3a0a 2020 2020 2020 2020 2020  ion":.          
+00015510: 2020 2020 2020 2020 2020 6966 2070 6c61            if pla
+00015520: 696e 5465 7874 3a0a 2020 2020 2020 2020  inText:.        
+00015530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015540: 706c 6169 6e54 6578 7420 2b3d 2022 5c6e  plainText += "\n
+00015550: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
+00015560: 2020 2020 2020 2020 6e61 6d65 203d 2069          name = i
+00015570: 5b22 6e61 6d65 225d 0a20 2020 2020 2020  ["name"].       
+00015580: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00015590: 696e 5465 7874 202b 3d20 6622 6060 605c  inText += f"```\
+000155a0: 6e7b 6e61 6d65 7d5c 6e60 6060 220a 2020  n{name}\n```".  
+000155b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155c0: 2020 636f 6e74 656e 7420 3d20 695b 2263    content = i["c
+000155d0: 6f6e 7465 6e74 225d 0a20 2020 2020 2020  ontent"].       
+000155e0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000155f0: 696e 5465 7874 202b 3d20 6622 5c6e 5c6e  inText += f"\n\n
+00015600: 7b63 6f6e 7465 6e74 7d5c 6e5c 6e22 0a20  {content}\n\n". 
+00015610: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00015620: 6c69 6620 695b 2272 6f6c 6522 5d20 3d3d  lif i["role"] ==
+00015630: 2022 6173 7369 7374 616e 7422 3a0a 2020   "assistant":.  
+00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015650: 2020 636f 6e74 656e 7420 3d20 695b 2263    content = i["c
+00015660: 6f6e 7465 6e74 225d 0a20 2020 2020 2020  ontent"].       
+00015670: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015680: 636f 6e74 656e 7420 6973 206e 6f74 204e  content is not N
+00015690: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000156a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000156b0: 706c 6169 6e54 6578 743a 0a20 2020 2020  plainText:.     
+000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000156d0: 2020 2020 2020 2070 6c61 696e 5465 7874         plainText
+000156e0: 202b 3d20 225c 6e5c 6e22 0a20 2020 2020   += "\n\n".     
+000156f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015700: 2020 2070 6c61 696e 5465 7874 202b 3d20     plainText += 
+00015710: 6622 7b63 6f6e 7465 6e74 7d5c 6e5c 6e22  f"{content}\n\n"
+00015720: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
+00015730: 696e 5465 7874 203d 2070 6c61 696e 5465  inText = plainTe
+00015740: 7874 2e73 7472 6970 2829 0a20 2020 2020  xt.strip().     
+00015750: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+00015760: 2e74 6572 6d69 6e61 6c45 6e61 626c 6554  .terminalEnableT
+00015770: 6572 6d75 7841 5049 3a0a 2020 2020 2020  ermuxAPI:.      
+00015780: 2020 2020 2020 2020 2020 7079 646f 632e            pydoc.
+00015790: 7069 7065 7061 6765 7228 706c 6169 6e54  pipepager(plainT
+000157a0: 6578 742c 2063 6d64 3d22 7465 726d 7578  ext, cmd="termux
+000157b0: 2d73 6861 7265 202d 6120 7365 6e64 2229  -share -a send")
+000157c0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+000157d0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000157e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000157f0: 2020 2020 2020 2020 2020 2020 666f 6c64              fold
+00015800: 6572 5061 7468 203d 206f 732e 7061 7468  erPath = os.path
+00015810: 2e6a 6f69 6e28 636f 6e66 6967 2e6c 6f63  .join(config.loc
+00015820: 616c 5374 6f72 6167 652c 2022 6368 6174  alStorage, "chat
+00015830: 7322 2c20 2265 7870 6f72 7422 290a 2020  s", "export").  
+00015840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015850: 2020 5061 7468 2866 6f6c 6465 7250 6174    Path(folderPat
+00015860: 6829 2e6d 6b64 6972 2870 6172 656e 7473  h).mkdir(parents
+00015870: 3d54 7275 652c 2065 7869 7374 5f6f 6b3d  =True, exist_ok=
+00015880: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00015890: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
+000158a0: 7061 7468 2e69 7364 6972 2866 6f6c 6465  path.isdir(folde
+000158b0: 7250 6174 6829 3a0a 2020 2020 2020 2020  rPath):.        
+000158c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158d0: 6368 6174 4669 6c65 203d 206f 732e 7061  chatFile = os.pa
+000158e0: 7468 2e6a 6f69 6e28 666f 6c64 6572 5061  th.join(folderPa
+000158f0: 7468 2c20 6622 7b74 696d 6573 7461 6d70  th, f"{timestamp
+00015900: 7d2e 7478 7422 290a 2020 2020 2020 2020  }.txt").        
+00015910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015920: 7769 7468 206f 7065 6e28 6368 6174 4669  with open(chatFi
+00015930: 6c65 2c20 2277 222c 2065 6e63 6f64 696e  le, "w", encodin
+00015940: 673d 2275 7466 2d38 2229 2061 7320 6669  g="utf-8") as fi
+00015950: 6c65 4f62 6a3a 0a20 2020 2020 2020 2020  leObj:.         
+00015960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015970: 2020 2066 696c 654f 626a 2e77 7269 7465     fileObj.write
+00015980: 2870 6c61 696e 5465 7874 290a 2020 2020  (plainText).    
+00015990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159a0: 2020 2020 6966 206f 7065 6e46 696c 6520      if openFile 
+000159b0: 616e 6420 6f73 2e70 6174 682e 6973 6669  and os.path.isfi
+000159c0: 6c65 2863 6861 7446 696c 6529 3a0a 2020  le(chatFile):.  
+000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159e0: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
+000159f0: 7465 6d28 6627 2727 7b63 6f6e 6669 672e  tem(f'''{config.
+00015a00: 6f70 656e 7d20 227b 6368 6174 4669 6c65  open} "{chatFile
+00015a10: 7d22 2727 2729 0a20 2020 2020 2020 2020  }"''').         
+00015a20: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a40: 2020 2070 7269 6e74 3228 2246 6169 6c65     print2("Faile
+00015a50: 6420 746f 2073 6176 6520 6368 6174 215c  d to save chat!\
+00015a60: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00015a70: 2020 2020 2020 2020 7368 6f77 4572 726f          showErro
+00015a80: 7273 2829 0a0a 2020 2020 6465 6620 7275  rs()..    def ru
+00015a90: 6e49 6e73 7472 7563 7469 6f6e 2873 656c  nInstruction(sel
+00015aa0: 6629 3a0a 2020 2020 2020 2020 696e 7374  f):.        inst
+00015ab0: 7275 6374 696f 6e73 203d 206c 6973 7428  ructions = list(
+00015ac0: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
+00015ad0: 6449 6e73 7472 7563 7469 6f6e 732e 6b65  dInstructions.ke
+00015ae0: 7973 2829 290a 2020 2020 2020 2020 696e  ys()).        in
+00015af0: 7374 7275 6374 696f 6e20 3d20 7365 6c66  struction = self
+00015b00: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
+00015b10: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
+00015b20: 2020 2020 2020 6f70 7469 6f6e 733d 696e        options=in
+00015b30: 7374 7275 6374 696f 6e73 2c0a 2020 2020  structions,.    
+00015b40: 2020 2020 2020 2020 7469 746c 653d 2250          title="P
+00015b50: 7265 6465 6669 6e65 6420 496e 7374 7275  redefined Instru
+00015b60: 6374 696f 6e73 222c 0a20 2020 2020 2020  ctions",.       
+00015b70: 2020 2020 2074 6578 743d 2253 656c 6563       text="Selec
+00015b80: 7420 616e 2069 6e73 7472 7563 7469 6f6e  t an instruction
+00015b90: 3a22 2c0a 2020 2020 2020 2020 290a 2020  :",.        ).  
+00015ba0: 2020 2020 2020 6966 2069 6e73 7472 7563        if instruc
+00015bb0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00015bc0: 2020 636f 6e66 6967 2e64 6566 6175 6c74    config.default
+00015bd0: 456e 7472 7920 3d20 636f 6e66 6967 2e70  Entry = config.p
+00015be0: 7265 6465 6669 6e65 6449 6e73 7472 7563  redefinedInstruc
+00015bf0: 7469 6f6e 735b 696e 7374 7275 6374 696f  tions[instructio
+00015c00: 6e5d 0a20 2020 2020 2020 2020 2020 2063  n].            c
+00015c10: 6f6e 6669 672e 6163 6365 7074 5f64 6566  onfig.accept_def
+00015c20: 6175 6c74 203d 2054 7275 650a 0a20 2020  ault = True..   
+00015c30: 2064 6566 2063 6861 6e67 6543 6f6e 7465   def changeConte
+00015c40: 7874 2873 656c 6629 3a0a 2020 2020 2020  xt(self):.      
+00015c50: 2020 636f 6e74 6578 7473 203d 206c 6973    contexts = lis
+00015c60: 7428 636f 6e66 6967 2e70 7265 6465 6669  t(config.predefi
+00015c70: 6e65 6443 6f6e 7465 7874 732e 6b65 7973  nedContexts.keys
+00015c80: 2829 290a 2020 2020 2020 2020 7072 6564  ()).        pred
+00015c90: 6566 696e 6564 436f 6e74 6578 7420 3d20  efinedContext = 
+00015ca0: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
+00015cb0: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
+00015cc0: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+00015cd0: 733d 636f 6e74 6578 7473 2c0a 2020 2020  s=contexts,.    
+00015ce0: 2020 2020 2020 2020 7469 746c 653d 2250          title="P
+00015cf0: 7265 6465 6669 6e65 6420 436f 6e74 6578  redefined Contex
+00015d00: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
+00015d10: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+00015d20: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
+00015d30: 742c 0a20 2020 2020 2020 2020 2020 2074  t,.            t
+00015d40: 6578 743d 2253 656c 6563 7420 6120 636f  ext="Select a co
+00015d50: 6e74 6578 743a 222c 0a20 2020 2020 2020  ntext:",.       
+00015d60: 2029 0a20 2020 2020 2020 2069 6620 7072   ).        if pr
+00015d70: 6564 6566 696e 6564 436f 6e74 6578 743a  edefinedContext:
+00015d80: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00015d90: 6669 672e 7072 6564 6566 696e 6564 436f  fig.predefinedCo
+00015da0: 6e74 6578 7420 3d20 7072 6564 6566 696e  ntext = predefin
+00015db0: 6564 436f 6e74 6578 740a 2020 2020 2020  edContext.      
+00015dc0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+00015dd0: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
+00015de0: 7420 3d3d 2022 5b63 7573 746f 6d5d 223a  t == "[custom]":
+00015df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e00: 2070 7269 6e74 3128 2245 6469 7420 6375   print1("Edit cu
+00015e10: 7374 6f6d 2063 6f6e 7465 7874 2062 656c  stom context bel
+00015e20: 6f77 3a22 290a 2020 2020 2020 2020 2020  ow:").          
+00015e30: 2020 2020 2020 6375 7374 6f6d 436f 6e74        customCont
+00015e40: 6578 7420 3d20 7365 6c66 2e70 726f 6d70  ext = self.promp
+00015e50: 7473 2e73 696d 706c 6550 726f 6d70 7428  ts.simplePrompt(
+00015e60: 7374 796c 653d 7365 6c66 2e70 726f 6d70  style=self.promp
+00015e70: 7473 2e70 726f 6d70 7453 7479 6c65 322c  ts.promptStyle2,
+00015e80: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+00015e90: 6375 7374 6f6d 5072 6564 6566 696e 6564  customPredefined
+00015ea0: 436f 6e74 6578 7429 0a20 2020 2020 2020  Context).       
+00015eb0: 2020 2020 2020 2020 2069 6620 6375 7374           if cust
+00015ec0: 6f6d 436f 6e74 6578 7420 616e 6420 6e6f  omContext and no
+00015ed0: 7420 6375 7374 6f6d 436f 6e74 6578 742e  t customContext.
+00015ee0: 7374 7269 7028 292e 6c6f 7765 7228 2920  strip().lower() 
+00015ef0: 3d3d 2063 6f6e 6669 672e 6578 6974 5f65  == config.exit_e
+00015f00: 6e74 7279 3a0a 2020 2020 2020 2020 2020  ntry:.          
+00015f10: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00015f20: 2e63 7573 746f 6d50 7265 6465 6669 6e65  .customPredefine
+00015f30: 6443 6f6e 7465 7874 203d 2063 7573 746f  dContext = custo
+00015f40: 6d43 6f6e 7465 7874 2e73 7472 6970 2829  mContext.strip()
+00015f50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00015f60: 2020 2020 2020 2020 2020 2023 2061 2077             # a w
+00015f70: 6179 2074 6f20 7175 6963 6b6c 7920 636c  ay to quickly cl
+00015f80: 6561 6e20 7570 2063 6f6e 7465 7874 0a20  ean up context. 
+00015f90: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00015fa0: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
+00015fb0: 6578 7420 3d20 225b 6e6f 6e65 5d22 0a20  ext = "[none]". 
+00015fc0: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+00015fd0: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
+00015fe0: 2020 2073 656c 662e 7368 6f77 4375 7272     self.showCurr
+00015ff0: 656e 7443 6f6e 7465 7874 2829 0a0a 2020  entContext()..  
+00016000: 2020 6465 6620 6765 7444 6972 6563 746f    def getDirecto
+00016010: 7279 4c69 7374 2873 656c 6629 3a0a 2020  ryList(self):.  
+00016020: 2020 2020 2020 6469 7265 6374 6f72 794c        directoryL
+00016030: 6973 7420 3d20 5b5d 0a20 2020 2020 2020  ist = [].       
+00016040: 2066 6f72 2066 2069 6e20 6f73 2e6c 6973   for f in os.lis
+00016050: 7464 6972 2827 2e27 293a 0a20 2020 2020  tdir('.'):.     
+00016060: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00016070: 682e 6973 6469 7228 6629 3a0a 2020 2020  h.isdir(f):.    
+00016080: 2020 2020 2020 2020 2020 2020 7365 7061              sepa
+00016090: 7261 746f 7220 3d20 225c 5c22 2069 6620  rator = "\\" if 
+000160a0: 636f 6e66 6967 2e74 6869 7350 6c61 7466  config.thisPlatf
+000160b0: 6f72 6d20 3d3d 2022 5769 6e64 6f77 7322  orm == "Windows"
+000160c0: 2065 6c73 6520 222f 220a 2020 2020 2020   else "/".      
+000160d0: 2020 2020 2020 2020 2020 6469 7265 6374            direct
+000160e0: 6f72 794c 6973 742e 6170 7065 6e64 2866  oryList.append(f
+000160f0: 227b 667d 7b73 6570 6172 6174 6f72 7d22  "{f}{separator}"
+00016100: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00016110: 6966 206f 732e 7061 7468 2e69 7366 696c  if os.path.isfil
+00016120: 6528 6629 3a0a 2020 2020 2020 2020 2020  e(f):.          
+00016130: 2020 2020 2020 6469 7265 6374 6f72 794c        directoryL
+00016140: 6973 742e 6170 7065 6e64 2866 290a 2020  ist.append(f).  
+00016150: 2020 2020 2020 7265 7475 726e 2064 6972        return dir
+00016160: 6563 746f 7279 4c69 7374 0a0a 2020 2020  ectoryList..    
+00016170: 6465 6620 7368 6f77 4c6f 676f 2873 656c  def showLogo(sel
+00016180: 6629 3a0a 2020 2020 2020 2020 6170 704e  f):.        appN
+00016190: 616d 6520 3d20 636f 6e66 6967 2e66 7265  ame = config.fre
+000161a0: 6547 656e 6975 7341 494e 616d 652e 7370  eGeniusAIName.sp
+000161b0: 6c69 7428 295b 305d 2e75 7070 6572 2829  lit()[0].upper()
+000161c0: 0a20 2020 2020 2020 2074 6572 6d69 6e61  .        termina
+000161d0: 6c5f 7769 6474 6820 3d20 7368 7574 696c  l_width = shutil
+000161e0: 2e67 6574 5f74 6572 6d69 6e61 6c5f 7369  .get_terminal_si
+000161f0: 7a65 2829 2e63 6f6c 756d 6e73 0a20 2020  ze().columns.   
+00016200: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00016210: 2020 2020 2020 6672 6f6d 2061 7274 2069        from art i
+00016220: 6d70 6f72 7420 7465 7874 3261 7274 0a20  mport text2art. 
+00016230: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00016240: 726d 696e 616c 5f77 6964 7468 203e 3d20  rminal_width >= 
+00016250: 3332 3a0a 2020 2020 2020 2020 2020 2020  32:.            
+00016260: 2020 2020 6c6f 676f 203d 2074 6578 7432      logo = text2
+00016270: 6172 7428 6170 704e 616d 652c 2066 6f6e  art(appName, fon
+00016280: 743d 2263 7962 6572 6d65 6475 6d22 290a  t="cybermedum").
+00016290: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000162a0: 2074 6572 6d69 6e61 6c5f 7769 6474 6820   terminal_width 
+000162b0: 3e3d 2032 303a 0a20 2020 2020 2020 2020  >= 20:.         
+000162c0: 2020 2020 2020 206c 6f67 6f20 3d20 7465         logo = te
+000162d0: 7874 3261 7274 2822 2022 2e6a 6f69 6e28  xt2art(" ".join(
+000162e0: 6170 704e 616d 6529 202b 2022 2022 2c20  appName) + " ", 
+000162f0: 666f 6e74 3d22 7768 6974 655f 6275 6262  font="white_bubb
+00016300: 6c65 2229 0a20 2020 2020 2020 2020 2020  le").           
+00016310: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00016320: 2020 2020 2020 206c 6f67 6f20 3d20 636f         logo = co
+00016330: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
+00016340: 494e 616d 650a 2020 2020 2020 2020 2020  IName.          
+00016350: 2020 6c6f 676f 203d 206c 6f67 6f5b 3a2d    logo = logo[:-
+00016360: 315d 2023 2072 656d 6f76 6520 7468 6520  1] # remove the 
+00016370: 6c69 6e65 6272 6561 6b20 6174 2074 6865  linebreak at the
+00016380: 2065 6e64 0a20 2020 2020 2020 2065 7863   end.        exc
+00016390: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+000163a0: 206c 6f67 6f20 3d20 636f 6e66 6967 2e66   logo = config.f
+000163b0: 7265 6547 656e 6975 7341 494e 616d 650a  reeGeniusAIName.
+000163c0: 2020 2020 2020 2020 7072 696e 745f 666f          print_fo
+000163d0: 726d 6174 7465 645f 7465 7874 2848 544d  rmatted_text(HTM
+000163e0: 4c28 6622 3c7b 636f 6e66 6967 2e74 6572  L(f"<{config.ter
+000163f0: 6d69 6e61 6c43 6f6d 6d61 6e64 456e 7472  minalCommandEntr
+00016400: 7943 6f6c 6f72 327d 3e7b 6c6f 676f 7d3c  yColor2}>{logo}<
+00016410: 2f7b 636f 6e66 6967 2e74 6572 6d69 6e61  /{config.termina
+00016420: 6c43 6f6d 6d61 6e64 456e 7472 7943 6f6c  lCommandEntryCol
+00016430: 6f72 327d 3e22 2929 0a0a 2020 2020 6465  or2}>"))..    de
+00016440: 6620 7275 6e50 7974 686f 6e53 6372 6970  f runPythonScrip
+00016450: 7428 7365 6c66 2c20 7363 7269 7074 293a  t(self, script):
+00016460: 0a20 2020 2020 2020 2073 6372 6970 7420  .        script 
+00016470: 3d20 7363 7269 7074 2e73 7472 6970 2829  = script.strip()
+00016480: 5b33 3a2d 335d 0a20 2020 2020 2020 2074  [3:-3].        t
+00016490: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000164a0: 6578 6563 2873 6372 6970 742c 2067 6c6f  exec(script, glo
+000164b0: 6261 6c73 2829 290a 2020 2020 2020 2020  bals()).        
+000164c0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000164d0: 2020 2020 7472 6163 6520 3d20 7472 6163      trace = trac
+000164e0: 6562 6163 6b2e 666f 726d 6174 5f65 7863  eback.format_exc
+000164f0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+00016500: 7269 6e74 2874 7261 6365 2069 6620 636f  rint(trace if co
+00016510: 6e66 6967 2e64 6576 656c 6f70 6572 2065  nfig.developer e
+00016520: 6c73 6520 2245 7272 6f72 2065 6e63 6f75  lse "Error encou
+00016530: 6e74 6572 6564 2122 290a 2020 2020 2020  ntered!").      
+00016540: 2020 2020 2020 7072 696e 7431 2863 6f6e        print1(con
+00016550: 6669 672e 6469 7669 6465 7229 0a20 2020  fig.divider).   
+00016560: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
+00016570: 6967 2e6d 6178 5f63 6f6e 7365 6375 7469  ig.max_consecuti
+00016580: 7665 5f61 7574 6f5f 636f 7272 6563 7469  ve_auto_correcti
+00016590: 6f6e 203e 2030 3a0a 2020 2020 2020 2020  on > 0:.        
+000165a0: 2020 2020 2020 2020 4361 6c6c 4c4c 4d2e          CallLLM.
+000165b0: 6175 746f 436f 7272 6563 7450 7974 686f  autoCorrectPytho
+000165c0: 6e43 6f64 6528 7363 7269 7074 2c20 7472  nCode(script, tr
+000165d0: 6163 6529 0a0a 2020 2020 6465 6620 7374  ace)..    def st
+000165e0: 6172 7443 6861 7473 2873 656c 6629 3a0a  artChats(self):.
+000165f0: 2020 2020 2020 2020 746f 6b65 6e56 616c          tokenVal
+00016600: 6964 6174 6f72 203d 2054 6f6b 656e 5661  idator = TokenVa
+00016610: 6c69 6461 746f 7228 290a 2020 2020 2020  lidator().      
+00016620: 2020 6465 6620 6765 7444 796e 616d 6963    def getDynamic
+00016630: 546f 6f6c 4261 7228 293a 0a20 2020 2020  ToolBar():.     
+00016640: 2020 2020 2020 2072 6574 7572 6e20 636f         return co
+00016650: 6e66 6967 2e64 796e 616d 6963 546f 6f6c  nfig.dynamicTool
+00016660: 4261 7254 6578 740a 2020 2020 2020 2020  BarText.        
+00016670: 6465 6620 7374 6172 7443 6861 7428 293a  def startChat():
+00016680: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
+00016690: 6172 2829 0a20 2020 2020 2020 2020 2020  ar().           
+000166a0: 2070 7269 6e74 3128 7365 6c66 2e64 6976   print1(self.div
+000166b0: 6964 6572 290a 2020 2020 2020 2020 2020  ider).          
+000166c0: 2020 7365 6c66 2e73 686f 774c 6f67 6f28    self.showLogo(
+000166d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000166e0: 6c66 2e73 686f 7743 7572 7265 6e74 436f  lf.showCurrentCo
+000166f0: 6e74 6578 7428 290a 2020 2020 2020 2020  ntext().        
+00016700: 2020 2020 2320 676f 2074 6f20 7374 6172      # go to star
+00016710: 7475 7020 6469 7265 6374 6f72 790a 2020  tup directory.  
+00016720: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+00016730: 6564 6972 6563 746f 7279 203d 2063 6f6e  edirectory = con
+00016740: 6669 672e 6c6f 6361 6c53 746f 7261 6765  fig.localStorage
+00016750: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
+00016760: 6368 6469 7228 7374 6f72 6167 6564 6972  chdir(storagedir
+00016770: 6563 746f 7279 290a 2020 2020 2020 2020  ectory).        
+00016780: 2020 2020 6d65 7373 6167 6573 203d 2043      messages = C
+00016790: 616c 6c4c 4c4d 2e72 6573 6574 4d65 7373  allLLM.resetMess
+000167a0: 6167 6573 2829 0a20 2020 2020 2020 2020  ages().         
+000167b0: 2020 2023 7072 696e 7431 2866 2273 7461     #print1(f"sta
+000167c0: 7274 7570 2064 6972 6563 746f 7279 3a5c  rtup directory:\
+000167d0: 6e7b 7374 6f72 6167 6564 6972 6563 746f  n{storagedirecto
+000167e0: 7279 7d22 290a 2020 2020 2020 2020 2020  ry}").          
+000167f0: 2020 7072 696e 745f 666f 726d 6174 7465    print_formatte
+00016800: 645f 7465 7874 2848 544d 4c28 6622 3c7b  d_text(HTML(f"<{
+00016810: 636f 6e66 6967 2e74 6572 6d69 6e61 6c50  config.terminalP
+00016820: 726f 6d70 7449 6e64 6963 6174 6f72 436f  romptIndicatorCo
+00016830: 6c6f 7232 7d3e 4469 7265 6374 6f72 793a  lor2}>Directory:
+00016840: 3c2f 7b63 6f6e 6669 672e 7465 726d 696e  </{config.termin
+00016850: 616c 5072 6f6d 7074 496e 6469 6361 746f  alPromptIndicato
+00016860: 7243 6f6c 6f72 327d 3e20 7b73 746f 7261  rColor2}> {stora
+00016870: 6765 6469 7265 6374 6f72 797d 2229 290a  gedirectory}")).
+00016880: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00016890: 7431 2873 656c 662e 6469 7669 6465 7229  t1(self.divider)
+000168a0: 0a0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000168b0: 6e66 6967 2e63 6f6e 7665 7273 6174 696f  nfig.conversatio
+000168c0: 6e53 7461 7274 6564 203d 2046 616c 7365  nStarted = False
+000168d0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000168e0: 7572 6e20 2873 746f 7261 6765 6469 7265  urn (storagedire
+000168f0: 6374 6f72 792c 206d 6573 7361 6765 7329  ctory, messages)
+00016900: 0a20 2020 2020 2020 2073 746f 7261 6765  .        storage
+00016910: 6469 7265 6374 6f72 792c 2063 6f6e 6669  directory, confi
+00016920: 672e 6375 7272 656e 744d 6573 7361 6765  g.currentMessage
+00016930: 7320 3d20 7374 6172 7443 6861 7428 290a  s = startChat().
+00016940: 2020 2020 2020 2020 636f 6e66 6967 2e6d          config.m
+00016950: 756c 7469 6c69 6e65 496e 7075 7420 3d20  ultilineInput = 
+00016960: 4661 6c73 650a 2020 2020 2020 2020 6665  False.        fe
+00016970: 6174 7572 6573 4c6f 7765 7220 3d20 6c69  aturesLower = li
+00016980: 7374 2873 656c 662e 6163 7469 6f6e 732e  st(self.actions.
+00016990: 6b65 7973 2829 2920 2b20 5b22 2e2e 2e22  keys()) + ["..."
+000169a0: 5d0a 2020 2020 2020 2020 2320 696e 7075  ].        # inpu
+000169b0: 7420 7375 6767 6573 7469 6f6e 730a 2020  t suggestions.  
+000169c0: 2020 2020 2020 636f 6e66 6967 2e69 6e70        config.inp
+000169d0: 7574 5375 6767 6573 7469 6f6e 7320 2b3d  utSuggestions +=
+000169e0: 2066 6561 7475 7265 734c 6f77 6572 0a20   featuresLower. 
+000169f0: 2020 2020 2020 2063 6f6d 706c 6574 6572         completer
+00016a00: 203d 2046 757a 7a79 436f 6d70 6c65 7465   = FuzzyComplete
+00016a10: 7228 576f 7264 436f 6d70 6c65 7465 7228  r(WordCompleter(
+00016a20: 636f 6e66 6967 2e69 6e70 7574 5375 6767  config.inputSugg
+00016a30: 6573 7469 6f6e 732c 2069 676e 6f72 655f  estions, ignore_
+00016a40: 6361 7365 3d54 7275 6529 2920 6966 2063  case=True)) if c
+00016a50: 6f6e 6669 672e 696e 7075 7453 7567 6765  onfig.inputSugge
+00016a60: 7374 696f 6e73 2065 6c73 6520 4e6f 6e65  stions else None
+00016a70: 0a20 2020 2020 2020 2063 6f6d 706c 6574  .        complet
+00016a80: 6572 5f64 6576 656c 6f70 6572 203d 2046  er_developer = F
+00016a90: 757a 7a79 436f 6d70 6c65 7465 7228 576f  uzzyCompleter(Wo
+00016aa0: 7264 436f 6d70 6c65 7465 7228 636f 6e66  rdCompleter(conf
+00016ab0: 6967 2e69 6e70 7574 5375 6767 6573 7469  ig.inputSuggesti
+00016ac0: 6f6e 735b 3a5d 202b 205b 6622 636f 6e66  ons[:] + [f"conf
+00016ad0: 6967 2e7b 697d 2220 666f 7220 6920 696e  ig.{i}" for i in
+00016ae0: 2064 6972 2863 6f6e 6669 6729 2069 6620   dir(config) if 
+00016af0: 6e6f 7420 692e 7374 6172 7473 7769 7468  not i.startswith
+00016b00: 2822 5f5f 2229 5d20 2b20 7365 6c66 2e67  ("__")] + self.g
+00016b10: 6574 4469 7265 6374 6f72 794c 6973 7428  etDirectoryList(
+00016b20: 292c 2069 676e 6f72 655f 6361 7365 3d54  ), ignore_case=T
+00016b30: 7275 6529 290a 2020 2020 2020 2020 7768  rue)).        wh
+00016b40: 696c 6520 5472 7565 3a0a 2020 2020 2020  ile True:.      
+00016b50: 2020 2020 2020 2320 6465 6661 756c 7420        # default 
+00016b60: 746f 6f6c 6261 7220 7465 7874 0a20 2020  toolbar text.   
+00016b70: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+00016b80: 6479 6e61 6d69 6354 6f6f 6c42 6172 5465  dynamicToolBarTe
+00016b90: 7874 203d 2066 2222 2220 7b73 7472 2863  xt = f""" {str(c
+00016ba0: 6f6e 6669 672e 686f 746b 6579 5f65 7869  onfig.hotkey_exi
+00016bb0: 7429 2e72 6570 6c61 6365 2822 2722 2c20  t).replace("'", 
+00016bc0: 2222 297d 2065 7869 7420 7b73 7472 2863  "")} exit {str(c
+00016bd0: 6f6e 6669 672e 686f 746b 6579 5f64 6973  onfig.hotkey_dis
+00016be0: 706c 6179 5f6b 6579 5f63 6f6d 626f 292e  play_key_combo).
+00016bf0: 7265 706c 6163 6528 2227 222c 2022 2229  replace("'", "")
+00016c00: 7d20 7368 6f72 7463 7574 7320 2222 220a  } shortcuts """.
+00016c10: 2020 2020 2020 2020 2020 2020 2320 6469              # di
+00016c20: 7370 6c61 7920 6375 7272 656e 7420 6469  splay current di
+00016c30: 7265 6374 6f72 7920 6966 2063 6861 6e67  rectory if chang
+00016c40: 6564 0a20 2020 2020 2020 2020 2020 2063  ed.            c
+00016c50: 7572 7265 6e74 4469 7265 6374 6f72 7920  urrentDirectory 
+00016c60: 3d20 6f73 2e67 6574 6377 6428 290a 2020  = os.getcwd().  
+00016c70: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00016c80: 2063 7572 7265 6e74 4469 7265 6374 6f72   currentDirector
+00016c90: 7920 3d3d 2073 746f 7261 6765 6469 7265  y == storagedire
+00016ca0: 6374 6f72 793a 0a20 2020 2020 2020 2020  ctory:.         
+00016cb0: 2020 2020 2020 2023 7072 696e 7431 2873         #print1(s
+00016cc0: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00016cd0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00016ce0: 6e74 3328 6622 4375 7272 656e 7420 6469  nt3(f"Current di
+00016cf0: 7265 6374 6f72 793a 207b 6375 7272 656e  rectory: {curren
+00016d00: 7444 6972 6563 746f 7279 7d22 290a 2020  tDirectory}").  
+00016d10: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00016d20: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
+00016d30: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+00016d40: 2020 2073 746f 7261 6765 6469 7265 6374     storagedirect
+00016d50: 6f72 7920 3d20 6375 7272 656e 7444 6972  ory = currentDir
+00016d60: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+00016d70: 2020 2023 2064 6566 6175 6c74 2069 6e70     # default inp
+00016d80: 7574 2065 6e74 7279 0a20 2020 2020 2020  ut entry.       
+00016d90: 2020 2020 2061 6363 6570 745f 6465 6661       accept_defa
+00016da0: 756c 7420 3d20 636f 6e66 6967 2e61 6363  ult = config.acc
+00016db0: 6570 745f 6465 6661 756c 740a 2020 2020  ept_default.    
+00016dc0: 2020 2020 2020 2020 636f 6e66 6967 2e61          config.a
+00016dd0: 6363 6570 745f 6465 6661 756c 7420 3d20  ccept_default = 
+00016de0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00016df0: 2020 6465 6661 756c 7445 6e74 7279 203d    defaultEntry =
+00016e00: 2063 6f6e 6669 672e 6465 6661 756c 7445   config.defaultE
+00016e10: 6e74 7279 0a20 2020 2020 2020 2020 2020  ntry.           
+00016e20: 2069 6620 6f73 2e70 6174 682e 6973 6669   if os.path.isfi
+00016e30: 6c65 2864 6566 6175 6c74 456e 7472 7929  le(defaultEntry)
+00016e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016e50: 2020 6465 6661 756c 7445 6e74 7279 203d    defaultEntry =
+00016e60: 2066 2746 696c 653a 2022 7b64 6566 6175   f'File: "{defau
+00016e70: 6c74 456e 7472 797d 225c 6e27 0a20 2020  ltEntry}"\n'.   
+00016e80: 2020 2020 2020 2020 2065 6c69 6620 6f73           elif os
+00016e90: 2e70 6174 682e 6973 6469 7228 6465 6661  .path.isdir(defa
+00016ea0: 756c 7445 6e74 7279 293a 0a20 2020 2020  ultEntry):.     
+00016eb0: 2020 2020 2020 2020 2020 2064 6566 6175             defau
+00016ec0: 6c74 456e 7472 7920 3d20 6627 466f 6c64  ltEntry = f'Fold
+00016ed0: 6572 3a20 227b 6465 6661 756c 7445 6e74  er: "{defaultEnt
+00016ee0: 7279 7d22 5c6e 270a 2020 2020 2020 2020  ry}"\n'.        
+00016ef0: 2020 2020 636f 6e66 6967 2e64 6566 6175      config.defau
+00016f00: 6c74 456e 7472 7920 3d20 2222 0a0a 2020  ltEntry = ""..  
+00016f10: 2020 2020 2020 2020 2020 2320 7573 6572            # user
+00016f20: 2069 6e70 7574 0a20 2020 2020 2020 2020   input.         
+00016f30: 2020 2075 7365 7249 6e70 7574 203d 2073     userInput = s
+00016f40: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
+00016f50: 6c65 5072 6f6d 7074 2870 726f 6d70 7453  lePrompt(promptS
+00016f60: 6573 7369 6f6e 3d73 656c 662e 7465 726d  ession=self.term
+00016f70: 696e 616c 5f63 6861 745f 7365 7373 696f  inal_chat_sessio
+00016f80: 6e2c 2063 6f6d 706c 6574 6572 3d63 6f6d  n, completer=com
+00016f90: 706c 6574 6572 5f64 6576 656c 6f70 6572  pleter_developer
+00016fa0: 2069 6620 636f 6e66 6967 2e64 6576 656c   if config.devel
+00016fb0: 6f70 6572 2065 6c73 6520 636f 6d70 6c65  oper else comple
+00016fc0: 7465 722c 2064 6566 6175 6c74 3d64 6566  ter, default=def
+00016fd0: 6175 6c74 456e 7472 792c 2061 6363 6570  aultEntry, accep
+00016fe0: 745f 6465 6661 756c 743d 6163 6365 7074  t_default=accept
+00016ff0: 5f64 6566 6175 6c74 2c20 7661 6c69 6461  _default, valida
+00017000: 746f 723d 746f 6b65 6e56 616c 6964 6174  tor=tokenValidat
+00017010: 6f72 2c20 626f 7474 6f6d 5f74 6f6f 6c62  or, bottom_toolb
+00017020: 6172 3d67 6574 4479 6e61 6d69 6354 6f6f  ar=getDynamicToo
+00017030: 6c42 6172 290a 2020 2020 2020 2020 2020  lBar).          
+00017040: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
+00017050: 2075 7064 6174 6520 7379 7374 656d 206d   update system m
+00017060: 6573 7361 6765 2077 6865 6e20 7573 6572  essage when user
+00017070: 2065 6e74 6572 2061 206e 6577 2069 6e70   enter a new inp
+00017080: 7574 0a20 2020 2020 2020 2020 2020 2063  ut.            c
+00017090: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
+000170a0: 7361 6765 7320 3d20 7365 6c66 2e75 7064  sages = self.upd
+000170b0: 6174 6553 7973 7465 6d4d 6573 7361 6765  ateSystemMessage
+000170c0: 2863 6f6e 6669 672e 6375 7272 656e 744d  (config.currentM
+000170d0: 6573 7361 6765 7329 0a20 2020 2020 2020  essages).       
+000170e0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+000170f0: 2020 2320 6469 7370 6c61 7920 6f70 7469    # display opti
+00017100: 6f6e 7320 7768 656e 2065 6d70 7479 2073  ons when empty s
+00017110: 7472 696e 6720 6973 2065 6e74 6572 6564  tring is entered
+00017120: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00017130: 7249 6e70 7574 4c6f 7765 7220 3d20 7573  rInputLower = us
+00017140: 6572 496e 7075 742e 6c6f 7765 7228 290a  erInput.lower().
+00017150: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00017160: 6f6e 6669 672e 6164 6450 6174 6841 7420  onfig.addPathAt 
+00017170: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00017180: 2020 2020 2020 2020 2020 2020 2070 7265               pre
+00017190: 6669 7820 3d20 7573 6572 496e 7075 745b  fix = userInput[
+000171a0: 3a63 6f6e 6669 672e 6164 6450 6174 6841  :config.addPathA
+000171b0: 745d 0a20 2020 2020 2020 2020 2020 2020  t].             
+000171c0: 2020 2070 7265 6669 7853 706c 6974 203d     prefixSplit =
+000171d0: 2070 7265 6669 782e 7273 706c 6974 2822   prefix.rsplit("
+000171e0: 2022 2c20 3129 0a20 2020 2020 2020 2020   ", 1).         
+000171f0: 2020 2020 2020 2069 6620 6c65 6e28 7072         if len(pr
+00017200: 6566 6978 5370 6c69 7429 203e 2031 3a0a  efixSplit) > 1:.
+00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017220: 2020 2020 6465 6661 756c 7420 3d20 7072      default = pr
+00017230: 6566 6978 5370 6c69 745b 2d31 5d0a 2020  efixSplit[-1].  
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 7072 6566 6978 203d 2066 227b 7072    prefix = f"{pr
+00017260: 6566 6978 5370 6c69 745b 305d 7d20 220a  efixSplit[0]} ".
 00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017280: 6465 6661 756c 7420 3d20 7072 6566 6978  default = prefix
-00017290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172a0: 2020 2020 2070 7265 6669 7820 3d20 2222       prefix = ""
-000172b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000172c0: 2073 7566 6669 7820 3d20 7573 6572 496e   suffix = userIn
-000172d0: 7075 745b 636f 6e66 6967 2e61 6464 5061  put[config.addPa
-000172e0: 7468 4174 3a5d 0a20 2020 2020 2020 2020  thAt:].         
-000172f0: 2020 2020 2020 2063 6f6e 6669 672e 6164         config.ad
-00017300: 6450 6174 6841 7420 3d20 4e6f 6e65 0a20  dPathAt = None. 
-00017310: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00017320: 6620 6e6f 7420 6465 6661 756c 743a 0a20  f not default:. 
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2064 6566 6175 6c74 203d 206f 732e     default = os.
-00017350: 6765 7463 7764 2829 0a20 2020 2020 2020  getcwd().       
-00017360: 2020 2020 2020 2020 2075 7365 7250 6174           userPat
-00017370: 6820 3d20 7365 6c66 2e67 6574 5061 7468  h = self.getPath
-00017380: 2e67 6574 5061 7468 286d 6573 7361 6765  .getPath(message
-00017390: 3d66 227b 7072 6566 6978 7d3c 7b63 6f6e  =f"{prefix}<{con
-000173a0: 6669 672e 7465 726d 696e 616c 436f 6d6d  fig.terminalComm
-000173b0: 616e 6445 6e74 7279 436f 6c6f 7232 7d3e  andEntryColor2}>
-000173c0: 5b61 6464 2061 2070 6174 6820 6865 7265  [add a path here
-000173d0: 5d3c 2f7b 636f 6e66 6967 2e74 6572 6d69  ]</{config.termi
-000173e0: 6e61 6c43 6f6d 6d61 6e64 456e 7472 7943  nalCommandEntryC
-000173f0: 6f6c 6f72 327d 3e7b 7375 6666 6978 7d22  olor2}>{suffix}"
-00017400: 2c20 7072 6f6d 7074 496e 6469 6361 746f  , promptIndicato
-00017410: 723d 223e 3e3e 2022 2c20 656d 7074 795f  r=">>> ", empty_
-00017420: 746f 5f63 616e 6365 6c3d 5472 7565 2c20  to_cancel=True, 
-00017430: 6465 6661 756c 743d 6465 6661 756c 7429  default=default)
-00017440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017450: 2063 6f6e 6669 672e 6465 6661 756c 7445   config.defaultE
-00017460: 6e74 7279 203d 2066 227b 7072 6566 6978  ntry = f"{prefix
-00017470: 7d7b 7573 6572 5061 7468 7d7b 7375 6666  }{userPath}{suff
-00017480: 6978 7d22 0a20 2020 2020 2020 2020 2020  ix}".           
-00017490: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
-000174a0: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-000174b0: 656c 6966 206e 6f74 2075 7365 7249 6e70  elif not userInp
-000174c0: 7574 4c6f 7765 723a 0a20 2020 2020 2020  utLower:.       
-000174d0: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
-000174e0: 7574 203d 2063 6f6e 6669 672e 626c 616e  ut = config.blan
-000174f0: 6b45 6e74 7279 4163 7469 6f6e 0a20 2020  kEntryAction.   
-00017500: 2020 2020 2020 2020 2069 6620 7573 6572           if user
-00017510: 496e 7075 7420 3d3d 2022 2e2e 2e22 3a0a  Input == "...":.
-00017520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017530: 7573 6572 496e 7075 7420 3d20 7573 6572  userInput = user
-00017540: 496e 7075 744c 6f77 6572 203d 2073 656c  InputLower = sel
-00017550: 662e 7275 6e41 6374 696f 6e73 2875 7365  f.runActions(use
-00017560: 7249 6e70 7574 290a 2020 2020 2020 2020  rInput).        
-00017570: 2020 2020 2365 6c69 6620 7573 6572 496e      #elif userIn
-00017580: 7075 744c 6f77 6572 2069 6e20 7475 706c  putLower in tupl
-00017590: 6528 7365 6c66 2e61 6374 696f 6e73 2e6b  e(self.actions.k
-000175a0: 6579 7328 2929 3a0a 2020 2020 2020 2020  eys()):.        
-000175b0: 2020 2020 656c 6966 2075 7365 7249 6e70      elif userInp
-000175c0: 7574 4c6f 7765 722e 7374 6172 7473 7769  utLower.startswi
-000175d0: 7468 2822 2e22 2920 616e 6420 6e6f 7420  th(".") and not 
-000175e0: 7573 6572 496e 7075 744c 6f77 6572 2069  userInputLower i
-000175f0: 6e20 2863 6f6e 6669 672e 6578 6974 5f65  n (config.exit_e
-00017600: 6e74 7279 2c20 636f 6e66 6967 2e63 616e  ntry, config.can
-00017610: 6365 6c5f 656e 7472 792c 2022 2e6e 6577  cel_entry, ".new
-00017620: 222c 2022 2e63 6f6e 7465 7874 2229 3a0a  ", ".context"):.
-00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017640: 7573 6572 496e 7075 7420 3d20 7573 6572  userInput = user
-00017650: 496e 7075 744c 6f77 6572 203d 2073 656c  InputLower = sel
-00017660: 662e 7275 6e41 6374 696f 6e73 2822 2e2e  f.runActions("..
-00017670: 2e22 2c20 7573 6572 496e 7075 7429 0a0a  .", userInput)..
-00017680: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00017690: 6574 546f 6f6c 4465 7065 6e64 656e 6365  etToolDependence
-000176a0: 2875 7365 7249 6e70 7574 293a 0a20 2020  (userInput):.   
-000176b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000176c0: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
-000176d0: 2020 2023 2072 6570 6c61 6365 2061 6c69     # replace ali
-000176e0: 6173 2c20 6966 2061 6e79 2c20 7769 7468  as, if any, with
-000176f0: 2066 756c 6c20 656e 7472 790a 2020 2020   full entry.    
-00017700: 2020 2020 2020 2020 666f 7220 616c 6961          for alia
-00017710: 732c 2066 756c 6c45 6e74 7279 2069 6e20  s, fullEntry in 
-00017720: 636f 6e66 6967 2e61 6c69 6173 6573 2e69  config.aliases.i
-00017730: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
-00017740: 2020 2020 2020 2020 2375 7365 7249 6e70          #userInp
-00017750: 7574 203d 2072 652e 7375 6228 616c 6961  ut = re.sub(alia
-00017760: 732c 2066 756c 6c45 6e74 7279 2c20 7573  s, fullEntry, us
-00017770: 6572 496e 7075 7429 2023 2065 7272 6f72  erInput) # error
-00017780: 206f 6e20 5769 6e64 6f77 7320 636f 7a20   on Windows coz 
-00017790: 6f66 2057 696e 646f 7773 2070 6174 680a  of Windows path.
-000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177b0: 7573 6572 496e 7075 7420 3d20 7573 6572  userInput = user
-000177c0: 496e 7075 742e 7265 706c 6163 6528 616c  Input.replace(al
-000177d0: 6961 732c 2066 756c 6c45 6e74 7279 290a  ias, fullEntry).
-000177e0: 0a20 2020 2020 2020 2020 2020 2023 206f  .            # o
-000177f0: 7065 6e20 6669 6c65 202f 2064 6972 6563  pen file / direc
-00017800: 746f 7279 2064 6972 6563 746c 790a 2020  tory directly.  
-00017810: 2020 2020 2020 2020 2020 646f 6373 5f70            docs_p
-00017820: 6174 6820 3d20 6973 4578 6973 7469 6e67  ath = isExisting
-00017830: 5061 7468 2875 7365 7249 6e70 7574 290a  Path(userInput).
-00017840: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00017850: 732e 7061 7468 2e69 7366 696c 6528 646f  s.path.isfile(do
-00017860: 6373 5f70 6174 6829 3a0a 2020 2020 2020  cs_path):.      
-00017870: 2020 2020 2020 2020 2020 6f73 2e73 7973            os.sys
-00017880: 7465 6d28 6622 7b63 6f6e 6669 672e 6f70  tem(f"{config.op
-00017890: 656e 7d20 7b64 6f63 735f 7061 7468 7d22  en} {docs_path}"
-000178a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000178b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-000178c0: 2020 2020 2020 2065 6c69 6620 6f73 2e70         elif os.p
-000178d0: 6174 682e 6973 6469 7228 646f 6373 5f70  ath.isdir(docs_p
-000178e0: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
-000178f0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00017900: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00017910: 732e 6368 6469 7228 646f 6373 5f70 6174  s.chdir(docs_pat
-00017920: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
-00017930: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
-00017940: 4469 7265 6374 6f72 7920 6368 616e 6765  Directory change
-00017950: 6420 746f 3a20 7b64 6f63 735f 7061 7468  d to: {docs_path
-00017960: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00017970: 2020 2020 2020 2020 7365 6c66 2e67 6574          self.get
-00017980: 5061 7468 2e64 6973 706c 6179 4469 7265  Path.displayDire
-00017990: 6374 6f72 7943 6f6e 7465 6e74 2829 0a20  ctoryContent(). 
-000179a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000179b0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-000179c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000179d0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-000179e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000179f0: 2020 2020 2020 2020 2020 2320 7472 7920            # try 
-00017a00: 6576 616c 0a20 2020 2020 2020 2020 2020  eval.           
-00017a10: 2069 6620 636f 6e66 6967 2e64 6576 656c   if config.devel
-00017a20: 6f70 6572 2061 6e64 206e 6f74 2075 7365  oper and not use
-00017a30: 7249 6e70 7574 203d 3d20 222e 2e2e 223a  rInput == "...":
-00017a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017a50: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00017a60: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-00017a70: 3d20 6576 616c 2875 7365 7249 6e70 7574  = eval(userInput
-00017a80: 2920 2320 6974 2073 6f6c 7665 2073 696d  ) # it solve sim
-00017a90: 706c 6520 6d61 7468 2c20 652e 672e 2031  ple math, e.g. 1
-00017aa0: 2b31 2c20 6f72 2072 6561 6420 7661 7269  +1, or read vari
-00017ab0: 6162 6c65 732c 2065 2e67 2e20 6469 7228  ables, e.g. dir(
-00017ac0: 636f 6e66 6967 290a 2020 2020 2020 2020  config).        
-00017ad0: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00017ae0: 616c 7565 2069 7320 6e6f 7420 4e6f 6e65  alue is not None
-00017af0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017b00: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
-00017b10: 2876 616c 7565 290a 2020 2020 2020 2020  (value).        
-00017b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b30: 7070 7269 6e74 2e70 7072 696e 7428 7661  pprint.pprint(va
-00017b40: 6c75 6529 0a20 2020 2020 2020 2020 2020  lue).           
-00017b50: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00017b60: 6e74 2822 2229 0a20 2020 2020 2020 2020  nt("").         
-00017b70: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00017b80: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-00017b90: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00017ba0: 2072 652e 7365 6172 6368 2822 5e70 7269   re.search("^pri
-00017bb0: 6e74 5c28 5b5e 5c29 5c29 5d2b 3f5c 2924  nt\([^\)\)]+?\)$
-00017bc0: 222c 2075 7365 7249 6e70 7574 293a 0a20  ", userInput):. 
-00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017be0: 2020 2020 2020 2070 7269 6e74 2822 2229         print("")
-00017bf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017c00: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00017c10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00017c20: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00017c30: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00017c40: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
-00017c50: 2074 7279 2074 6f20 7275 6e20 6173 2061   try to run as a
-00017c60: 2070 7974 686f 6e20 7363 7269 7074 2066   python script f
-00017c70: 6972 7374 0a20 2020 2020 2020 2020 2020  irst.           
-00017c80: 2069 6620 636f 6e66 6967 2e64 6576 656c   if config.devel
-00017c90: 6f70 6572 3a0a 2020 2020 2020 2020 2020  oper:.          
-00017ca0: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-00017cb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00017cc0: 7865 6328 7573 6572 496e 7075 742c 2067  xec(userInput, g
-00017cd0: 6c6f 6261 6c73 2829 290a 2020 2020 2020  lobals()).      
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00017cf0: 696e 7428 2222 290a 2020 2020 2020 2020  int("").        
-00017d00: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00017d10: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
-00017d20: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d40: 2070 6173 730a 0a20 2020 2020 2020 2020   pass..         
-00017d50: 2020 2069 6620 7573 6572 496e 7075 742e     if userInput.
-00017d60: 7374 6172 7473 7769 7468 2822 2122 293a  startswith("!"):
-00017d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017d80: 2073 656c 662e 7275 6e53 7973 7465 6d43   self.runSystemC
-00017d90: 6f6d 6d61 6e64 2875 7365 7249 6e70 7574  ommand(userInput
-00017da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00017db0: 2020 7072 696e 7428 2222 290a 2020 2020    print("").    
-00017dc0: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-00017dd0: 6669 672e 6465 7665 6c6f 7065 7220 616e  fig.developer an
-00017de0: 6420 7573 6572 496e 7075 742e 7374 6172  d userInput.star
-00017df0: 7473 7769 7468 2822 6060 6022 2920 616e  tswith("```") an
-00017e00: 6420 7573 6572 496e 7075 742e 656e 6473  d userInput.ends
-00017e10: 7769 7468 2822 6060 6022 2920 616e 6420  with("```") and 
-00017e20: 6e6f 7420 7573 6572 496e 7075 7420 3d3d  not userInput ==
-00017e30: 2022 6060 6060 6060 223a 0a20 2020 2020   "``````":.     
-00017e40: 2020 2020 2020 2020 2020 2075 7365 7249             userI
-00017e50: 6e70 7574 203d 2072 652e 7375 6228 2260  nput = re.sub("`
-00017e60: 6060 7079 7468 6f6e 222c 2022 6060 6022  ``python", "```"
-00017e70: 2c20 7573 6572 496e 7075 7429 0a20 2020  , userInput).   
-00017e80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017e90: 662e 7275 6e50 7974 686f 6e53 6372 6970  f.runPythonScrip
-00017ea0: 7428 7573 6572 496e 7075 7429 0a20 2020  t(userInput).   
-00017eb0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00017ec0: 6e74 2822 2229 0a20 2020 2020 2020 2020  nt("").         
-00017ed0: 2020 2065 6c69 6620 7573 6572 496e 7075     elif userInpu
-00017ee0: 744c 6f77 6572 203d 3d20 636f 6e66 6967  tLower == config
-00017ef0: 2e65 7869 745f 656e 7472 793a 0a20 2020  .exit_entry:.   
-00017f00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00017f10: 662e 7361 7665 4368 6174 2863 6f6e 6669  f.saveChat(confi
-00017f20: 672e 6375 7272 656e 744d 6573 7361 6765  g.currentMessage
-00017f30: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00017f40: 2020 2072 6574 7572 6e20 7365 6c66 2e65     return self.e
-00017f50: 7869 7441 6374 696f 6e28 290a 2020 2020  xitAction().    
-00017f60: 2020 2020 2020 2020 656c 6966 2075 7365          elif use
-00017f70: 7249 6e70 7574 4c6f 7765 7220 3d3d 2063  rInputLower == c
-00017f80: 6f6e 6669 672e 6361 6e63 656c 5f65 6e74  onfig.cancel_ent
-00017f90: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00017fa0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
-00017fb0: 2020 2020 2065 6c69 6620 7573 6572 496e       elif userIn
-00017fc0: 7075 744c 6f77 6572 203d 3d20 222e 636f  putLower == ".co
-00017fd0: 6e74 6578 7422 3a0a 2020 2020 2020 2020  ntext":.        
-00017fe0: 2020 2020 2020 2020 7365 6c66 2e63 6861          self.cha
-00017ff0: 6e67 6543 6f6e 7465 7874 2829 0a20 2020  ngeContext().   
-00018000: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018010: 6e6f 7420 636f 6e66 6967 2e61 7070 6c79  not config.apply
-00018020: 5072 6564 6566 696e 6564 436f 6e74 6578  PredefinedContex
-00018030: 7441 6c77 6179 733a 0a20 2020 2020 2020  tAlways:.       
-00018040: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00018050: 636f 6e66 6967 2e63 6f6e 7665 7273 6174  config.conversat
-00018060: 696f 6e53 7461 7274 6564 3a0a 2020 2020  ionStarted:.    
-00018070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018080: 2020 2020 7365 6c66 2e73 6176 6543 6861      self.saveCha
-00018090: 7428 636f 6e66 6967 2e63 7572 7265 6e74  t(config.current
-000180a0: 4d65 7373 6167 6573 290a 2020 2020 2020  Messages).      
-000180b0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-000180c0: 6f72 6167 6564 6972 6563 746f 7279 2c20  oragedirectory, 
-000180d0: 636f 6e66 6967 2e63 7572 7265 6e74 4d65  config.currentMe
-000180e0: 7373 6167 6573 203d 2073 7461 7274 4368  ssages = startCh
-000180f0: 6174 2829 0a20 2020 2020 2020 2020 2020  at().           
-00018100: 2065 6c69 6620 7573 6572 496e 7075 744c   elif userInputL
-00018110: 6f77 6572 203d 3d20 222e 6e65 7722 3a0a  ower == ".new":.
-00018120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018130: 7365 6c66 2e73 6176 6543 6861 7428 636f  self.saveChat(co
-00018140: 6e66 6967 2e63 7572 7265 6e74 4d65 7373  nfig.currentMess
-00018150: 6167 6573 290a 2020 2020 2020 2020 2020  ages).          
-00018160: 2020 2020 2020 7374 6f72 6167 6564 6972        storagedir
-00018170: 6563 746f 7279 2c20 636f 6e66 6967 2e63  ectory, config.c
-00018180: 7572 7265 6e74 4d65 7373 6167 6573 203d  urrentMessages =
-00018190: 2073 7461 7274 4368 6174 2829 0a20 2020   startChat().   
-000181a0: 2020 2020 2020 2020 2065 6c69 6620 7573           elif us
-000181b0: 6572 496e 7075 7420 616e 6420 6e6f 7420  erInput and not 
-000181c0: 7573 6572 496e 7075 744c 6f77 6572 2069  userInputLower i
-000181d0: 6e20 6665 6174 7572 6573 4c6f 7765 723a  n featuresLower:
-000181e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000181f0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00018200: 2020 2020 2020 2020 2020 6966 2075 7365            if use
-00018210: 7249 6e70 7574 2061 6e64 2063 6f6e 6669  rInput and confi
-00018220: 672e 7474 7349 6e70 7574 3a0a 2020 2020  g.ttsInput:.    
-00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018240: 2020 2020 5454 5355 7469 6c2e 706c 6179      TTSUtil.play
-00018250: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
-00018260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018270: 2320 4665 6174 7572 653a 2069 6d70 726f  # Feature: impro
-00018280: 7665 2077 7269 7469 6e67 3a0a 2020 2020  ve writing:.    
-00018290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000182a0: 7370 6563 6961 6c45 6e74 7279 5061 7474  specialEntryPatt
-000182b0: 6572 6e20 3d20 225c 5b54 4f4f 4c5f 5b5e  ern = "\[TOOL_[^
-000182c0: 5c5b 5c5d 5d2a 3f5c 5d7c 5c5b 4e4f 5f54  \[\]]*?\]|\[NO_T
-000182d0: 4f4f 4c5c 5d7c 5c5b 4e4f 5f53 4352 4545  OOL\]|\[NO_SCREE
-000182e0: 4e49 4e47 5c5d 220a 2020 2020 2020 2020  NING\]".        
-000182f0: 2020 2020 2020 2020 2020 2020 7370 6563              spec
-00018300: 6961 6c45 6e74 7279 203d 2072 652e 7365  ialEntry = re.se
-00018310: 6172 6368 2873 7065 6369 616c 456e 7472  arch(specialEntr
-00018320: 7950 6174 7465 726e 2c20 7573 6572 496e  yPattern, userIn
-00018330: 7075 7429 0a20 2020 2020 2020 2020 2020  put).           
-00018340: 2020 2020 2020 2020 2073 7065 6369 616c           special
-00018350: 456e 7472 7920 3d20 7370 6563 6961 6c45  Entry = specialE
-00018360: 6e74 7279 2e67 726f 7570 2830 2920 6966  ntry.group(0) if
-00018370: 2073 7065 6369 616c 456e 7472 7920 656c   specialEntry el
-00018380: 7365 2022 220a 2020 2020 2020 2020 2020  se "".          
-00018390: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-000183a0: 7075 7420 3d20 7265 2e73 7562 2873 7065  put = re.sub(spe
-000183b0: 6369 616c 456e 7472 7950 6174 7465 726e  cialEntryPattern
-000183c0: 2c20 2222 2c20 7573 6572 496e 7075 7429  , "", userInput)
-000183d0: 2023 2072 656d 6f76 6520 7370 6563 6961   # remove specia
-000183e0: 6c20 656e 7472 7920 7465 6d70 6f72 6172  l entry temporar
-000183f0: 696c 790a 2020 2020 2020 2020 2020 2020  ily.            
-00018400: 2020 2020 2020 2020 6966 2075 7365 7249          if userI
-00018410: 6e70 7574 2061 6e64 2063 6f6e 6669 672e  nput and config.
-00018420: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
-00018430: 7269 7469 6e67 3a0a 2020 2020 2020 2020  riting:.        
-00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018450: 7573 6572 496e 7075 7420 3d20 7265 2e73  userInput = re.s
-00018460: 7562 2822 5c6e 5c5b 4375 7272 656e 7420  ub("\n\[Current 
-00018470: 7469 6d65 3a20 5b5e 5c6e 5d2a 3f24 222c  time: [^\n]*?$",
-00018480: 2022 222c 2075 7365 7249 6e70 7574 290a   "", userInput).
-00018490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184a0: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
-000184b0: 672e 6973 5465 726d 7578 3a0a 2020 2020  g.isTermux:.    
-000184c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184d0: 2020 2020 2020 2020 6461 795f 6f66 5f77          day_of_w
-000184e0: 6565 6b20 3d20 2222 0a20 2020 2020 2020  eek = "".       
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00018510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018520: 2020 2064 6179 5f6f 665f 7765 656b 203d     day_of_week =
-00018530: 2066 2274 6f64 6179 2069 7320 7b67 6574   f"today is {get
-00018540: 4461 794f 6657 6565 6b28 297d 2061 6e64  DayOfWeek()} and
-00018550: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-00018560: 2020 2020 2020 2020 2020 2069 6d70 726f             impro
-00018570: 7665 6456 6572 7369 6f6e 203d 2043 616c  vedVersion = Cal
-00018580: 6c4c 4c4d 2e67 6574 5369 6e67 6c65 4368  lLLM.getSingleCh
-00018590: 6174 5265 7370 6f6e 7365 2866 2222 2249  atResponse(f"""I
-000185a0: 6d70 726f 7665 2074 6865 2066 6f6c 6c6f  mprove the follo
-000185b0: 7769 6e67 2077 7269 7469 6e67 2c20 6163  wing writing, ac
-000185c0: 636f 7264 696e 6720 746f 207b 636f 6e66  cording to {conf
-000185d0: 6967 2e69 6d70 726f 7665 6457 7269 7469  ig.improvedWriti
-000185e0: 6e67 5379 746c 657d 0a49 6e20 6164 6469  ngSytle}.In addi
-000185f0: 7469 6f6e 2c20 4920 776f 756c 6420 6c69  tion, I would li
-00018600: 6b65 2079 6f75 2074 6f20 6865 6c70 206d  ke you to help m
-00018610: 6520 7769 7468 2063 6f6e 7665 7274 696e  e with convertin
-00018620: 6720 7265 6c61 7469 7665 2064 6174 6573  g relative dates
-00018630: 2061 6e64 2074 696d 6573 2c20 6966 2061   and times, if a
-00018640: 6e79 2c20 696e 746f 2065 7861 6374 2064  ny, into exact d
-00018650: 6174 6573 2061 6e64 2074 696d 6573 2062  ates and times b
-00018660: 6173 6564 206f 6e20 7468 6520 7265 6665  ased on the refe
-00018670: 7265 6e63 6520 7468 6174 207b 6461 795f  rence that {day_
-00018680: 6f66 5f77 6565 6b7d 6375 7272 656e 7420  of_week}current 
-00018690: 6461 7465 7469 6d65 2069 7320 7b73 7472  datetime is {str
-000186a0: 2864 6174 6574 696d 652e 6461 7465 7469  (datetime.dateti
-000186b0: 6d65 2e6e 6f77 2829 297d 2e0a 5265 6d65  me.now())}..Reme
-000186c0: 6d62 6572 2c20 7072 6f76 6964 6520 6d65  mber, provide me
-000186d0: 2077 6974 6820 7468 6520 696d 7072 6f76   with the improv
-000186e0: 6564 2077 7269 7469 6e67 206f 6e6c 792c  ed writing only,
-000186f0: 2065 6e63 6c6f 7365 6420 696e 2074 7269   enclosed in tri
-00018700: 706c 6520 7175 6f74 6573 2060 6060 2061  ple quotes ``` a
-00018710: 6e64 2077 6974 686f 7574 2061 6e79 2061  nd without any a
-00018720: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00018730: 6174 696f 6e20 6f72 2063 6f6d 6d65 6e74  ation or comment
-00018740: 732e 0a4d 7920 7772 6974 696e 673a 0a7b  s..My writing:.{
-00018750: 7573 6572 496e 7075 747d 2222 2229 0a20  userInput}"""). 
-00018760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018770: 2020 2020 2020 2069 6620 696d 7072 6f76         if improv
-00018780: 6564 5665 7273 696f 6e20 616e 6420 696d  edVersion and im
-00018790: 7072 6f76 6564 5665 7273 696f 6e2e 7374  provedVersion.st
-000187a0: 6172 7473 7769 7468 2822 6060 6022 2920  artswith("```") 
-000187b0: 616e 6420 696d 7072 6f76 6564 5665 7273  and improvedVers
-000187c0: 696f 6e2e 656e 6473 7769 7468 2822 6060  ion.endswith("``
-000187d0: 6022 293a 0a20 2020 2020 2020 2020 2020  `"):.           
-000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000187f0: 2070 7269 6e74 3128 696d 7072 6f76 6564   print1(improved
-00018800: 5665 7273 696f 6e29 0a20 2020 2020 2020  Version).       
-00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018820: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
-00018830: 2069 6d70 726f 7665 6456 6572 7369 6f6e   improvedVersion
-00018840: 5b33 3a2d 335d 0a20 2020 2020 2020 2020  [3:-3].         
-00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018860: 2020 2069 6620 636f 6e66 6967 2e74 7473     if config.tts
-00018870: 4f75 7470 7574 3a0a 2020 2020 2020 2020  Output:.        
-00018880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018890: 2020 2020 2020 2020 5454 5355 7469 6c2e          TTSUtil.
-000188a0: 706c 6179 2875 7365 7249 6e70 7574 290a  play(userInput).
-000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188c0: 2020 2020 6966 2073 7065 6369 616c 456e      if specialEn
-000188d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000188e0: 2020 2020 2020 2020 2020 2020 2075 7365               use
-000188f0: 7249 6e70 7574 203d 2066 227b 7573 6572  rInput = f"{user
-00018900: 496e 7075 747d 7b73 7065 6369 616c 456e  Input}{specialEn
-00018910: 7472 797d 220a 2020 2020 2020 2020 2020  try}".          
-00018920: 2020 2020 2020 2020 2020 2320 7265 6669            # refi
-00018930: 6e65 206d 6573 7361 6765 7320 6265 666f  ne messages befo
-00018940: 7265 2072 756e 6e69 6e67 2063 6f6d 706c  re running compl
-00018950: 6574 696f 6e0a 2020 2020 2020 2020 2020  etion.          
-00018960: 2020 2020 2020 2020 2020 6669 6e65 5475            fineTu
-00018970: 6e65 6455 7365 7249 6e70 7574 203d 2073  nedUserInput = s
-00018980: 656c 662e 6669 6e65 5475 6e65 5573 6572  elf.fineTuneUser
-00018990: 496e 7075 7428 7573 6572 496e 7075 7429  Input(userInput)
-000189a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000189b0: 2020 2020 2023 2069 6e20 6361 7365 206f       # in case o
-000189c0: 6620 7472 616e 736c 6174 696f 6e0a 2020  f translation.  
-000189d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000189e0: 2020 6966 2063 6f6e 6669 672e 7072 6564    if config.pred
-000189f0: 6566 696e 6564 436f 6e74 6578 7420 3d3d  efinedContext ==
-00018a00: 2022 4c65 7420 6d65 2054 7261 6e73 6c61   "Let me Transla
-00018a10: 7465 2220 616e 6420 6669 6e65 5475 6e65  te" and fineTune
-00018a20: 6455 7365 7249 6e70 7574 2e73 7461 7274  dUserInput.start
-00018a30: 7377 6974 6828 2241 7373 6973 7420 6d65  swith("Assist me
-00018a40: 2062 7920 6163 7469 6e67 2061 7320 6120   by acting as a 
-00018a50: 7472 616e 736c 6174 6f72 2e5c 6e50 6c65  translator.\nPle
-00018a60: 6173 6520 7472 616e 736c 6174 6522 293a  ase translate"):
-00018a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018a80: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
-00018a90: 2250 6c65 6173 6520 7370 6563 6966 7920  "Please specify 
-00018aa0: 6265 6c6f 7720 7468 6520 6c61 6e67 7561  below the langua
-00018ab0: 6765 2079 6f75 2077 6f75 6c64 206c 696b  ge you would lik
-00018ac0: 6520 7468 6520 636f 6e74 656e 7420 746f  e the content to
-00018ad0: 2062 6520 7472 616e 736c 6174 6564 2069   be translated i
-00018ae0: 6e74 6f3a 2229 0a20 2020 2020 2020 2020  nto:").         
-00018af0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00018b00: 616e 6775 6167 6520 3d20 7365 6c66 2e70  anguage = self.p
-00018b10: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
-00018b20: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
-00018b30: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
-00018b40: 6c65 322c 2064 6566 6175 6c74 3d63 6f6e  le2, default=con
-00018b50: 6669 672e 7472 616e 736c 6174 6554 6f4c  fig.translateToL
-00018b60: 616e 6775 6167 6529 0a20 2020 2020 2020  anguage).       
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b80: 2069 6620 6c61 6e67 7561 6765 2061 6e64   if language and
-00018b90: 206e 6f74 206c 616e 6775 6167 652e 7374   not language.st
-00018ba0: 7269 7028 292e 6c6f 7765 7228 2920 696e  rip().lower() in
-00018bb0: 2028 636f 6e66 6967 2e63 616e 6365 6c5f   (config.cancel_
-00018bc0: 656e 7472 792c 2063 6f6e 6669 672e 6578  entry, config.ex
-00018bd0: 6974 5f65 6e74 7279 293a 0a20 2020 2020  it_entry):.     
-00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bf0: 2020 2020 2020 2066 696e 6554 756e 6564         fineTuned
-00018c00: 5573 6572 496e 7075 7420 3d20 6622 7b66  UserInput = f"{f
-00018c10: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-00018c20: 747d 5c6e 5c6e 506c 6561 7365 2074 7261  t}\n\nPlease tra
-00018c30: 6e73 6c61 7465 2074 6865 2063 6f6e 7465  nslate the conte
-00018c40: 6e74 2069 6e74 6f20 3c6c 616e 6775 6167  nt into <languag
-00018c50: 653e 7b6c 616e 6775 6167 657d 3c2f 6c61  e>{language}</la
-00018c60: 6e67 7561 6765 3e2e 220a 2020 2020 2020  nguage>.".      
-00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c80: 2020 2020 2020 636f 6e66 6967 2e74 7261        config.tra
-00018c90: 6e73 6c61 7465 546f 4c61 6e67 7561 6765  nslateToLanguage
-00018ca0: 203d 206c 616e 6775 6167 650a 2020 2020   = language.    
-00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cc0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00017280: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00017290: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+000172a0: 7420 3d20 7072 6566 6978 0a20 2020 2020  t = prefix.     
+000172b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000172c0: 7265 6669 7820 3d20 2222 0a20 2020 2020  refix = "".     
+000172d0: 2020 2020 2020 2020 2020 2073 7566 6669             suffi
+000172e0: 7820 3d20 7573 6572 496e 7075 745b 636f  x = userInput[co
+000172f0: 6e66 6967 2e61 6464 5061 7468 4174 3a5d  nfig.addPathAt:]
+00017300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017310: 2063 6f6e 6669 672e 6164 6450 6174 6841   config.addPathA
+00017320: 7420 3d20 4e6f 6e65 0a20 2020 2020 2020  t = None.       
+00017330: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00017340: 6465 6661 756c 743a 0a20 2020 2020 2020  default:.       
+00017350: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00017360: 6175 6c74 203d 206f 732e 6765 7463 7764  ault = os.getcwd
+00017370: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00017380: 2020 2075 7365 7250 6174 6820 3d20 7365     userPath = se
+00017390: 6c66 2e67 6574 5061 7468 2e67 6574 5061  lf.getPath.getPa
+000173a0: 7468 286d 6573 7361 6765 3d66 227b 7072  th(message=f"{pr
+000173b0: 6566 6978 7d3c 7b63 6f6e 6669 672e 7465  efix}<{config.te
+000173c0: 726d 696e 616c 436f 6d6d 616e 6445 6e74  rminalCommandEnt
+000173d0: 7279 436f 6c6f 7232 7d3e 5b61 6464 2061  ryColor2}>[add a
+000173e0: 2070 6174 6820 6865 7265 5d3c 2f7b 636f   path here]</{co
+000173f0: 6e66 6967 2e74 6572 6d69 6e61 6c43 6f6d  nfig.terminalCom
+00017400: 6d61 6e64 456e 7472 7943 6f6c 6f72 327d  mandEntryColor2}
+00017410: 3e7b 7375 6666 6978 7d22 2c20 7072 6f6d  >{suffix}", prom
+00017420: 7074 496e 6469 6361 746f 723d 223e 3e3e  ptIndicator=">>>
+00017430: 2022 2c20 656d 7074 795f 746f 5f63 616e   ", empty_to_can
+00017440: 6365 6c3d 5472 7565 2c20 6465 6661 756c  cel=True, defaul
+00017450: 743d 6465 6661 756c 7429 0a20 2020 2020  t=default).     
+00017460: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00017470: 672e 6465 6661 756c 7445 6e74 7279 203d  g.defaultEntry =
+00017480: 2066 227b 7072 6566 6978 7d7b 7573 6572   f"{prefix}{user
+00017490: 5061 7468 7d7b 7375 6666 6978 7d22 0a20  Path}{suffix}". 
+000174a0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+000174b0: 7365 7249 6e70 7574 203d 2022 220a 2020  serInput = "".  
+000174c0: 2020 2020 2020 2020 2020 656c 6966 206e            elif n
+000174d0: 6f74 2075 7365 7249 6e70 7574 4c6f 7765  ot userInputLowe
+000174e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+000174f0: 2020 2075 7365 7249 6e70 7574 203d 2063     userInput = c
+00017500: 6f6e 6669 672e 626c 616e 6b45 6e74 7279  onfig.blankEntry
+00017510: 4163 7469 6f6e 0a20 2020 2020 2020 2020  Action.         
+00017520: 2020 2069 6620 7573 6572 496e 7075 7420     if userInput 
+00017530: 3d3d 2022 2e2e 2e22 3a0a 2020 2020 2020  == "...":.      
+00017540: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
+00017550: 7075 7420 3d20 7573 6572 496e 7075 744c  put = userInputL
+00017560: 6f77 6572 203d 2073 656c 662e 7275 6e41  ower = self.runA
+00017570: 6374 696f 6e73 2875 7365 7249 6e70 7574  ctions(userInput
+00017580: 290a 2020 2020 2020 2020 2020 2020 2365  ).            #e
+00017590: 6c69 6620 7573 6572 496e 7075 744c 6f77  lif userInputLow
+000175a0: 6572 2069 6e20 7475 706c 6528 7365 6c66  er in tuple(self
+000175b0: 2e61 6374 696f 6e73 2e6b 6579 7328 2929  .actions.keys())
+000175c0: 3a0a 2020 2020 2020 2020 2020 2020 656c  :.            el
+000175d0: 6966 2075 7365 7249 6e70 7574 4c6f 7765  if userInputLowe
+000175e0: 722e 7374 6172 7473 7769 7468 2822 2e22  r.startswith("."
+000175f0: 2920 616e 6420 6e6f 7420 7573 6572 496e  ) and not userIn
+00017600: 7075 744c 6f77 6572 2069 6e20 2863 6f6e  putLower in (con
+00017610: 6669 672e 6578 6974 5f65 6e74 7279 2c20  fig.exit_entry, 
+00017620: 636f 6e66 6967 2e63 616e 6365 6c5f 656e  config.cancel_en
+00017630: 7472 792c 2022 2e6e 6577 222c 2022 2e63  try, ".new", ".c
+00017640: 6f6e 7465 7874 2229 3a0a 2020 2020 2020  ontext"):.      
+00017650: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
+00017660: 7075 7420 3d20 7573 6572 496e 7075 744c  put = userInputL
+00017670: 6f77 6572 203d 2073 656c 662e 7275 6e41  ower = self.runA
+00017680: 6374 696f 6e73 2822 2e2e 2e22 2c20 7573  ctions("...", us
+00017690: 6572 496e 7075 7429 0a0a 2020 2020 2020  erInput)..      
+000176a0: 2020 2020 2020 6966 2073 6574 546f 6f6c        if setTool
+000176b0: 4465 7065 6e64 656e 6365 2875 7365 7249  Dependence(userI
+000176c0: 6e70 7574 293a 0a20 2020 2020 2020 2020  nput):.         
+000176d0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+000176e0: 0a20 2020 2020 2020 2020 2020 2023 2072  .            # r
+000176f0: 6570 6c61 6365 2061 6c69 6173 2c20 6966  eplace alias, if
+00017700: 2061 6e79 2c20 7769 7468 2066 756c 6c20   any, with full 
+00017710: 656e 7472 790a 2020 2020 2020 2020 2020  entry.          
+00017720: 2020 666f 7220 616c 6961 732c 2066 756c    for alias, ful
+00017730: 6c45 6e74 7279 2069 6e20 636f 6e66 6967  lEntry in config
+00017740: 2e61 6c69 6173 6573 2e69 7465 6d73 2829  .aliases.items()
+00017750: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017760: 2020 2375 7365 7249 6e70 7574 203d 2072    #userInput = r
+00017770: 652e 7375 6228 616c 6961 732c 2066 756c  e.sub(alias, ful
+00017780: 6c45 6e74 7279 2c20 7573 6572 496e 7075  lEntry, userInpu
+00017790: 7429 2023 2065 7272 6f72 206f 6e20 5769  t) # error on Wi
+000177a0: 6e64 6f77 7320 636f 7a20 6f66 2057 696e  ndows coz of Win
+000177b0: 646f 7773 2070 6174 680a 2020 2020 2020  dows path.      
+000177c0: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
+000177d0: 7075 7420 3d20 7573 6572 496e 7075 742e  put = userInput.
+000177e0: 7265 706c 6163 6528 616c 6961 732c 2066  replace(alias, f
+000177f0: 756c 6c45 6e74 7279 290a 0a20 2020 2020  ullEntry)..     
+00017800: 2020 2020 2020 2023 206f 7065 6e20 6669         # open fi
+00017810: 6c65 202f 2064 6972 6563 746f 7279 2064  le / directory d
+00017820: 6972 6563 746c 790a 2020 2020 2020 2020  irectly.        
+00017830: 2020 2020 646f 6373 5f70 6174 6820 3d20      docs_path = 
+00017840: 6973 4578 6973 7469 6e67 5061 7468 2875  isExistingPath(u
+00017850: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
+00017860: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+00017870: 2e69 7366 696c 6528 646f 6373 5f70 6174  .isfile(docs_pat
+00017880: 6829 3a0a 2020 2020 2020 2020 2020 2020  h):.            
+00017890: 2020 2020 6f73 2e73 7973 7465 6d28 6622      os.system(f"
+000178a0: 7b63 6f6e 6669 672e 6f70 656e 7d20 7b64  {config.open} {d
+000178b0: 6f63 735f 7061 7468 7d22 290a 2020 2020  ocs_path}").    
+000178c0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+000178d0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+000178e0: 2065 6c69 6620 6f73 2e70 6174 682e 6973   elif os.path.is
+000178f0: 6469 7228 646f 6373 5f70 6174 6829 3a0a  dir(docs_path):.
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00017920: 2020 2020 2020 2020 206f 732e 6368 6469           os.chdi
+00017930: 7228 646f 6373 5f70 6174 6829 0a20 2020  r(docs_path).   
+00017940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017950: 2070 7269 6e74 3328 6622 4469 7265 6374   print3(f"Direct
+00017960: 6f72 7920 6368 616e 6765 6420 746f 3a20  ory changed to: 
+00017970: 7b64 6f63 735f 7061 7468 7d22 290a 2020  {docs_path}").  
+00017980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017990: 2020 7365 6c66 2e67 6574 5061 7468 2e64    self.getPath.d
+000179a0: 6973 706c 6179 4469 7265 6374 6f72 7943  isplayDirectoryC
+000179b0: 6f6e 7465 6e74 2829 0a20 2020 2020 2020  ontent().       
+000179c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000179d0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+000179e0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a00: 2020 7061 7373 0a0a 2020 2020 2020 2020    pass..        
+00017a10: 2020 2020 2320 7472 7920 6576 616c 0a20      # try eval. 
+00017a20: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00017a30: 6e66 6967 2e64 6576 656c 6f70 6572 2061  nfig.developer a
+00017a40: 6e64 206e 6f74 2075 7365 7249 6e70 7574  nd not userInput
+00017a50: 203d 3d20 222e 2e2e 223a 0a20 2020 2020   == "...":.     
+00017a60: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00017a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a80: 2020 2020 7661 6c75 6520 3d20 6576 616c      value = eval
+00017a90: 2875 7365 7249 6e70 7574 2920 2320 6974  (userInput) # it
+00017aa0: 2073 6f6c 7665 2073 696d 706c 6520 6d61   solve simple ma
+00017ab0: 7468 2c20 652e 672e 2031 2b31 2c20 6f72  th, e.g. 1+1, or
+00017ac0: 2072 6561 6420 7661 7269 6162 6c65 732c   read variables,
+00017ad0: 2065 2e67 2e20 6469 7228 636f 6e66 6967   e.g. dir(config
+00017ae0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017af0: 2020 2020 2020 6966 2076 616c 7565 2069        if value i
+00017b00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00017b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b20: 2020 2020 2370 7269 6e74 2876 616c 7565      #print(value
+00017b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017b40: 2020 2020 2020 2020 2020 7070 7269 6e74            pprint
+00017b50: 2e70 7072 696e 7428 7661 6c75 6529 0a20  .pprint(value). 
+00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b70: 2020 2020 2020 2070 7269 6e74 2822 2229         print("")
+00017b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017b90: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00017ba0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00017bb0: 2020 2020 2020 656c 6966 2072 652e 7365        elif re.se
+00017bc0: 6172 6368 2822 5e70 7269 6e74 5c28 5b5e  arch("^print\([^
+00017bd0: 5c29 5c29 5d2b 3f5c 2924 222c 2075 7365  \)\)]+?\)$", use
+00017be0: 7249 6e70 7574 293a 0a20 2020 2020 2020  rInput):.       
+00017bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c00: 2070 7269 6e74 2822 2229 0a20 2020 2020   print("").     
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00017c30: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00017c40: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+00017c50: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
+00017c60: 2020 2020 2020 2020 2023 2074 7279 2074           # try t
+00017c70: 6f20 7275 6e20 6173 2061 2070 7974 686f  o run as a pytho
+00017c80: 6e20 7363 7269 7074 2066 6972 7374 0a20  n script first. 
+00017c90: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+00017ca0: 6e66 6967 2e64 6576 656c 6f70 6572 3a0a  nfig.developer:.
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cc0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00017cd0: 2020 2020 2020 2020 2065 7865 6328 7573           exec(us
+00017ce0: 6572 496e 7075 742c 2067 6c6f 6261 6c73  erInput, globals
+00017cf0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00017d00: 2020 2020 2020 2020 7072 696e 7428 2222          print(""
+00017d10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00017d20: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00017d30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017d40: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00017d50: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00017d60: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017d70: 7573 6572 496e 7075 742e 7374 6172 7473  userInput.starts
+00017d80: 7769 7468 2822 2122 293a 0a20 2020 2020  with("!"):.     
+00017d90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00017da0: 7275 6e53 7973 7465 6d43 6f6d 6d61 6e64  runSystemCommand
+00017db0: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
+00017dc0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00017dd0: 7428 2222 290a 2020 2020 2020 2020 2020  t("").          
+00017de0: 2020 656c 6966 2063 6f6e 6669 672e 6465    elif config.de
+00017df0: 7665 6c6f 7065 7220 616e 6420 7573 6572  veloper and user
+00017e00: 496e 7075 742e 7374 6172 7473 7769 7468  Input.startswith
+00017e10: 2822 6060 6022 2920 616e 6420 7573 6572  ("```") and user
+00017e20: 496e 7075 742e 656e 6473 7769 7468 2822  Input.endswith("
+00017e30: 6060 6022 2920 616e 6420 6e6f 7420 7573  ```") and not us
+00017e40: 6572 496e 7075 7420 3d3d 2022 6060 6060  erInput == "````
+00017e50: 6060 223a 0a20 2020 2020 2020 2020 2020  ``":.           
+00017e60: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
+00017e70: 2072 652e 7375 6228 2260 6060 7079 7468   re.sub("```pyth
+00017e80: 6f6e 222c 2022 6060 6022 2c20 7573 6572  on", "```", user
+00017e90: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
+00017ea0: 2020 2020 2020 2073 656c 662e 7275 6e50         self.runP
+00017eb0: 7974 686f 6e53 6372 6970 7428 7573 6572  ythonScript(user
+00017ec0: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
+00017ed0: 2020 2020 2020 2070 7269 6e74 2822 2229         print("")
+00017ee0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00017ef0: 6620 7573 6572 496e 7075 744c 6f77 6572  f userInputLower
+00017f00: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
+00017f10: 656e 7472 793a 0a20 2020 2020 2020 2020  entry:.         
+00017f20: 2020 2020 2020 2073 656c 662e 7361 7665         self.save
+00017f30: 4368 6174 2863 6f6e 6669 672e 6375 7272  Chat(config.curr
+00017f40: 656e 744d 6573 7361 6765 7329 0a20 2020  entMessages).   
+00017f50: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00017f60: 7572 6e20 7365 6c66 2e65 7869 7441 6374  urn self.exitAct
+00017f70: 696f 6e28 290a 2020 2020 2020 2020 2020  ion().          
+00017f80: 2020 656c 6966 2075 7365 7249 6e70 7574    elif userInput
+00017f90: 4c6f 7765 7220 3d3d 2063 6f6e 6669 672e  Lower == config.
+00017fa0: 6361 6e63 656c 5f65 6e74 7279 3a0a 2020  cancel_entry:.  
+00017fb0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00017fc0: 7373 0a20 2020 2020 2020 2020 2020 2065  ss.            e
+00017fd0: 6c69 6620 7573 6572 496e 7075 744c 6f77  lif userInputLow
+00017fe0: 6572 203d 3d20 222e 636f 6e74 6578 7422  er == ".context"
+00017ff0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018000: 2020 7365 6c66 2e63 6861 6e67 6543 6f6e    self.changeCon
+00018010: 7465 7874 2829 0a20 2020 2020 2020 2020  text().         
+00018020: 2020 2020 2020 2069 6620 6e6f 7420 636f         if not co
+00018030: 6e66 6967 2e61 7070 6c79 5072 6564 6566  nfig.applyPredef
+00018040: 696e 6564 436f 6e74 6578 7441 6c77 6179  inedContextAlway
+00018050: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00018060: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+00018070: 2e63 6f6e 7665 7273 6174 696f 6e53 7461  .conversationSta
+00018080: 7274 6564 3a0a 2020 2020 2020 2020 2020  rted:.          
+00018090: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000180a0: 6c66 2e73 6176 6543 6861 7428 636f 6e66  lf.saveChat(conf
+000180b0: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
+000180c0: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+000180d0: 2020 2020 2020 2020 7374 6f72 6167 6564          storaged
+000180e0: 6972 6563 746f 7279 2c20 636f 6e66 6967  irectory, config
+000180f0: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
+00018100: 203d 2073 7461 7274 4368 6174 2829 0a20   = startChat(). 
+00018110: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00018120: 7573 6572 496e 7075 744c 6f77 6572 203d  userInputLower =
+00018130: 3d20 222e 6e65 7722 3a0a 2020 2020 2020  = ".new":.      
+00018140: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+00018150: 6176 6543 6861 7428 636f 6e66 6967 2e63  aveChat(config.c
+00018160: 7572 7265 6e74 4d65 7373 6167 6573 290a  urrentMessages).
+00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018180: 7374 6f72 6167 6564 6972 6563 746f 7279  storagedirectory
+00018190: 2c20 636f 6e66 6967 2e63 7572 7265 6e74  , config.current
+000181a0: 4d65 7373 6167 6573 203d 2073 7461 7274  Messages = start
+000181b0: 4368 6174 2829 0a20 2020 2020 2020 2020  Chat().         
+000181c0: 2020 2065 6c69 6620 7573 6572 496e 7075     elif userInpu
+000181d0: 7420 616e 6420 6e6f 7420 7573 6572 496e  t and not userIn
+000181e0: 7075 744c 6f77 6572 2069 6e20 6665 6174  putLower in feat
+000181f0: 7572 6573 4c6f 7765 723a 0a20 2020 2020  uresLower:.     
+00018200: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018220: 2020 2020 6966 2075 7365 7249 6e70 7574      if userInput
+00018230: 2061 6e64 2063 6f6e 6669 672e 7474 7349   and config.ttsI
+00018240: 6e70 7574 3a0a 2020 2020 2020 2020 2020  nput:.          
+00018250: 2020 2020 2020 2020 2020 2020 2020 5454                TT
+00018260: 5355 7469 6c2e 706c 6179 2875 7365 7249  SUtil.play(userI
+00018270: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
+00018280: 2020 2020 2020 2020 2020 2320 4665 6174            # Feat
+00018290: 7572 653a 2069 6d70 726f 7665 2077 7269  ure: improve wri
+000182a0: 7469 6e67 3a0a 2020 2020 2020 2020 2020  ting:.          
+000182b0: 2020 2020 2020 2020 2020 7370 6563 6961            specia
+000182c0: 6c45 6e74 7279 5061 7474 6572 6e20 3d20  lEntryPattern = 
+000182d0: 225c 5b54 4f4f 4c5f 5b5e 5c5b 5c5d 5d2a  "\[TOOL_[^\[\]]*
+000182e0: 3f5c 5d7c 5c5b 4e4f 5f54 4f4f 4c5c 5d7c  ?\]|\[NO_TOOL\]|
+000182f0: 5c5b 4e4f 5f53 4352 4545 4e49 4e47 5c5d  \[NO_SCREENING\]
+00018300: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00018310: 2020 2020 2020 7370 6563 6961 6c45 6e74        specialEnt
+00018320: 7279 203d 2072 652e 7365 6172 6368 2873  ry = re.search(s
+00018330: 7065 6369 616c 456e 7472 7950 6174 7465  pecialEntryPatte
+00018340: 726e 2c20 7573 6572 496e 7075 7429 0a20  rn, userInput). 
+00018350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018360: 2020 2073 7065 6369 616c 456e 7472 7920     specialEntry 
+00018370: 3d20 7370 6563 6961 6c45 6e74 7279 2e67  = specialEntry.g
+00018380: 726f 7570 2830 2920 6966 2073 7065 6369  roup(0) if speci
+00018390: 616c 456e 7472 7920 656c 7365 2022 220a  alEntry else "".
+000183a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000183b0: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
+000183c0: 7265 2e73 7562 2873 7065 6369 616c 456e  re.sub(specialEn
+000183d0: 7472 7950 6174 7465 726e 2c20 2222 2c20  tryPattern, "", 
+000183e0: 7573 6572 496e 7075 7429 2023 2072 656d  userInput) # rem
+000183f0: 6f76 6520 7370 6563 6961 6c20 656e 7472  ove special entr
+00018400: 7920 7465 6d70 6f72 6172 696c 790a 2020  y temporarily.  
+00018410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018420: 2020 6966 2075 7365 7249 6e70 7574 2061    if userInput a
+00018430: 6e64 2063 6f6e 6669 672e 6469 7370 6c61  nd config.displa
+00018440: 7949 6d70 726f 7665 6457 7269 7469 6e67  yImprovedWriting
+00018450: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018460: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
+00018470: 7075 7420 3d20 7265 2e73 7562 2822 5c6e  put = re.sub("\n
+00018480: 5c5b 4375 7272 656e 7420 7469 6d65 3a20  \[Current time: 
+00018490: 5b5e 5c6e 5d2a 3f24 222c 2022 222c 2075  [^\n]*?$", "", u
+000184a0: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
+000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184c0: 2020 6966 2063 6f6e 6669 672e 6973 5465    if config.isTe
+000184d0: 726d 7578 3a0a 2020 2020 2020 2020 2020  rmux:.          
+000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000184f0: 2020 6461 795f 6f66 5f77 6565 6b20 3d20    day_of_week = 
+00018500: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00018510: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00018520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018530: 2020 2020 2020 2020 2020 2020 2064 6179               day
+00018540: 5f6f 665f 7765 656b 203d 2066 2274 6f64  _of_week = f"tod
+00018550: 6179 2069 7320 7b67 6574 4461 794f 6657  ay is {getDayOfW
+00018560: 6565 6b28 297d 2061 6e64 2022 0a20 2020  eek()} and ".   
+00018570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018580: 2020 2020 2069 6d70 726f 7665 6456 6572       improvedVer
+00018590: 7369 6f6e 203d 2043 616c 6c4c 4c4d 2e67  sion = CallLLM.g
+000185a0: 6574 5369 6e67 6c65 4368 6174 5265 7370  etSingleChatResp
+000185b0: 6f6e 7365 2866 2222 2249 6d70 726f 7665  onse(f"""Improve
+000185c0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2077   the following w
+000185d0: 7269 7469 6e67 2c20 6163 636f 7264 696e  riting, accordin
+000185e0: 6720 746f 207b 636f 6e66 6967 2e69 6d70  g to {config.imp
+000185f0: 726f 7665 6457 7269 7469 6e67 5379 746c  rovedWritingSytl
+00018600: 657d 0a49 6e20 6164 6469 7469 6f6e 2c20  e}.In addition, 
+00018610: 4920 776f 756c 6420 6c69 6b65 2079 6f75  I would like you
+00018620: 2074 6f20 6865 6c70 206d 6520 7769 7468   to help me with
+00018630: 2063 6f6e 7665 7274 696e 6720 7265 6c61   converting rela
+00018640: 7469 7665 2064 6174 6573 2061 6e64 2074  tive dates and t
+00018650: 696d 6573 2c20 6966 2061 6e79 2c20 696e  imes, if any, in
+00018660: 746f 2065 7861 6374 2064 6174 6573 2061  to exact dates a
+00018670: 6e64 2074 696d 6573 2062 6173 6564 206f  nd times based o
+00018680: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
+00018690: 7468 6174 207b 6461 795f 6f66 5f77 6565  that {day_of_wee
+000186a0: 6b7d 6375 7272 656e 7420 6461 7465 7469  k}current dateti
+000186b0: 6d65 2069 7320 7b73 7472 2864 6174 6574  me is {str(datet
+000186c0: 696d 652e 6461 7465 7469 6d65 2e6e 6f77  ime.datetime.now
+000186d0: 2829 297d 2e0a 5265 6d65 6d62 6572 2c20  ())}..Remember, 
+000186e0: 7072 6f76 6964 6520 6d65 2077 6974 6820  provide me with 
+000186f0: 7468 6520 696d 7072 6f76 6564 2077 7269  the improved wri
+00018700: 7469 6e67 206f 6e6c 792c 2065 6e63 6c6f  ting only, enclo
+00018710: 7365 6420 696e 2074 7269 706c 6520 7175  sed in triple qu
+00018720: 6f74 6573 2060 6060 2061 6e64 2077 6974  otes ``` and wit
+00018730: 686f 7574 2061 6e79 2061 6464 6974 696f  hout any additio
+00018740: 6e61 6c20 696e 666f 726d 6174 696f 6e20  nal information 
+00018750: 6f72 2063 6f6d 6d65 6e74 732e 0a4d 7920  or comments..My 
+00018760: 7772 6974 696e 673a 0a7b 7573 6572 496e  writing:.{userIn
+00018770: 7075 747d 2222 2229 0a20 2020 2020 2020  put}""").       
+00018780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018790: 2069 6620 696d 7072 6f76 6564 5665 7273   if improvedVers
+000187a0: 696f 6e20 616e 6420 696d 7072 6f76 6564  ion and improved
+000187b0: 5665 7273 696f 6e2e 7374 6172 7473 7769  Version.startswi
+000187c0: 7468 2822 6060 6022 2920 616e 6420 696d  th("```") and im
+000187d0: 7072 6f76 6564 5665 7273 696f 6e2e 656e  provedVersion.en
+000187e0: 6473 7769 7468 2822 6060 6022 293a 0a20  dswith("```"):. 
+000187f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018800: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00018810: 3128 696d 7072 6f76 6564 5665 7273 696f  1(improvedVersio
+00018820: 6e29 0a20 2020 2020 2020 2020 2020 2020  n).             
+00018830: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00018840: 7365 7249 6e70 7574 203d 2069 6d70 726f  serInput = impro
+00018850: 7665 6456 6572 7369 6f6e 5b33 3a2d 335d  vedVersion[3:-3]
+00018860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018880: 636f 6e66 6967 2e74 7473 4f75 7470 7574  config.ttsOutput
+00018890: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000188a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188b0: 2020 5454 5355 7469 6c2e 706c 6179 2875    TTSUtil.play(u
+000188c0: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
+000188d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000188e0: 2073 7065 6369 616c 456e 7472 793a 0a20   specialEntry:. 
+000188f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018900: 2020 2020 2020 2075 7365 7249 6e70 7574         userInput
+00018910: 203d 2066 227b 7573 6572 496e 7075 747d   = f"{userInput}
+00018920: 7b73 7065 6369 616c 456e 7472 797d 220a  {specialEntry}".
+00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018940: 2020 2020 2320 7265 6669 6e65 206d 6573      # refine mes
+00018950: 7361 6765 7320 6265 666f 7265 2072 756e  sages before run
+00018960: 6e69 6e67 2063 6f6d 706c 6574 696f 6e0a  ning completion.
+00018970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018980: 2020 2020 6669 6e65 5475 6e65 6455 7365      fineTunedUse
+00018990: 7249 6e70 7574 203d 2073 656c 662e 6669  rInput = self.fi
+000189a0: 6e65 5475 6e65 5573 6572 496e 7075 7428  neTuneUserInput(
+000189b0: 7573 6572 496e 7075 7429 0a20 2020 2020  userInput).     
+000189c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000189d0: 2069 6e20 6361 7365 206f 6620 7472 616e   in case of tran
+000189e0: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
+000189f0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00018a00: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
+00018a10: 436f 6e74 6578 7420 3d3d 2022 4c65 7420  Context == "Let 
+00018a20: 6d65 2054 7261 6e73 6c61 7465 2220 616e  me Translate" an
+00018a30: 6420 6669 6e65 5475 6e65 6455 7365 7249  d fineTunedUserI
+00018a40: 6e70 7574 2e73 7461 7274 7377 6974 6828  nput.startswith(
+00018a50: 2241 7373 6973 7420 6d65 2062 7920 6163  "Assist me by ac
+00018a60: 7469 6e67 2061 7320 6120 7472 616e 736c  ting as a transl
+00018a70: 6174 6f72 2e5c 6e50 6c65 6173 6520 7472  ator.\nPlease tr
+00018a80: 616e 736c 6174 6522 293a 0a20 2020 2020  anslate"):.     
+00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018aa0: 2020 2070 7269 6e74 3128 2250 6c65 6173     print1("Pleas
+00018ab0: 6520 7370 6563 6966 7920 6265 6c6f 7720  e specify below 
+00018ac0: 7468 6520 6c61 6e67 7561 6765 2079 6f75  the language you
+00018ad0: 2077 6f75 6c64 206c 696b 6520 7468 6520   would like the 
+00018ae0: 636f 6e74 656e 7420 746f 2062 6520 7472  content to be tr
+00018af0: 616e 736c 6174 6564 2069 6e74 6f3a 2229  anslated into:")
+00018b00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018b10: 2020 2020 2020 2020 206c 616e 6775 6167           languag
+00018b20: 6520 3d20 7365 6c66 2e70 726f 6d70 7473  e = self.prompts
+00018b30: 2e73 696d 706c 6550 726f 6d70 7428 7374  .simplePrompt(st
+00018b40: 796c 653d 7365 6c66 2e70 726f 6d70 7473  yle=self.prompts
+00018b50: 2e70 726f 6d70 7453 7479 6c65 322c 2064  .promptStyle2, d
+00018b60: 6566 6175 6c74 3d63 6f6e 6669 672e 7472  efault=config.tr
+00018b70: 616e 736c 6174 6554 6f4c 616e 6775 6167  anslateToLanguag
+00018b80: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00018b90: 2020 2020 2020 2020 2020 2069 6620 6c61             if la
+00018ba0: 6e67 7561 6765 2061 6e64 206e 6f74 206c  nguage and not l
+00018bb0: 616e 6775 6167 652e 7374 7269 7028 292e  anguage.strip().
+00018bc0: 6c6f 7765 7228 2920 696e 2028 636f 6e66  lower() in (conf
+00018bd0: 6967 2e63 616e 6365 6c5f 656e 7472 792c  ig.cancel_entry,
+00018be0: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
+00018bf0: 7279 293a 0a20 2020 2020 2020 2020 2020  ry):.           
+00018c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c10: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
+00018c20: 7075 7420 3d20 6622 7b66 696e 6554 756e  put = f"{fineTun
+00018c30: 6564 5573 6572 496e 7075 747d 5c6e 5c6e  edUserInput}\n\n
+00018c40: 506c 6561 7365 2074 7261 6e73 6c61 7465  Please translate
+00018c50: 2074 6865 2063 6f6e 7465 6e74 2069 6e74   the content int
+00018c60: 6f20 3c6c 616e 6775 6167 653e 7b6c 616e  o <language>{lan
+00018c70: 6775 6167 657d 3c2f 6c61 6e67 7561 6765  guage}</language
+00018c80: 3e2e 220a 2020 2020 2020 2020 2020 2020  >.".            
+00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 636f 6e66 6967 2e74 7261 6e73 6c61 7465  config.translate
+00018cb0: 546f 4c61 6e67 7561 6765 203d 206c 616e  ToLanguage = lan
+00018cc0: 6775 6167 650a 2020 2020 2020 2020 2020  guage.          
+00018cd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00018ce0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
 00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d00: 2020 2023 2063 6c65 6172 2063 6f6e 6669     # clear confi
-00018d10: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
-00018d20: 6578 7454 656d 7020 6966 2061 6e79 0a20  extTemp if any. 
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d40: 2020 2069 6620 636f 6e66 6967 2e70 7265     if config.pre
-00018d50: 6465 6669 6e65 6443 6f6e 7465 7874 5465  definedContextTe
-00018d60: 6d70 3a0a 2020 2020 2020 2020 2020 2020  mp:.            
-00018d70: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00018d80: 6967 2e70 7265 6465 6669 6e65 6443 6f6e  ig.predefinedCon
-00018d90: 7465 7874 203d 2063 6f6e 6669 672e 7072  text = config.pr
-00018da0: 6564 6566 696e 6564 436f 6e74 6578 7454  edefinedContextT
-00018db0: 656d 700a 2020 2020 2020 2020 2020 2020  emp.            
-00018dc0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00018dd0: 6967 2e70 7265 6465 6669 6e65 6443 6f6e  ig.predefinedCon
-00018de0: 7465 7874 5465 6d70 203d 2022 220a 2020  textTemp = "".  
-00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e00: 2020 2320 656d 7074 7920 636f 6e66 6967    # empty config
-00018e10: 2e70 6167 6572 436f 6e74 656e 740a 2020  .pagerContent.  
-00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e30: 2020 636f 6e66 6967 2e70 6167 6572 436f    config.pagerCo
-00018e40: 6e74 656e 7420 3d20 2222 0a0a 2020 2020  ntent = ""..    
-00018e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e60: 2320 6368 6563 6b20 7370 6563 6961 6c20  # check special 
-00018e70: 656e 7472 6965 730a 2020 2020 2020 2020  entries.        
-00018e80: 2020 2020 2020 2020 2020 2020 2320 6966              # if
-00018e90: 2075 7365 7220 6361 6c6c 2061 2063 6861   user call a cha
-00018ea0: 7462 6f74 2077 6974 686f 7574 2066 756e  tbot without fun
-00018eb0: 6374 696f 6e20 6361 6c6c 696e 670a 2020  ction calling.  
-00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ed0: 2020 6966 2022 5b43 4841 545d 2220 696e    if "[CHAT]" in
-00018ee0: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
-00018ef0: 7075 743a 0a20 2020 2020 2020 2020 2020  put:.           
-00018f00: 2020 2020 2020 2020 2020 2020 2063 6861               cha
-00018f10: 7462 6f74 203d 2063 6f6e 6669 672e 6c6c  tbot = config.ll
-00018f20: 6d49 6e74 6572 6661 6365 0a20 2020 2020  mInterface.     
-00018f30: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018f40: 6c69 6620 6361 6c6c 4368 6174 426f 7420  lif callChatBot 
-00018f50: 3a3d 2072 652e 7365 6172 6368 2822 5c5b  := re.search("\[
-00018f60: 4348 4154 5f28 5b5e 5c5b 5c5d 5d2b 3f29  CHAT_([^\[\]]+?)
-00018f70: 5c5d 222c 2066 696e 6554 756e 6564 5573  \]", fineTunedUs
-00018f80: 6572 496e 7075 7429 3a0a 2020 2020 2020  erInput):.      
-00018f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fa0: 2020 6368 6174 626f 7420 3d20 6361 6c6c    chatbot = call
-00018fb0: 4368 6174 426f 742e 6772 6f75 7028 3129  ChatBot.group(1)
-00018fc0: 2e6c 6f77 6572 2829 2069 6620 6361 6c6c  .lower() if call
-00018fd0: 4368 6174 426f 7420 616e 6420 6361 6c6c  ChatBot and call
-00018fe0: 4368 6174 426f 742e 6772 6f75 7028 3129  ChatBot.group(1)
-00018ff0: 2e6c 6f77 6572 2829 2069 6e20 2822 6368  .lower() in ("ch
-00019000: 6174 6770 7422 2c20 2267 656d 696e 6970  atgpt", "geminip
-00019010: 726f 222c 2022 7061 6c6d 3222 2c20 2263  ro", "palm2", "c
-00019020: 6f64 6579 2229 2065 6c73 6520 2222 0a20  odey") else "". 
-00019030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019040: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00019050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019060: 2063 6861 7462 6f74 203d 2022 220a 2020   chatbot = "".  
-00019070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019080: 2020 6966 2063 6861 7462 6f74 3a0a 2020    if chatbot:.  
-00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190a0: 2020 2020 2020 2320 6361 6c6c 2074 6865        # call the
-000190b0: 2073 7063 6966 6965 6420 6368 6174 626f   spcified chatbo
-000190c0: 7420 746f 2063 6f6e 7469 6e75 6520 7468  t to continue th
-000190d0: 6520 636f 6e76 6572 7361 7469 6f6e 0a20  e conversation. 
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2066 696e 6554 756e 6564         fineTuned
-00019100: 5573 6572 496e 7075 7420 3d20 7265 2e73  UserInput = re.s
-00019110: 7562 2822 5c5b 4348 4154 5c5d 7c5c 5b43  ub("\[CHAT\]|\[C
-00019120: 4841 545f 5b5e 5c5b 5c5d 5d2b 3f5c 5d22  HAT_[^\[\]]+?\]"
-00019130: 2c20 2222 2c20 6669 6e65 5475 6e65 6455  , "", fineTunedU
-00019140: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
-00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019160: 2020 7365 6c66 2e6c 6175 6e63 6843 6861    self.launchCha
-00019170: 7462 6f74 2863 6861 7462 6f74 2c20 6669  tbot(chatbot, fi
-00019180: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-00019190: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000191a0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-000191b0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-000191c0: 2020 2020 2020 2023 2077 6865 6e20 7573         # when us
-000191d0: 6572 2064 6f6e 2774 2077 616e 7420 6120  er don't want a 
-000191e0: 6675 6e63 7469 6f6e 2063 616c 6c0a 2020  function call.  
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 6e6f 4675 6e63 7469 6f6e 4361 6c6c    noFunctionCall
-00019210: 203d 2028 225b 4e4f 5f54 4f4f 4c5d 2220   = ("[NO_TOOL]" 
-00019220: 696e 2066 696e 6554 756e 6564 5573 6572  in fineTunedUser
-00019230: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
-00019240: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
-00019250: 6e20 7573 6572 2077 616e 7420 746f 2063  n user want to c
-00019260: 616c 6c20 6120 7061 7274 6963 756c 6172  all a particular
-00019270: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-00019280: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00019290: 6563 6b43 616c 6c53 7065 6369 6669 6346  eckCallSpecificF
-000192a0: 756e 6374 696f 6e20 3d20 7265 2e73 6561  unction = re.sea
-000192b0: 7263 6828 225c 5b54 4f4f 4c5f 285b 5e5c  rch("\[TOOL_([^\
-000192c0: 5b5c 5d5d 2b3f 295c 5d22 2c20 6669 6e65  [\]]+?)\]", fine
-000192d0: 5475 6e65 6455 7365 7249 6e70 7574 290a  TunedUserInput).
-000192e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000192f0: 2020 2020 636f 6e66 6967 2e73 656c 6563      config.selec
-00019300: 7465 6454 6f6f 6c20 3d20 6368 6563 6b43  tedTool = checkC
-00019310: 616c 6c53 7065 6369 6669 6346 756e 6374  allSpecificFunct
-00019320: 696f 6e2e 6772 6f75 7028 3129 2069 6620  ion.group(1) if 
-00019330: 6368 6563 6b43 616c 6c53 7065 6369 6669  checkCallSpecifi
-00019340: 6346 756e 6374 696f 6e20 616e 6420 6368  cFunction and ch
-00019350: 6563 6b43 616c 6c53 7065 6369 6669 6346  eckCallSpecificF
-00019360: 756e 6374 696f 6e2e 6772 6f75 7028 3129  unction.group(1)
-00019370: 2069 6e20 636f 6e66 6967 2e74 6f6f 6c46   in config.toolF
-00019380: 756e 6374 696f 6e4d 6574 686f 6473 2065  unctionMethods e
-00019390: 6c73 6520 2222 0a20 2020 2020 2020 2020  lse "".         
-000193a0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-000193b0: 6e66 6967 2e64 6576 656c 6f70 6572 2061  nfig.developer a
-000193c0: 6e64 2063 6f6e 6669 672e 7365 6c65 6374  nd config.select
-000193d0: 6564 546f 6f6c 3a0a 2020 2020 2020 2020  edTool:.        
-000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000193f0: 2370 7269 6e74 3128 6622 6361 6c6c 696e  #print1(f"callin
-00019400: 6720 6675 6e63 7469 6f6e 2027 7b63 6f6e  g function '{con
-00019410: 6669 672e 7365 6c65 6374 6564 546f 6f6c  fig.selectedTool
-00019420: 7d27 202e 2e2e 2229 0a20 2020 2020 2020  }' ...").       
-00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019440: 2070 7269 6e74 5f66 6f72 6d61 7474 6564   print_formatted
-00019450: 5f74 6578 7428 4854 4d4c 2866 223c 7b63  _text(HTML(f"<{c
-00019460: 6f6e 6669 672e 7465 726d 696e 616c 5072  onfig.terminalPr
-00019470: 6f6d 7074 496e 6469 6361 746f 7243 6f6c  omptIndicatorCol
-00019480: 6f72 327d 3e43 616c 6c69 6e67 2066 756e  or2}>Calling fun
-00019490: 6374 696f 6e3c 2f7b 636f 6e66 6967 2e74  ction</{config.t
-000194a0: 6572 6d69 6e61 6c50 726f 6d70 7449 6e64  erminalPromptInd
-000194b0: 6963 6174 6f72 436f 6c6f 7232 7d3e 203c  icatorColor2}> <
-000194c0: 7b63 6f6e 6669 672e 7465 726d 696e 616c  {config.terminal
-000194d0: 436f 6d6d 616e 6445 6e74 7279 436f 6c6f  CommandEntryColo
-000194e0: 7232 7d3e 277b 636f 6e66 6967 2e73 656c  r2}>'{config.sel
-000194f0: 6563 7465 6454 6f6f 6c7d 273c 2f7b 636f  ectedTool}'</{co
-00019500: 6e66 6967 2e74 6572 6d69 6e61 6c43 6f6d  nfig.terminalCom
-00019510: 6d61 6e64 456e 7472 7943 6f6c 6f72 327d  mandEntryColor2}
-00019520: 3e20 3c7b 636f 6e66 6967 2e74 6572 6d69  > <{config.termi
-00019530: 6e61 6c50 726f 6d70 7449 6e64 6963 6174  nalPromptIndicat
-00019540: 6f72 436f 6c6f 7232 7d3e 2e2e 2e3c 2f7b  orColor2}>...</{
-00019550: 636f 6e66 6967 2e74 6572 6d69 6e61 6c50  config.terminalP
-00019560: 726f 6d70 7449 6e64 6963 6174 6f72 436f  romptIndicatorCo
-00019570: 6c6f 7232 7d3e 2229 290a 2020 2020 2020  lor2}>")).      
-00019580: 2020 2020 2020 2020 2020 2020 2020 6669                fi
-00019590: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-000195a0: 203d 2072 652e 7375 6228 7370 6563 6961   = re.sub(specia
-000195b0: 6c45 6e74 7279 5061 7474 6572 6e2c 2022  lEntryPattern, "
-000195c0: 222c 2066 696e 6554 756e 6564 5573 6572  ", fineTunedUser
-000195d0: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
-000195e0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-000195f0: 672e 6375 7272 656e 744d 6573 7361 6765  g.currentMessage
-00019600: 732e 6170 7065 6e64 287b 2272 6f6c 6522  s.append({"role"
-00019610: 3a20 2275 7365 7222 2c20 2263 6f6e 7465  : "user", "conte
-00019620: 6e74 223a 2066 696e 6554 756e 6564 5573  nt": fineTunedUs
-00019630: 6572 496e 7075 747d 290a 0a20 2020 2020  erInput})..     
-00019640: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00019650: 2073 7461 7274 2073 7069 6e6e 696e 670a   start spinning.
-00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019670: 2020 2020 636f 6e66 6967 2e73 746f 705f      config.stop_
-00019680: 6576 656e 7420 3d20 7468 7265 6164 696e  event = threadin
-00019690: 672e 4576 656e 7428 290a 2020 2020 2020  g.Event().      
-000196a0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000196b0: 6e66 6967 2e73 7069 6e6e 6572 5f74 6872  nfig.spinner_thr
-000196c0: 6561 6420 3d20 7468 7265 6164 696e 672e  ead = threading.
-000196d0: 5468 7265 6164 2874 6172 6765 743d 7370  Thread(target=sp
-000196e0: 696e 6e69 6e67 5f61 6e69 6d61 7469 6f6e  inning_animation
-000196f0: 2c20 6172 6773 3d28 636f 6e66 6967 2e73  , args=(config.s
-00019700: 746f 705f 6576 656e 742c 2929 0a20 2020  top_event,)).   
-00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019720: 2063 6f6e 6669 672e 7370 696e 6e65 725f   config.spinner_
-00019730: 7468 7265 6164 2e73 7461 7274 2829 0a0a  thread.start()..
-00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 2020 2020 2320 666f 7263 6520 6c6f 6164      # force load
-00019760: 696e 6720 696e 7465 726e 6574 2073 6561  ing internet sea
-00019770: 7263 6865 730a 2020 2020 2020 2020 2020  rches.          
-00019780: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-00019790: 6669 672e 6c6f 6164 696e 6749 6e74 6572  fig.loadingInter
-000197a0: 6e65 7453 6561 7263 6865 7320 3d3d 2022  netSearches == "
-000197b0: 616c 7761 7973 223a 0a20 2020 2020 2020  always":.       
-000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197f0: 2020 636f 6e66 6967 2e63 7572 7265 6e74    config.current
-00019800: 4d65 7373 6167 6573 203d 2043 616c 6c4c  Messages = CallL
-00019810: 4c4d 2e72 756e 5369 6e67 6c65 4675 6e63  LM.runSingleFunc
-00019820: 7469 6f6e 4361 6c6c 2863 6f6e 6669 672e  tionCall(config.
-00019830: 6375 7272 656e 744d 6573 7361 6765 732c  currentMessages,
-00019840: 2022 696e 7465 6772 6174 655f 676f 6f67   "integrate_goog
-00019850: 6c65 5f73 6561 7263 6865 7322 290a 2020  le_searches").  
-00019860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019870: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00018d00: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00018d10: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+00018d20: 6c65 6172 2063 6f6e 6669 672e 7072 6564  lear config.pred
+00018d30: 6566 696e 6564 436f 6e74 6578 7454 656d  efinedContextTem
+00018d40: 7020 6966 2061 6e79 0a20 2020 2020 2020  p if any.       
+00018d50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018d60: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
+00018d70: 6443 6f6e 7465 7874 5465 6d70 3a0a 2020  dContextTemp:.  
+00018d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d90: 2020 2020 2020 636f 6e66 6967 2e70 7265        config.pre
+00018da0: 6465 6669 6e65 6443 6f6e 7465 7874 203d  definedContext =
+00018db0: 2063 6f6e 6669 672e 7072 6564 6566 696e   config.predefin
+00018dc0: 6564 436f 6e74 6578 7454 656d 700a 2020  edContextTemp.  
+00018dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018de0: 2020 2020 2020 636f 6e66 6967 2e70 7265        config.pre
+00018df0: 6465 6669 6e65 6443 6f6e 7465 7874 5465  definedContextTe
+00018e00: 6d70 203d 2022 220a 2020 2020 2020 2020  mp = "".        
+00018e10: 2020 2020 2020 2020 2020 2020 2320 656d              # em
+00018e20: 7074 7920 636f 6e66 6967 2e70 6167 6572  pty config.pager
+00018e30: 436f 6e74 656e 740a 2020 2020 2020 2020  Content.        
+00018e40: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00018e50: 6967 2e70 6167 6572 436f 6e74 656e 7420  ig.pagerContent 
+00018e60: 3d20 2222 0a0a 2020 2020 2020 2020 2020  = ""..          
+00018e70: 2020 2020 2020 2020 2020 2320 6368 6563            # chec
+00018e80: 6b20 7370 6563 6961 6c20 656e 7472 6965  k special entrie
+00018e90: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00018ea0: 2020 2020 2020 2320 6966 2075 7365 7220        # if user 
+00018eb0: 6361 6c6c 2061 2063 6861 7462 6f74 2077  call a chatbot w
+00018ec0: 6974 686f 7574 2066 756e 6374 696f 6e20  ithout function 
+00018ed0: 6361 6c6c 696e 670a 2020 2020 2020 2020  calling.        
+00018ee0: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00018ef0: 5b43 4841 545d 2220 696e 2066 696e 6554  [CHAT]" in fineT
+00018f00: 756e 6564 5573 6572 496e 7075 743a 0a20  unedUserInput:. 
+00018f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f20: 2020 2020 2020 2063 6861 7462 6f74 203d         chatbot =
+00018f30: 2063 6f6e 6669 672e 6c6c 6d49 6e74 6572   config.llmInter
+00018f40: 6661 6365 0a20 2020 2020 2020 2020 2020  face.           
+00018f50: 2020 2020 2020 2020 2065 6c69 6620 6361           elif ca
+00018f60: 6c6c 4368 6174 426f 7420 3a3d 2072 652e  llChatBot := re.
+00018f70: 7365 6172 6368 2822 5c5b 4348 4154 5f28  search("\[CHAT_(
+00018f80: 5b5e 5c5b 5c5d 5d2b 3f29 5c5d 222c 2066  [^\[\]]+?)\]", f
+00018f90: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+00018fa0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00018fb0: 2020 2020 2020 2020 2020 2020 6368 6174              chat
+00018fc0: 626f 7420 3d20 6361 6c6c 4368 6174 426f  bot = callChatBo
+00018fd0: 742e 6772 6f75 7028 3129 2e6c 6f77 6572  t.group(1).lower
+00018fe0: 2829 2069 6620 6361 6c6c 4368 6174 426f  () if callChatBo
+00018ff0: 7420 616e 6420 6361 6c6c 4368 6174 426f  t and callChatBo
+00019000: 742e 6772 6f75 7028 3129 2e6c 6f77 6572  t.group(1).lower
+00019010: 2829 2069 6e20 2822 6368 6174 6770 7422  () in ("chatgpt"
+00019020: 2c20 2267 656d 696e 6970 726f 222c 2022  , "geminipro", "
+00019030: 7061 6c6d 3222 2c20 2263 6f64 6579 2229  palm2", "codey")
+00019040: 2065 6c73 6520 2222 0a20 2020 2020 2020   else "".       
+00019050: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00019060: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00019070: 2020 2020 2020 2020 2020 2063 6861 7462             chatb
+00019080: 6f74 203d 2022 220a 2020 2020 2020 2020  ot = "".        
+00019090: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+000190a0: 6861 7462 6f74 3a0a 2020 2020 2020 2020  hatbot:.        
+000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190c0: 2320 6361 6c6c 2074 6865 2073 7063 6966  # call the spcif
+000190d0: 6965 6420 6368 6174 626f 7420 746f 2063  ied chatbot to c
+000190e0: 6f6e 7469 6e75 6520 7468 6520 636f 6e76  ontinue the conv
+000190f0: 6572 7361 7469 6f6e 0a20 2020 2020 2020  ersation.       
+00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019110: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
+00019120: 7075 7420 3d20 7265 2e73 7562 2822 5c5b  put = re.sub("\[
+00019130: 4348 4154 5c5d 7c5c 5b43 4841 545f 5b5e  CHAT\]|\[CHAT_[^
+00019140: 5c5b 5c5d 5d2b 3f5c 5d22 2c20 2222 2c20  \[\]]+?\]", "", 
+00019150: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
+00019160: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+00019170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019180: 2e6c 6175 6e63 6843 6861 7462 6f74 2863  .launchChatbot(c
+00019190: 6861 7462 6f74 2c20 6669 6e65 5475 6e65  hatbot, fineTune
+000191a0: 6455 7365 7249 6e70 7574 290a 2020 2020  dUserInput).    
+000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191c0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+000191d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191e0: 2023 2077 6865 6e20 7573 6572 2064 6f6e   # when user don
+000191f0: 2774 2077 616e 7420 6120 6675 6e63 7469  't want a functi
+00019200: 6f6e 2063 616c 6c0a 2020 2020 2020 2020  on call.        
+00019210: 2020 2020 2020 2020 2020 2020 6e6f 4675              noFu
+00019220: 6e63 7469 6f6e 4361 6c6c 203d 2028 225b  nctionCall = ("[
+00019230: 4e4f 5f54 4f4f 4c5d 2220 696e 2066 696e  NO_TOOL]" in fin
+00019240: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
+00019250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019260: 2020 2020 2023 2077 6865 6e20 7573 6572       # when user
+00019270: 2077 616e 7420 746f 2063 616c 6c20 6120   want to call a 
+00019280: 7061 7274 6963 756c 6172 2066 756e 6374  particular funct
+00019290: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000192a0: 2020 2020 2020 2020 6368 6563 6b43 616c          checkCal
+000192b0: 6c53 7065 6369 6669 6346 756e 6374 696f  lSpecificFunctio
+000192c0: 6e20 3d20 7265 2e73 6561 7263 6828 225c  n = re.search("\
+000192d0: 5b54 4f4f 4c5f 285b 5e5c 5b5c 5d5d 2b3f  [TOOL_([^\[\]]+?
+000192e0: 295c 5d22 2c20 6669 6e65 5475 6e65 6455  )\]", fineTunedU
+000192f0: 7365 7249 6e70 7574 290a 2020 2020 2020  serInput).      
+00019300: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00019310: 6e66 6967 2e73 656c 6563 7465 6454 6f6f  nfig.selectedToo
+00019320: 6c20 3d20 6368 6563 6b43 616c 6c53 7065  l = checkCallSpe
+00019330: 6369 6669 6346 756e 6374 696f 6e2e 6772  cificFunction.gr
+00019340: 6f75 7028 3129 2069 6620 6368 6563 6b43  oup(1) if checkC
+00019350: 616c 6c53 7065 6369 6669 6346 756e 6374  allSpecificFunct
+00019360: 696f 6e20 616e 6420 6368 6563 6b43 616c  ion and checkCal
+00019370: 6c53 7065 6369 6669 6346 756e 6374 696f  lSpecificFunctio
+00019380: 6e2e 6772 6f75 7028 3129 2069 6e20 636f  n.group(1) in co
+00019390: 6e66 6967 2e74 6f6f 6c46 756e 6374 696f  nfig.toolFunctio
+000193a0: 6e4d 6574 686f 6473 2065 6c73 6520 2222  nMethods else ""
+000193b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000193c0: 2020 2020 2069 6620 636f 6e66 6967 2e64       if config.d
+000193d0: 6576 656c 6f70 6572 2061 6e64 2063 6f6e  eveloper and con
+000193e0: 6669 672e 7365 6c65 6374 6564 546f 6f6c  fig.selectedTool
+000193f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019400: 2020 2020 2020 2020 2020 2370 7269 6e74            #print
+00019410: 3128 6622 6361 6c6c 696e 6720 6675 6e63  1(f"calling func
+00019420: 7469 6f6e 2027 7b63 6f6e 6669 672e 7365  tion '{config.se
+00019430: 6c65 6374 6564 546f 6f6c 7d27 202e 2e2e  lectedTool}' ...
+00019440: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00019450: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00019460: 5f66 6f72 6d61 7474 6564 5f74 6578 7428  _formatted_text(
+00019470: 4854 4d4c 2866 223c 7b63 6f6e 6669 672e  HTML(f"<{config.
+00019480: 7465 726d 696e 616c 5072 6f6d 7074 496e  terminalPromptIn
+00019490: 6469 6361 746f 7243 6f6c 6f72 327d 3e43  dicatorColor2}>C
+000194a0: 616c 6c69 6e67 2066 756e 6374 696f 6e3c  alling function<
+000194b0: 2f7b 636f 6e66 6967 2e74 6572 6d69 6e61  /{config.termina
+000194c0: 6c50 726f 6d70 7449 6e64 6963 6174 6f72  lPromptIndicator
+000194d0: 436f 6c6f 7232 7d3e 203c 7b63 6f6e 6669  Color2}> <{confi
+000194e0: 672e 7465 726d 696e 616c 436f 6d6d 616e  g.terminalComman
+000194f0: 6445 6e74 7279 436f 6c6f 7232 7d3e 277b  dEntryColor2}>'{
+00019500: 636f 6e66 6967 2e73 656c 6563 7465 6454  config.selectedT
+00019510: 6f6f 6c7d 273c 2f7b 636f 6e66 6967 2e74  ool}'</{config.t
+00019520: 6572 6d69 6e61 6c43 6f6d 6d61 6e64 456e  erminalCommandEn
+00019530: 7472 7943 6f6c 6f72 327d 3e20 3c7b 636f  tryColor2}> <{co
+00019540: 6e66 6967 2e74 6572 6d69 6e61 6c50 726f  nfig.terminalPro
+00019550: 6d70 7449 6e64 6963 6174 6f72 436f 6c6f  mptIndicatorColo
+00019560: 7232 7d3e 2e2e 2e3c 2f7b 636f 6e66 6967  r2}>...</{config
+00019570: 2e74 6572 6d69 6e61 6c50 726f 6d70 7449  .terminalPromptI
+00019580: 6e64 6963 6174 6f72 436f 6c6f 7232 7d3e  ndicatorColor2}>
+00019590: 2229 290a 2020 2020 2020 2020 2020 2020  ")).            
+000195a0: 2020 2020 2020 2020 6669 6e65 5475 6e65          fineTune
+000195b0: 6455 7365 7249 6e70 7574 203d 2072 652e  dUserInput = re.
+000195c0: 7375 6228 7370 6563 6961 6c45 6e74 7279  sub(specialEntry
+000195d0: 5061 7474 6572 6e2c 2022 222c 2066 696e  Pattern, "", fin
+000195e0: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
+000195f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019600: 2020 2020 2063 6f6e 6669 672e 6375 7272       config.curr
+00019610: 656e 744d 6573 7361 6765 732e 6170 7065  entMessages.appe
+00019620: 6e64 287b 2272 6f6c 6522 3a20 2275 7365  nd({"role": "use
+00019630: 7222 2c20 2263 6f6e 7465 6e74 223a 2066  r", "content": f
+00019640: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+00019650: 747d 290a 0a20 2020 2020 2020 2020 2020  t})..           
+00019660: 2020 2020 2020 2020 2023 2073 7461 7274           # start
+00019670: 2073 7069 6e6e 696e 670a 2020 2020 2020   spinning.      
+00019680: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00019690: 6e66 6967 2e73 746f 705f 6576 656e 7420  nfig.stop_event 
+000196a0: 3d20 7468 7265 6164 696e 672e 4576 656e  = threading.Even
+000196b0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
+000196c0: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+000196d0: 7069 6e6e 6572 5f74 6872 6561 6420 3d20  pinner_thread = 
+000196e0: 7468 7265 6164 696e 672e 5468 7265 6164  threading.Thread
+000196f0: 2874 6172 6765 743d 7370 696e 6e69 6e67  (target=spinning
+00019700: 5f61 6e69 6d61 7469 6f6e 2c20 6172 6773  _animation, args
+00019710: 3d28 636f 6e66 6967 2e73 746f 705f 6576  =(config.stop_ev
+00019720: 656e 742c 2929 0a20 2020 2020 2020 2020  ent,)).         
+00019730: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00019740: 672e 7370 696e 6e65 725f 7468 7265 6164  g.spinner_thread
+00019750: 2e73 7461 7274 2829 0a0a 2020 2020 2020  .start()..      
+00019760: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00019770: 666f 7263 6520 6c6f 6164 696e 6720 696e  force loading in
+00019780: 7465 726e 6574 2073 6561 7263 6865 730a  ternet searches.
+00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 2020 2020 6966 2063 6f6e 6669 672e 6c6f      if config.lo
+000197b0: 6164 696e 6749 6e74 6572 6e65 7453 6561  adingInternetSea
+000197c0: 7263 6865 7320 3d3d 2022 616c 7761 7973  rches == "always
+000197d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+000197e0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+000197f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019800: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00019810: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
+00019820: 6573 203d 2043 616c 6c4c 4c4d 2e72 756e  es = CallLLM.run
+00019830: 5369 6e67 6c65 4675 6e63 7469 6f6e 4361  SingleFunctionCa
+00019840: 6c6c 2863 6f6e 6669 672e 6375 7272 656e  ll(config.curren
+00019850: 744d 6573 7361 6765 732c 2022 696e 7465  tMessages, "inte
+00019860: 6772 6174 655f 676f 6f67 6c65 5f73 6561  grate_google_sea
+00019870: 7263 6865 7322 290a 2020 2020 2020 2020  rches").        
 00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019890: 2020 2020 2020 2020 2020 7072 696e 7431            print1
-000198a0: 2822 556e 6162 6c65 2074 6f20 6c6f 6164  ("Unable to load
-000198b0: 2069 6e74 6572 6e65 7420 7265 736f 7572   internet resour
-000198c0: 6365 732e 2229 0a20 2020 2020 2020 2020  ces.").         
-000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198e0: 2020 2073 686f 7745 7272 6f72 7328 290a     showErrors().
-000198f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019900: 2020 2020 2063 6f6d 706c 6574 696f 6e20       completion 
-00019910: 3d20 4361 6c6c 4c4c 4d2e 7275 6e47 656e  = CallLLM.runGen
-00019920: 6975 7343 616c 6c28 636f 6e66 6967 2e63  iusCall(config.c
-00019930: 7572 7265 6e74 4d65 7373 6167 6573 2c20  urrentMessages, 
-00019940: 6e6f 4675 6e63 7469 6f6e 4361 6c6c 290a  noFunctionCall).
-00019950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019960: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00019970: 2020 2020 2020 2020 2023 2073 746f 7020           # stop 
-00019980: 7370 696e 6e69 6e67 0a20 2020 2020 2020  spinning.       
-00019990: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000199a0: 6669 672e 7275 6e50 7974 686f 6e20 3d20  fig.runPython = 
-000199b0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-000199c0: 2020 2020 2020 2020 2073 746f 7053 7069           stopSpi
-000199d0: 6e6e 696e 6728 290a 0a20 2020 2020 2020  nning()..       
-000199e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000199f0: 636f 6d70 6c65 7469 6f6e 2069 7320 6e6f  completion is no
-00019a00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00019a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a20: 2320 4372 6561 7465 2061 206e 6577 2074  # Create a new t
-00019a30: 6872 6561 6420 666f 7220 7468 6520 7374  hread for the st
-00019a40: 7265 616d 696e 6720 7461 736b 0a20 2020  reaming task.   
-00019a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a60: 2020 2020 2073 7472 6561 6d69 6e67 576f       streamingWo
-00019a70: 7264 5772 6170 7065 7220 3d20 5374 7265  rdWrapper = Stre
-00019a80: 616d 696e 6757 6f72 6457 7261 7070 6572  amingWordWrapper
-00019a90: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00019aa0: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-00019ab0: 6d69 6e67 5f65 7665 6e74 203d 2074 6872  ming_event = thr
-00019ac0: 6561 6469 6e67 2e45 7665 6e74 2829 0a20  eading.Event(). 
-00019ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ae0: 2020 2020 2020 2073 656c 662e 7374 7265         self.stre
-00019af0: 616d 696e 675f 7468 7265 6164 203d 2074  aming_thread = t
-00019b00: 6872 6561 6469 6e67 2e54 6872 6561 6428  hreading.Thread(
-00019b10: 7461 7267 6574 3d73 7472 6561 6d69 6e67  target=streaming
-00019b20: 576f 7264 5772 6170 7065 722e 7374 7265  WordWrapper.stre
-00019b30: 616d 4f75 7470 7574 732c 2061 7267 733d  amOutputs, args=
-00019b40: 2873 7472 6561 6d69 6e67 5f65 7665 6e74  (streaming_event
-00019b50: 2c20 636f 6d70 6c65 7469 6f6e 2c20 5472  , completion, Tr
-00019b60: 7565 2069 6620 636f 6e66 6967 2e6c 6c6d  ue if config.llm
-00019b70: 496e 7465 7266 6163 6520 696e 2028 2263  Interface in ("c
-00019b80: 6861 7467 7074 222c 2022 6c65 746d 6564  hatgpt", "letmed
-00019b90: 6f69 7422 2c20 2267 726f 7122 2920 656c  oit", "groq") el
-00019ba0: 7365 2046 616c 7365 2929 0a20 2020 2020  se False)).     
-00019bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bc0: 2020 2023 2053 7461 7274 2074 6865 2073     # Start the s
-00019bd0: 7472 6561 6d69 6e67 2074 6872 6561 640a  treaming thread.
-00019be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019bf0: 2020 2020 2020 2020 7365 6c66 2e73 7472          self.str
-00019c00: 6561 6d69 6e67 5f74 6872 6561 642e 7374  eaming_thread.st
-00019c10: 6172 7428 290a 0a20 2020 2020 2020 2020  art()..         
-00019c20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00019c30: 2077 6169 7420 7768 696c 6520 7465 7874   wait while text
-00019c40: 206f 7574 7075 7420 6973 2073 7465 616d   output is steam
-00019c50: 696e 673b 2063 6170 7475 7265 206b 6579  ing; capture key
-00019c60: 2063 6f6d 626f 2027 6374 726c 2b71 2720   combo 'ctrl+q' 
-00019c70: 6f72 2027 6374 726c 2b7a 2720 746f 2073  or 'ctrl+z' to s
-00019c80: 746f 7020 7468 6520 7374 7265 616d 696e  top the streamin
-00019c90: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00019ca0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-00019cb0: 696e 6757 6f72 6457 7261 7070 6572 2e6b  ingWordWrapper.k
-00019cc0: 6579 546f 5374 6f70 5374 7265 616d 696e  eyToStopStreamin
-00019cd0: 6728 7374 7265 616d 696e 675f 6576 656e  g(streaming_even
-00019ce0: 7429 0a0a 2020 2020 2020 2020 2020 2020  t)..            
-00019cf0: 2020 2020 2020 2020 2020 2020 2320 7768              # wh
-00019d00: 656e 2073 7472 6561 6d69 6e67 2069 7320  en streaming is 
-00019d10: 646f 6e65 206f 7220 7768 656e 2075 7365  done or when use
-00019d20: 7220 7072 6573 7320 2263 7472 6c2b 7122  r press "ctrl+q"
-00019d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019d40: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-00019d50: 7265 616d 696e 675f 7468 7265 6164 2e6a  reaming_thread.j
-00019d60: 6f69 6e28 290a 0a20 2020 2020 2020 2020  oin()..         
-00019d70: 2020 2020 2020 2023 2065 7272 6f72 2063         # error c
-00019d80: 6f64 6573 3a20 6874 7470 733a 2f2f 706c  odes: https://pl
-00019d90: 6174 666f 726d 2e6f 7065 6e61 692e 636f  atform.openai.co
-00019da0: 6d2f 646f 6373 2f67 7569 6465 732f 6572  m/docs/guides/er
-00019db0: 726f 722d 636f 6465 732f 7079 7468 6f6e  ror-codes/python
-00019dc0: 2d6c 6962 7261 7279 2d65 7272 6f72 2d74  -library-error-t
-00019dd0: 7970 6573 0a20 2020 2020 2020 2020 2020  ypes.           
-00019de0: 2020 2020 2065 7863 6570 7420 6f70 656e       except open
-00019df0: 6169 2e41 5049 4572 726f 7220 6173 2065  ai.APIError as e
-00019e00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019e10: 2020 2020 2020 7374 6f70 5370 696e 6e69        stopSpinni
-00019e20: 6e67 2829 0a20 2020 2020 2020 2020 2020  ng().           
-00019e30: 2020 2020 2020 2020 2023 4861 6e64 6c65           #Handle
-00019e40: 2041 5049 2065 7272 6f72 2068 6572 652c   API error here,
-00019e50: 2065 2e67 2e20 7265 7472 7920 6f72 206c   e.g. retry or l
-00019e60: 6f67 0a20 2020 2020 2020 2020 2020 2020  og.             
-00019e70: 2020 2020 2020 2070 7269 6e74 3128 6622         print1(f"
-00019e80: 4f70 656e 4149 2041 5049 2072 6574 7572  OpenAI API retur
-00019e90: 6e65 6420 616e 2041 5049 2045 7272 6f72  ned an API Error
-00019ea0: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
-00019eb0: 2020 2020 2020 2020 6578 6365 7074 206f          except o
-00019ec0: 7065 6e61 692e 4150 4943 6f6e 6e65 6374  penai.APIConnect
-00019ed0: 696f 6e45 7272 6f72 2061 7320 653a 0a20  ionError as e:. 
-00019ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ef0: 2020 2073 746f 7053 7069 6e6e 696e 6728     stopSpinning(
-00019f00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00019f10: 2020 2020 2020 2348 616e 646c 6520 636f        #Handle co
-00019f20: 6e6e 6563 7469 6f6e 2065 7272 6f72 2068  nnection error h
-00019f30: 6572 650a 2020 2020 2020 2020 2020 2020  ere.            
-00019f40: 2020 2020 2020 2020 7072 696e 7431 2866          print1(f
-00019f50: 2246 6169 6c65 6420 746f 2063 6f6e 6e65  "Failed to conne
-00019f60: 6374 2074 6f20 4f70 656e 4149 2041 5049  ct to OpenAI API
-00019f70: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
-00019f80: 2020 2020 2020 2020 6578 6365 7074 206f          except o
-00019f90: 7065 6e61 692e 5261 7465 4c69 6d69 7445  penai.RateLimitE
-00019fa0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-00019fb0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019fc0: 746f 7053 7069 6e6e 696e 6728 290a 2020  topSpinning().  
-00019fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fe0: 2020 2348 616e 646c 6520 7261 7465 206c    #Handle rate l
-00019ff0: 696d 6974 2065 7272 6f72 2028 7765 2072  imit error (we r
-0001a000: 6563 6f6d 6d65 6e64 2075 7369 6e67 2065  ecommend using e
-0001a010: 7870 6f6e 656e 7469 616c 2062 6163 6b6f  xponential backo
-0001a020: 6666 290a 2020 2020 2020 2020 2020 2020  ff).            
-0001a030: 2020 2020 2020 2020 7072 696e 7431 2866          print1(f
-0001a040: 224f 7065 6e41 4920 4150 4920 7265 7175  "OpenAI API requ
-0001a050: 6573 7420 6578 6365 6564 6564 2072 6174  est exceeded rat
-0001a060: 6520 6c69 6d69 743a 207b 657d 2229 0a20  e limit: {e}"). 
-0001a070: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001a080: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
-0001a090: 2020 2020 2020 2020 2020 2073 746f 7053             stopS
-0001a0a0: 7069 6e6e 696e 6728 290a 2020 2020 2020  pinning().      
-0001a0b0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0001a0c0: 6163 6520 3d20 7472 6163 6562 6163 6b2e  ace = traceback.
-0001a0d0: 666f 726d 6174 5f65 7863 2829 0a20 2020  format_exc().   
-0001a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0f0: 2069 6620 2250 6c65 6173 6520 7265 6475   if "Please redu
-0001a100: 6365 2074 6865 206c 656e 6774 6820 6f66  ce the length of
-0001a110: 2074 6865 206d 6573 7361 6765 7320 6f72   the messages or
-0001a120: 2063 6f6d 706c 6574 696f 6e22 2069 6e20   completion" in 
-0001a130: 7472 6163 653a 0a20 2020 2020 2020 2020  trace:.         
-0001a140: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001a150: 7269 6e74 3128 224d 6178 696d 756d 2074  rint1("Maximum t
-0001a160: 6f6b 656e 7320 7265 6163 6865 6421 2229  okens reached!")
-0001a170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a180: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
-0001a190: 2e64 6576 656c 6f70 6572 3a0a 2020 2020  .developer:.    
-0001a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1b0: 2020 2020 7072 696e 7431 2873 656c 662e      print1(self.
-0001a1c0: 6469 7669 6465 7229 0a20 2020 2020 2020  divider).       
-0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1e0: 2070 7269 6e74 3128 7472 6163 6529 0a20   print1(trace). 
-0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a200: 2020 2020 2020 2070 7269 6e74 3128 7365         print1(se
-0001a210: 6c66 2e64 6976 6964 6572 290a 2020 2020  lf.divider).    
-0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a230: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001a240: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0001a250: 696e 7431 2822 4572 726f 7220 656e 636f  int1("Error enco
-0001a260: 756e 7465 7265 6421 2229 0a0a 2020 2020  untered!")..    
-0001a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a280: 636f 6e66 6967 2e64 6566 6175 6c74 456e  config.defaultEn
-0001a290: 7472 7920 3d20 7573 6572 496e 7075 740a  try = userInput.
-0001a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2b0: 2020 2020 7072 696e 7431 2822 7374 6172      print1("star
-0001a2c0: 7469 6e67 2061 206e 6577 2063 6861 7421  ting a new chat!
-0001a2d0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0001a2e0: 2020 2020 2020 2073 656c 662e 7361 7665         self.save
-0001a2f0: 4368 6174 2863 6f6e 6669 672e 6375 7272  Chat(config.curr
-0001a300: 656e 744d 6573 7361 6765 7329 0a20 2020  entMessages).   
-0001a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a320: 2073 746f 7261 6765 6469 7265 6374 6f72   storagedirector
-0001a330: 792c 2063 6f6e 6669 672e 6375 7272 656e  y, config.curren
-0001a340: 744d 6573 7361 6765 7320 3d20 7374 6172  tMessages = star
-0001a350: 7443 6861 7428 290a 0a20 2020 2064 6566  tChat()..    def
-0001a360: 206c 6175 6e63 6843 6861 7462 6f74 2873   launchChatbot(s
-0001a370: 656c 662c 2063 6861 7462 6f74 2c20 6669  elf, chatbot, fi
-0001a380: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-0001a390: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
-0001a3a0: 7420 6368 6174 626f 743a 0a20 2020 2020  t chatbot:.     
-0001a3b0: 2020 2020 2020 2063 6861 7462 6f74 203d         chatbot =
-0001a3c0: 2063 6f6e 6669 672e 6c6c 6d49 6e74 6572   config.llmInter
-0001a3d0: 6661 6365 0a20 2020 2020 2020 2069 6620  face.        if 
-0001a3e0: 636f 6e66 6967 2e69 7354 6572 6d75 783a  config.isTermux:
-0001a3f0: 0a20 2020 2020 2020 2020 2020 2023 6368  .            #ch
-0001a400: 6174 626f 7420 3d20 2263 6861 7467 7074  atbot = "chatgpt
-0001a410: 220a 2020 2020 2020 2020 2020 2020 2e2e  ".            ..
-0001a420: 2e0a 2020 2020 2020 2020 6368 6174 626f  ..        chatbo
-0001a430: 7473 203d 207b 0a20 2020 2020 2020 2020  ts = {.         
-0001a440: 2020 2022 6c6c 616d 6163 7070 223a 206c     "llamacpp": l
-0001a450: 616d 6264 613a 204c 6c61 6d61 6370 7043  ambda: LlamacppC
-0001a460: 6861 7428 6d6f 6465 6c3d 4e6f 6e65 2069  hat(model=None i
-0001a470: 6620 636f 6e66 6967 2e75 7365 4164 6469  f config.useAddi
-0001a480: 7469 6f6e 616c 4368 6174 4d6f 6465 6c20  tionalChatModel 
-0001a490: 656c 7365 2063 6f6e 6669 672e 6c6c 616d  else config.llam
-0001a4a0: 6163 7070 4d61 696e 4d6f 6465 6c29 2e72  acppMainModel).r
-0001a4b0: 756e 2866 696e 6554 756e 6564 5573 6572  un(fineTunedUser
-0001a4c0: 496e 7075 7429 2c0a 2020 2020 2020 2020  Input),.        
-0001a4d0: 2020 2020 226f 6c6c 616d 6122 3a20 6c61      "ollama": la
-0001a4e0: 6d62 6461 3a20 4f6c 6c61 6d61 4368 6174  mbda: OllamaChat
-0001a4f0: 2829 2e72 756e 2866 696e 6554 756e 6564  ().run(fineTuned
-0001a500: 5573 6572 496e 7075 742c 206d 6f64 656c  UserInput, model
-0001a510: 3d63 6f6e 6669 672e 6f6c 6c61 6d61 4368  =config.ollamaCh
-0001a520: 6174 4d6f 6465 6c20 6966 2063 6f6e 6669  atModel if confi
-0001a530: 672e 7573 6541 6464 6974 696f 6e61 6c43  g.useAdditionalC
-0001a540: 6861 744d 6f64 656c 2065 6c73 6520 636f  hatModel else co
-0001a550: 6e66 6967 2e6f 6c6c 616d 614d 6169 6e4d  nfig.ollamaMainM
-0001a560: 6f64 656c 292c 0a20 2020 2020 2020 2020  odel),.         
-0001a570: 2020 2022 6772 6f71 223a 206c 616d 6264     "groq": lambd
-0001a580: 613a 2047 726f 7143 6861 7462 6f74 2829  a: GroqChatbot()
-0001a590: 2e72 756e 2866 696e 6554 756e 6564 5573  .run(fineTunedUs
-0001a5a0: 6572 496e 7075 7429 2c0a 2020 2020 2020  erInput),.      
-0001a5b0: 2020 2020 2020 2263 6861 7467 7074 223a        "chatgpt":
-0001a5c0: 206c 616d 6264 613a 2043 6861 7447 5054   lambda: ChatGPT
-0001a5d0: 2829 2e72 756e 2866 696e 6554 756e 6564  ().run(fineTuned
-0001a5e0: 5573 6572 496e 7075 7429 2c0a 2020 2020  UserInput),.    
-0001a5f0: 2020 2020 2020 2020 226c 6574 6d65 646f          "letmedo
-0001a600: 6974 223a 206c 616d 6264 613a 2043 6861  it": lambda: Cha
-0001a610: 7447 5054 2829 2e72 756e 2866 696e 6554  tGPT().run(fineT
-0001a620: 756e 6564 5573 6572 496e 7075 7429 2c0a  unedUserInput),.
-0001a630: 2020 2020 2020 2020 2020 2020 2267 656d              "gem
-0001a640: 696e 6922 3a20 6c61 6d62 6461 3a20 4765  ini": lambda: Ge
-0001a650: 6d69 6e69 5072 6f28 7465 6d70 6572 6174  miniPro(temperat
-0001a660: 7572 653d 636f 6e66 6967 2e6c 6c6d 5465  ure=config.llmTe
-0001a670: 6d70 6572 6174 7572 6529 2e72 756e 2866  mperature).run(f
-0001a680: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-0001a690: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-0001a6a0: 2267 656d 696e 6970 726f 223a 206c 616d  "geminipro": lam
-0001a6b0: 6264 613a 2047 656d 696e 6950 726f 2874  bda: GeminiPro(t
-0001a6c0: 656d 7065 7261 7475 7265 3d63 6f6e 6669  emperature=confi
-0001a6d0: 672e 6c6c 6d54 656d 7065 7261 7475 7265  g.llmTemperature
-0001a6e0: 292e 7275 6e28 6669 6e65 5475 6e65 6455  ).run(fineTunedU
-0001a6f0: 7365 7249 6e70 7574 292c 0a20 2020 2020  serInput),.     
-0001a700: 2020 2020 2020 2022 7061 6c6d 3222 3a20         "palm2": 
-0001a710: 6c61 6d62 6461 3a20 5061 6c6d 3228 292e  lambda: Palm2().
-0001a720: 7275 6e28 6669 6e65 5475 6e65 6455 7365  run(fineTunedUse
-0001a730: 7249 6e70 7574 2c20 7465 6d70 6572 6174  rInput, temperat
-0001a740: 7572 653d 636f 6e66 6967 2e6c 6c6d 5465  ure=config.llmTe
-0001a750: 6d70 6572 6174 7572 6529 2c0a 2020 2020  mperature),.    
-0001a760: 2020 2020 2020 2020 2263 6f64 6579 223a          "codey":
-0001a770: 206c 616d 6264 613a 2043 6f64 6579 2829   lambda: Codey()
-0001a780: 2e72 756e 2866 696e 6554 756e 6564 5573  .run(fineTunedUs
-0001a790: 6572 496e 7075 742c 2074 656d 7065 7261  erInput, tempera
-0001a7a0: 7475 7265 3d63 6f6e 6669 672e 6c6c 6d54  ture=config.llmT
-0001a7b0: 656d 7065 7261 7475 7265 292c 0a20 2020  emperature),.   
-0001a7c0: 2020 2020 207d 0a20 2020 2020 2020 2069       }.        i
-0001a7d0: 6620 6368 6174 626f 7420 696e 2063 6861  f chatbot in cha
-0001a7e0: 7462 6f74 733a 0a20 2020 2020 2020 2020  tbots:.         
-0001a7f0: 2020 2063 6861 7462 6f74 735b 6368 6174     chatbots[chat
-0001a800: 626f 745d 2829 0a0a 2020 2020 6465 6620  bot]()..    def 
-0001a810: 6164 6450 6167 6572 5465 7874 2873 656c  addPagerText(sel
-0001a820: 662c 2074 6578 742c 2077 7261 7057 6f72  f, text, wrapWor
-0001a830: 6473 3d46 616c 7365 293a 0a20 2020 2020  ds=False):.     
-0001a840: 2020 2069 6620 7772 6170 576f 7264 733a     if wrapWords:
-0001a850: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-0001a860: 7420 3d20 7365 6c66 2e67 6574 5772 6170  t = self.getWrap
-0001a870: 7065 6448 544d 4c54 6578 7428 7465 7874  pedHTMLText(text
-0001a880: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
-0001a890: 2e70 6167 6572 436f 6e74 656e 7420 2b3d  .pagerContent +=
-0001a8a0: 2066 227b 7465 7874 7d5c 6e22 0a0a 2020   f"{text}\n"..  
-0001a8b0: 2020 6465 6620 6c61 756e 6368 5061 6765    def launchPage
-0001a8c0: 7228 7365 6c66 2c20 7061 6765 7243 6f6e  r(self, pagerCon
-0001a8d0: 7465 6e74 3d4e 6f6e 6529 3a0a 2020 2020  tent=None):.    
-0001a8e0: 2020 2020 6966 2070 6167 6572 436f 6e74      if pagerCont
-0001a8f0: 656e 7420 6973 204e 6f6e 653a 0a20 2020  ent is None:.   
-0001a900: 2020 2020 2020 2020 2070 6167 6572 436f           pagerCo
-0001a910: 6e74 656e 7420 3d20 636f 6e66 6967 2e70  ntent = config.p
-0001a920: 6167 6572 436f 6e74 656e 740a 2020 2020  agerContent.    
-0001a930: 2020 2020 6966 2070 6167 6572 436f 6e74      if pagerCont
-0001a940: 656e 743a 0a20 2020 2020 2020 2020 2020  ent:.           
-0001a950: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0001a960: 2020 2020 2020 6966 2073 6875 7469 6c2e        if shutil.
-0001a970: 7768 6963 6828 2262 6174 2229 3a0a 2020  which("bat"):.  
-0001a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a990: 2020 2320 5769 6e64 6f77 7320 7573 6572    # Windows user
-0001a9a0: 7320 6361 6e20 696e 7374 616c 6c20 6261  s can install ba
-0001a9b0: 7420 636f 6d6d 616e 6420 7769 7468 2073  t command with s
-0001a9c0: 636f 6f70 0a20 2020 2020 2020 2020 2020  coop.           
-0001a9d0: 2020 2020 2020 2020 2023 2072 6561 643a           # read:
-0001a9e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-0001a9f0: 636f 6d2f 5363 6f6f 7049 6e73 7461 6c6c  com/ScoopInstall
-0001aa00: 6572 2f53 636f 6f70 0a20 2020 2020 2020  er/Scoop.       
-0001aa10: 2020 2020 2020 2020 2020 2020 2023 203e               # >
-0001aa20: 2069 7772 202d 7573 6562 2067 6574 2e73   iwr -useb get.s
-0001aa30: 636f 6f70 2e73 6820 7c20 6965 780a 2020  coop.sh | iex.  
-0001aa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa50: 2020 2320 3e20 7363 6f6f 7020 696e 7374    # > scoop inst
-0001aa60: 616c 6c20 6172 6961 3220 6261 740a 2020  all aria2 bat.  
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa80: 2020 6966 2072 652e 7365 6172 6368 2822    if re.search("
-0001aa90: 3c5b 5e3c 3e5d 2b3f 3e22 2c20 7061 6765  <[^<>]+?>", page
-0001aaa0: 7243 6f6e 7465 6e74 293a 0a20 2020 2020  rContent):.     
-0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 2070 6167 6572 436f 6e74 656e 7420     pagerContent 
-0001aad0: 3d20 5465 7874 5574 696c 2e63 6f6e 7665  = TextUtil.conve
-0001aae0: 7274 4874 6d6c 5461 6754 6f43 6f6c 6f72  rtHtmlTagToColor
-0001aaf0: 616d 6128 7061 6765 7243 6f6e 7465 6e74  ama(pagerContent
-0001ab00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001ab10: 2020 2020 2020 6c61 6e67 7561 6765 203d        language =
-0001ab20: 2022 5079 7468 6f6e 2220 6966 2022 6060   "Python" if "``
-0001ab30: 6070 7974 686f 6e22 2069 6e20 7061 6765  `python" in page
-0001ab40: 7243 6f6e 7465 6e74 2065 6c73 6520 224d  rContent else "M
-0001ab50: 6172 6b64 6f77 6e22 0a20 2020 2020 2020  arkdown".       
-0001ab60: 2020 2020 2020 2020 2020 2020 2070 7964               pyd
-0001ab70: 6f63 2e70 6970 6570 6167 6572 2870 6167  oc.pipepager(pag
-0001ab80: 6572 436f 6e74 656e 742c 2063 6d64 3d66  erContent, cmd=f
-0001ab90: 2262 6174 202d 6c20 7b6c 616e 6775 6167  "bat -l {languag
-0001aba0: 657d 202d 2d70 6167 696e 6720 616c 7761  e} --paging alwa
-0001abb0: 7973 2229 0a20 2020 2020 2020 2020 2020  ys").           
-0001abc0: 2020 2020 2065 6c69 6620 7368 7574 696c       elif shutil
-0001abd0: 2e77 6869 6368 2822 6c65 7373 2229 3a0a  .which("less"):.
-0001abe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abf0: 2020 2020 2320 5769 6e64 6f77 7320 7573      # Windows us
-0001ac00: 6572 7320 6361 6e20 696e 7374 616c 6c20  ers can install 
-0001ac10: 6c65 7373 2063 6f6d 6d61 6e64 2077 6974  less command wit
-0001ac20: 6820 7363 6f6f 700a 2020 2020 2020 2020  h scoop.        
-0001ac30: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-0001ac40: 6164 3a20 6874 7470 733a 2f2f 6769 7468  ad: https://gith
-0001ac50: 7562 2e63 6f6d 2f53 636f 6f70 496e 7374  ub.com/ScoopInst
-0001ac60: 616c 6c65 722f 5363 6f6f 700a 2020 2020  aller/Scoop.    
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac80: 2320 3e20 6977 7220 2d75 7365 6220 6765  # > iwr -useb ge
-0001ac90: 742e 7363 6f6f 702e 7368 207c 2069 6578  t.scoop.sh | iex
-0001aca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001acb0: 2020 2020 2023 203e 2073 636f 6f70 2069       # > scoop i
-0001acc0: 6e73 7461 6c6c 2061 7269 6132 206c 6573  nstall aria2 les
-0001acd0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0001ace0: 2020 2020 2020 6966 2072 652e 7365 6172        if re.sear
-0001acf0: 6368 2822 3c5b 5e3c 3e5d 2b3f 3e22 2c20  ch("<[^<>]+?>", 
-0001ad00: 7061 6765 7243 6f6e 7465 6e74 293a 0a20  pagerContent):. 
-0001ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad20: 2020 2020 2020 2070 6167 6572 436f 6e74         pagerCont
-0001ad30: 656e 7420 3d20 5465 7874 5574 696c 2e63  ent = TextUtil.c
-0001ad40: 6f6e 7665 7274 4874 6d6c 5461 6754 6f43  onvertHtmlTagToC
-0001ad50: 6f6c 6f72 616d 6128 7061 6765 7243 6f6e  olorama(pagerCon
-0001ad60: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
-0001ad70: 2020 2020 2020 2020 2020 7079 646f 632e            pydoc.
-0001ad80: 7069 7065 7061 6765 7228 7061 6765 7243  pipepager(pagerC
-0001ad90: 6f6e 7465 6e74 2c20 636d 643d 276c 6573  ontent, cmd='les
-0001ada0: 7320 2d52 2729 0a20 2020 2020 2020 2020  s -R').         
-0001adb0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001add0: 2070 7964 6f63 2e70 6167 6572 2870 6167   pydoc.pager(pag
-0001ade0: 6572 436f 6e74 656e 7429 0a20 2020 2020  erContent).     
-0001adf0: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-0001ae00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001ae10: 6f6e 6669 672e 7061 6765 7256 6965 7720  onfig.pagerView 
-0001ae20: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
-0001ae30: 2020 2020 2020 2020 7368 6f77 4572 726f          showErro
-0001ae40: 7273 2829 0a0a 2020 2020 2320 7772 6170  rs()..    # wrap
-0001ae50: 2068 746d 6c20 7465 7874 2061 7420 7370   html text at sp
-0001ae60: 6163 6573 0a20 2020 2064 6566 2067 6574  aces.    def get
-0001ae70: 5772 6170 7065 6448 544d 4c54 6578 7428  WrappedHTMLText(
-0001ae80: 7365 6c66 2c20 7465 7874 2c20 7465 726d  self, text, term
-0001ae90: 696e 616c 5f77 6964 7468 3d4e 6f6e 6529  inal_width=None)
-0001aea0: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-0001aeb0: 2022 2022 2069 6e20 7465 7874 3a0a 2020   " " in text:.  
-0001aec0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001aed0: 2074 6578 740a 2020 2020 2020 2020 6966   text.        if
-0001aee0: 2074 6572 6d69 6e61 6c5f 7769 6474 6820   terminal_width 
-0001aef0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0001af00: 2020 2020 2074 6572 6d69 6e61 6c5f 7769       terminal_wi
-0001af10: 6474 6820 3d20 7368 7574 696c 2e67 6574  dth = shutil.get
-0001af20: 5f74 6572 6d69 6e61 6c5f 7369 7a65 2829  _terminal_size()
-0001af30: 2e63 6f6c 756d 6e73 0a20 2020 2020 2020  .columns.       
-0001af40: 2073 656c 662e 7772 6170 7065 6454 6578   self.wrappedTex
-0001af50: 7420 3d20 2222 0a20 2020 2020 2020 2073  t = "".        s
-0001af60: 656c 662e 6c69 6e65 5769 6474 6820 3d20  elf.lineWidth = 
-0001af70: 300a 0a20 2020 2020 2020 2064 6566 2061  0..        def a
-0001af80: 6464 576f 7264 7328 776f 7264 7329 3a0a  ddWords(words):.
-0001af90: 2020 2020 2020 2020 2020 2020 776f 7264              word
-0001afa0: 7320 3d20 776f 7264 732e 7370 6c69 7428  s = words.split(
-0001afb0: 2220 2229 0a20 2020 2020 2020 2020 2020  " ").           
-0001afc0: 2066 6f72 2069 6e64 6578 2c20 6974 656d   for index, item
-0001afd0: 2069 6e20 656e 756d 6572 6174 6528 776f   in enumerate(wo
-0001afe0: 7264 7329 3a0a 2020 2020 2020 2020 2020  rds):.          
-0001aff0: 2020 2020 2020 6973 4c61 7374 4974 656d        isLastItem
-0001b000: 203d 2028 6c65 6e28 776f 7264 7329 202d   = (len(words) -
-0001b010: 2069 6e64 6578 203d 3d20 3129 0a20 2020   index == 1).   
-0001b020: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001b030: 6973 5f43 4a4b 2869 7465 6d29 3a0a 2020  is_CJK(item):.  
-0001b040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b050: 2020 666f 7220 6949 6e64 6578 2c20 6920    for iIndex, i 
-0001b060: 696e 2065 6e75 6d65 7261 7465 2869 7465  in enumerate(ite
-0001b070: 6d29 3a0a 2020 2020 2020 2020 2020 2020  m):.            
-0001b080: 2020 2020 2020 2020 2020 2020 6973 5370              isSp
-0001b090: 6163 6549 7465 6d20 3d20 286e 6f74 2069  aceItem = (not i
-0001b0a0: 734c 6173 7449 7465 6d20 616e 6420 286c  sLastItem and (l
-0001b0b0: 656e 2869 7465 6d29 202d 2069 496e 6465  en(item) - iInde
-0001b0c0: 7820 3d3d 2031 2929 0a20 2020 2020 2020  x == 1)).       
-0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0e0: 2069 5769 6474 6820 3d20 6765 7453 7472   iWidth = getStr
-0001b0f0: 696e 6757 6964 7468 2869 290a 2020 2020  ingWidth(i).    
-0001b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b110: 2020 2020 6966 2069 7353 7061 6365 4974      if isSpaceIt
-0001b120: 656d 3a0a 2020 2020 2020 2020 2020 2020  em:.            
-0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b140: 6e65 774c 696e 6557 6964 7468 203d 2073  newLineWidth = s
-0001b150: 656c 662e 6c69 6e65 5769 6474 6820 2b20  elf.lineWidth + 
-0001b160: 6957 6964 7468 202b 2031 0a20 2020 2020  iWidth + 1.     
-0001b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b180: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1a0: 2020 2020 206e 6577 4c69 6e65 5769 6474       newLineWidt
-0001b1b0: 6820 3d20 7365 6c66 2e6c 696e 6557 6964  h = self.lineWid
-0001b1c0: 7468 202b 2069 5769 6474 680a 2020 2020  th + iWidth.    
-0001b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b1e0: 2020 2020 6966 206e 6577 4c69 6e65 5769      if newLineWi
-0001b1f0: 6474 6820 3e20 7465 726d 696e 616c 5f77  dth > terminal_w
-0001b200: 6964 7468 3a0a 2020 2020 2020 2020 2020  idth:.          
-0001b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b220: 2020 7365 6c66 2e77 7261 7070 6564 5465    self.wrappedTe
-0001b230: 7874 202b 3d20 6622 5c6e 7b69 7d20 2220  xt += f"\n{i} " 
-0001b240: 6966 2069 7353 7061 6365 4974 656d 2065  if isSpaceItem e
-0001b250: 6c73 6520 6622 5c6e 7b69 7d22 0a20 2020  lse f"\n{i}".   
-0001b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b270: 2020 2020 2020 2020 2073 656c 662e 6c69           self.li
-0001b280: 6e65 5769 6474 6820 3d20 6957 6964 7468  neWidth = iWidth
-0001b290: 202b 2031 2069 6620 6973 5370 6163 6549   + 1 if isSpaceI
-0001b2a0: 7465 6d20 656c 7365 2069 5769 6474 680a  tem else iWidth.
-0001b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00019890: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 2020 2020 7072 696e 7431 2822 556e 6162      print1("Unab
+000198c0: 6c65 2074 6f20 6c6f 6164 2069 6e74 6572  le to load inter
+000198d0: 6e65 7420 7265 736f 7572 6365 732e 2229  net resources.")
+000198e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000198f0: 2020 2020 2020 2020 2020 2020 2073 686f               sho
+00019900: 7745 7272 6f72 7328 290a 0a20 2020 2020  wErrors()..     
+00019910: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019920: 6f6d 706c 6574 696f 6e20 3d20 4361 6c6c  ompletion = Call
+00019930: 4c4c 4d2e 7275 6e47 656e 6975 7343 616c  LLM.runGeniusCal
+00019940: 6c28 636f 6e66 6967 2e63 7572 7265 6e74  l(config.current
+00019950: 4d65 7373 6167 6573 2c20 6e6f 4675 6e63  Messages, noFunc
+00019960: 7469 6f6e 4361 6c6c 290a 2020 2020 2020  tionCall).      
+00019970: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019990: 2020 2023 2073 746f 7020 7370 696e 6e69     # stop spinni
+000199a0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+000199b0: 2020 2020 2020 2063 6f6e 6669 672e 7275         config.ru
+000199c0: 6e50 7974 686f 6e20 3d20 5472 7565 0a20  nPython = True. 
+000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199e0: 2020 2073 746f 7053 7069 6e6e 696e 6728     stopSpinning(
+000199f0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00019a00: 2020 2020 2020 2069 6620 636f 6d70 6c65         if comple
+00019a10: 7469 6f6e 2069 7320 6e6f 7420 4e6f 6e65  tion is not None
+00019a20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00019a30: 2020 2020 2020 2020 2020 2320 4372 6561            # Crea
+00019a40: 7465 2061 206e 6577 2074 6872 6561 6420  te a new thread 
+00019a50: 666f 7220 7468 6520 7374 7265 616d 696e  for the streamin
+00019a60: 6720 7461 736b 0a20 2020 2020 2020 2020  g task.         
+00019a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019a80: 7472 6561 6d69 6e67 576f 7264 5772 6170  treamingWordWrap
+00019a90: 7065 7220 3d20 5374 7265 616d 696e 6757  per = StreamingW
+00019aa0: 6f72 6457 7261 7070 6572 2829 0a20 2020  ordWrapper().   
+00019ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ac0: 2020 2020 2073 7472 6561 6d69 6e67 5f65       streaming_e
+00019ad0: 7665 6e74 203d 2074 6872 6561 6469 6e67  vent = threading
+00019ae0: 2e45 7665 6e74 2829 0a20 2020 2020 2020  .Event().       
+00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b00: 2073 656c 662e 7374 7265 616d 696e 675f   self.streaming_
+00019b10: 7468 7265 6164 203d 2074 6872 6561 6469  thread = threadi
+00019b20: 6e67 2e54 6872 6561 6428 7461 7267 6574  ng.Thread(target
+00019b30: 3d73 7472 6561 6d69 6e67 576f 7264 5772  =streamingWordWr
+00019b40: 6170 7065 722e 7374 7265 616d 4f75 7470  apper.streamOutp
+00019b50: 7574 732c 2061 7267 733d 2873 7472 6561  uts, args=(strea
+00019b60: 6d69 6e67 5f65 7665 6e74 2c20 636f 6d70  ming_event, comp
+00019b70: 6c65 7469 6f6e 2c20 5472 7565 2069 6620  letion, True if 
+00019b80: 636f 6e66 6967 2e6c 6c6d 496e 7465 7266  config.llmInterf
+00019b90: 6163 6520 696e 2028 2263 6861 7467 7074  ace in ("chatgpt
+00019ba0: 222c 2022 6c65 746d 6564 6f69 7422 2c20  ", "letmedoit", 
+00019bb0: 2267 726f 7122 2920 656c 7365 2046 616c  "groq") else Fal
+00019bc0: 7365 2929 0a20 2020 2020 2020 2020 2020  se)).           
+00019bd0: 2020 2020 2020 2020 2020 2020 2023 2053               # S
+00019be0: 7461 7274 2074 6865 2073 7472 6561 6d69  tart the streami
+00019bf0: 6e67 2074 6872 6561 640a 2020 2020 2020  ng thread.      
+00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c10: 2020 7365 6c66 2e73 7472 6561 6d69 6e67    self.streaming
+00019c20: 5f74 6872 6561 642e 7374 6172 7428 290a  _thread.start().
+00019c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019c40: 2020 2020 2020 2020 2023 2077 6169 7420           # wait 
+00019c50: 7768 696c 6520 7465 7874 206f 7574 7075  while text outpu
+00019c60: 7420 6973 2073 7465 616d 696e 673b 2063  t is steaming; c
+00019c70: 6170 7475 7265 206b 6579 2063 6f6d 626f  apture key combo
+00019c80: 2027 6374 726c 2b71 2720 6f72 2027 6374   'ctrl+q' or 'ct
+00019c90: 726c 2b7a 2720 746f 2073 746f 7020 7468  rl+z' to stop th
+00019ca0: 6520 7374 7265 616d 696e 670a 2020 2020  e streaming.    
+00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019cc0: 2020 2020 7374 7265 616d 696e 6757 6f72      streamingWor
+00019cd0: 6457 7261 7070 6572 2e6b 6579 546f 5374  dWrapper.keyToSt
+00019ce0: 6f70 5374 7265 616d 696e 6728 7374 7265  opStreaming(stre
+00019cf0: 616d 696e 675f 6576 656e 7429 0a0a 2020  aming_event)..  
+00019d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d10: 2020 2020 2020 2320 7768 656e 2073 7472        # when str
+00019d20: 6561 6d69 6e67 2069 7320 646f 6e65 206f  eaming is done o
+00019d30: 7220 7768 656e 2075 7365 7220 7072 6573  r when user pres
+00019d40: 7320 2263 7472 6c2b 7122 0a20 2020 2020  s "ctrl+q".     
+00019d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d60: 2020 2073 656c 662e 7374 7265 616d 696e     self.streamin
+00019d70: 675f 7468 7265 6164 2e6a 6f69 6e28 290a  g_thread.join().
+00019d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019d90: 2023 2065 7272 6f72 2063 6f64 6573 3a20   # error codes: 
+00019da0: 6874 7470 733a 2f2f 706c 6174 666f 726d  https://platform
+00019db0: 2e6f 7065 6e61 692e 636f 6d2f 646f 6373  .openai.com/docs
+00019dc0: 2f67 7569 6465 732f 6572 726f 722d 636f  /guides/error-co
+00019dd0: 6465 732f 7079 7468 6f6e 2d6c 6962 7261  des/python-libra
+00019de0: 7279 2d65 7272 6f72 2d74 7970 6573 0a20  ry-error-types. 
+00019df0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00019e00: 7863 6570 7420 6f70 656e 6169 2e41 5049  xcept openai.API
+00019e10: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e30: 7374 6f70 5370 696e 6e69 6e67 2829 0a20  stopSpinning(). 
+00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e50: 2020 2023 4861 6e64 6c65 2041 5049 2065     #Handle API e
+00019e60: 7272 6f72 2068 6572 652c 2065 2e67 2e20  rror here, e.g. 
+00019e70: 7265 7472 7920 6f72 206c 6f67 0a20 2020  retry or log.   
+00019e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e90: 2070 7269 6e74 3128 6622 4f70 656e 4149   print1(f"OpenAI
+00019ea0: 2041 5049 2072 6574 7572 6e65 6420 616e   API returned an
+00019eb0: 2041 5049 2045 7272 6f72 3a20 7b65 7d22   API Error: {e}"
+00019ec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019ed0: 2020 6578 6365 7074 206f 7065 6e61 692e    except openai.
+00019ee0: 4150 4943 6f6e 6e65 6374 696f 6e45 7272  APIConnectionErr
+00019ef0: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+00019f00: 2020 2020 2020 2020 2020 2020 2073 746f               sto
+00019f10: 7053 7069 6e6e 696e 6728 290a 2020 2020  pSpinning().    
+00019f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f30: 2348 616e 646c 6520 636f 6e6e 6563 7469  #Handle connecti
+00019f40: 6f6e 2065 7272 6f72 2068 6572 650a 2020  on error here.  
+00019f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f60: 2020 7072 696e 7431 2866 2246 6169 6c65    print1(f"Faile
+00019f70: 6420 746f 2063 6f6e 6e65 6374 2074 6f20  d to connect to 
+00019f80: 4f70 656e 4149 2041 5049 3a20 7b65 7d22  OpenAI API: {e}"
+00019f90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00019fa0: 2020 6578 6365 7074 206f 7065 6e61 692e    except openai.
+00019fb0: 5261 7465 4c69 6d69 7445 7272 6f72 2061  RateLimitError a
+00019fc0: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00019fd0: 2020 2020 2020 2020 2073 746f 7053 7069           stopSpi
+00019fe0: 6e6e 696e 6728 290a 2020 2020 2020 2020  nning().        
+00019ff0: 2020 2020 2020 2020 2020 2020 2348 616e              #Han
+0001a000: 646c 6520 7261 7465 206c 696d 6974 2065  dle rate limit e
+0001a010: 7272 6f72 2028 7765 2072 6563 6f6d 6d65  rror (we recomme
+0001a020: 6e64 2075 7369 6e67 2065 7870 6f6e 656e  nd using exponen
+0001a030: 7469 616c 2062 6163 6b6f 6666 290a 2020  tial backoff).  
+0001a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a050: 2020 7072 696e 7431 2866 224f 7065 6e41    print1(f"OpenA
+0001a060: 4920 4150 4920 7265 7175 6573 7420 6578  I API request ex
+0001a070: 6365 6564 6564 2072 6174 6520 6c69 6d69  ceeded rate limi
+0001a080: 743a 207b 657d 2229 0a20 2020 2020 2020  t: {e}").       
+0001a090: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+0001a0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a0b0: 2020 2020 2073 746f 7053 7069 6e6e 696e       stopSpinnin
+0001a0c0: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+0001a0d0: 2020 2020 2020 2020 7472 6163 6520 3d20          trace = 
+0001a0e0: 7472 6163 6562 6163 6b2e 666f 726d 6174  traceback.format
+0001a0f0: 5f65 7863 2829 0a20 2020 2020 2020 2020  _exc().         
+0001a100: 2020 2020 2020 2020 2020 2069 6620 2250             if "P
+0001a110: 6c65 6173 6520 7265 6475 6365 2074 6865  lease reduce the
+0001a120: 206c 656e 6774 6820 6f66 2074 6865 206d   length of the m
+0001a130: 6573 7361 6765 7320 6f72 2063 6f6d 706c  essages or compl
+0001a140: 6574 696f 6e22 2069 6e20 7472 6163 653a  etion" in trace:
+0001a150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a160: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
+0001a170: 224d 6178 696d 756d 2074 6f6b 656e 7320  "Maximum tokens 
+0001a180: 7265 6163 6865 6421 2229 0a20 2020 2020  reached!").     
+0001a190: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001a1a0: 6c69 6620 636f 6e66 6967 2e64 6576 656c  lif config.devel
+0001a1b0: 6f70 6572 3a0a 2020 2020 2020 2020 2020  oper:.          
+0001a1c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0001a1d0: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
+0001a1e0: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+0001a1f0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0001a200: 3128 7472 6163 6529 0a20 2020 2020 2020  1(trace).       
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a220: 2070 7269 6e74 3128 7365 6c66 2e64 6976   print1(self.div
+0001a230: 6964 6572 290a 2020 2020 2020 2020 2020  ider).          
+0001a240: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a260: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+0001a270: 4572 726f 7220 656e 636f 756e 7465 7265  Error encountere
+0001a280: 6421 2229 0a0a 2020 2020 2020 2020 2020  d!")..          
+0001a290: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0001a2a0: 2e64 6566 6175 6c74 456e 7472 7920 3d20  .defaultEntry = 
+0001a2b0: 7573 6572 496e 7075 740a 2020 2020 2020  userInput.      
+0001a2c0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0001a2d0: 696e 7431 2822 7374 6172 7469 6e67 2061  int1("starting a
+0001a2e0: 206e 6577 2063 6861 7421 2229 0a20 2020   new chat!").   
+0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a300: 2073 656c 662e 7361 7665 4368 6174 2863   self.saveChat(c
+0001a310: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
+0001a320: 7361 6765 7329 0a20 2020 2020 2020 2020  sages).         
+0001a330: 2020 2020 2020 2020 2020 2073 746f 7261             stora
+0001a340: 6765 6469 7265 6374 6f72 792c 2063 6f6e  gedirectory, con
+0001a350: 6669 672e 6375 7272 656e 744d 6573 7361  fig.currentMessa
+0001a360: 6765 7320 3d20 7374 6172 7443 6861 7428  ges = startChat(
+0001a370: 290a 0a20 2020 2064 6566 206c 6175 6e63  )..    def launc
+0001a380: 6843 6861 7462 6f74 2873 656c 662c 2063  hChatbot(self, c
+0001a390: 6861 7462 6f74 2c20 6669 6e65 5475 6e65  hatbot, fineTune
+0001a3a0: 6455 7365 7249 6e70 7574 293a 0a20 2020  dUserInput):.   
+0001a3b0: 2020 2020 2069 6620 6e6f 7420 6368 6174       if not chat
+0001a3c0: 626f 743a 0a20 2020 2020 2020 2020 2020  bot:.           
+0001a3d0: 2063 6861 7462 6f74 203d 2063 6f6e 6669   chatbot = confi
+0001a3e0: 672e 6c6c 6d49 6e74 6572 6661 6365 0a20  g.llmInterface. 
+0001a3f0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+0001a400: 2e69 7354 6572 6d75 783a 0a20 2020 2020  .isTermux:.     
+0001a410: 2020 2020 2020 2023 6368 6174 626f 7420         #chatbot 
+0001a420: 3d20 2263 6861 7467 7074 220a 2020 2020  = "chatgpt".    
+0001a430: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+0001a440: 2020 2020 6368 6174 626f 7473 203d 207b      chatbots = {
+0001a450: 0a20 2020 2020 2020 2020 2020 2022 6c6c  .            "ll
+0001a460: 616d 6163 7070 223a 206c 616d 6264 613a  amacpp": lambda:
+0001a470: 204c 6c61 6d61 6370 7043 6861 7428 6d6f   LlamacppChat(mo
+0001a480: 6465 6c3d 4e6f 6e65 2069 6620 636f 6e66  del=None if conf
+0001a490: 6967 2e75 7365 4164 6469 7469 6f6e 616c  ig.useAdditional
+0001a4a0: 4368 6174 4d6f 6465 6c20 656c 7365 2063  ChatModel else c
+0001a4b0: 6f6e 6669 672e 6c6c 616d 6163 7070 4d61  onfig.llamacppMa
+0001a4c0: 696e 4d6f 6465 6c29 2e72 756e 2866 696e  inModel).run(fin
+0001a4d0: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
+0001a4e0: 2c0a 2020 2020 2020 2020 2020 2020 226f  ,.            "o
+0001a4f0: 6c6c 616d 6122 3a20 6c61 6d62 6461 3a20  llama": lambda: 
+0001a500: 4f6c 6c61 6d61 4368 6174 2829 2e72 756e  OllamaChat().run
+0001a510: 2866 696e 6554 756e 6564 5573 6572 496e  (fineTunedUserIn
+0001a520: 7075 742c 206d 6f64 656c 3d63 6f6e 6669  put, model=confi
+0001a530: 672e 6f6c 6c61 6d61 4368 6174 4d6f 6465  g.ollamaChatMode
+0001a540: 6c20 6966 2063 6f6e 6669 672e 7573 6541  l if config.useA
+0001a550: 6464 6974 696f 6e61 6c43 6861 744d 6f64  dditionalChatMod
+0001a560: 656c 2065 6c73 6520 636f 6e66 6967 2e6f  el else config.o
+0001a570: 6c6c 616d 614d 6169 6e4d 6f64 656c 292c  llamaMainModel),
+0001a580: 0a20 2020 2020 2020 2020 2020 2022 6772  .            "gr
+0001a590: 6f71 223a 206c 616d 6264 613a 2047 726f  oq": lambda: Gro
+0001a5a0: 7143 6861 7462 6f74 2829 2e72 756e 2866  qChatbot().run(f
+0001a5b0: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+0001a5c0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
+0001a5d0: 2263 6861 7467 7074 223a 206c 616d 6264  "chatgpt": lambd
+0001a5e0: 613a 2043 6861 7447 5054 2829 2e72 756e  a: ChatGPT().run
+0001a5f0: 2866 696e 6554 756e 6564 5573 6572 496e  (fineTunedUserIn
+0001a600: 7075 7429 2c0a 2020 2020 2020 2020 2020  put),.          
+0001a610: 2020 226c 6574 6d65 646f 6974 223a 206c    "letmedoit": l
+0001a620: 616d 6264 613a 2043 6861 7447 5054 2829  ambda: ChatGPT()
+0001a630: 2e72 756e 2866 696e 6554 756e 6564 5573  .run(fineTunedUs
+0001a640: 6572 496e 7075 7429 2c0a 2020 2020 2020  erInput),.      
+0001a650: 2020 2020 2020 2267 656d 696e 6922 3a20        "gemini": 
+0001a660: 6c61 6d62 6461 3a20 4765 6d69 6e69 5072  lambda: GeminiPr
+0001a670: 6f28 7465 6d70 6572 6174 7572 653d 636f  o(temperature=co
+0001a680: 6e66 6967 2e6c 6c6d 5465 6d70 6572 6174  nfig.llmTemperat
+0001a690: 7572 6529 2e72 756e 2866 696e 6554 756e  ure).run(fineTun
+0001a6a0: 6564 5573 6572 496e 7075 7429 2c0a 2020  edUserInput),.  
+0001a6b0: 2020 2020 2020 2020 2020 2267 656d 696e            "gemin
+0001a6c0: 6970 726f 223a 206c 616d 6264 613a 2047  ipro": lambda: G
+0001a6d0: 656d 696e 6950 726f 2874 656d 7065 7261  eminiPro(tempera
+0001a6e0: 7475 7265 3d63 6f6e 6669 672e 6c6c 6d54  ture=config.llmT
+0001a6f0: 656d 7065 7261 7475 7265 292e 7275 6e28  emperature).run(
+0001a700: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
+0001a710: 7574 292c 0a20 2020 2020 2020 2020 2020  ut),.           
+0001a720: 2022 7061 6c6d 3222 3a20 6c61 6d62 6461   "palm2": lambda
+0001a730: 3a20 5061 6c6d 3228 292e 7275 6e28 6669  : Palm2().run(fi
+0001a740: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
+0001a750: 2c20 7465 6d70 6572 6174 7572 653d 636f  , temperature=co
+0001a760: 6e66 6967 2e6c 6c6d 5465 6d70 6572 6174  nfig.llmTemperat
+0001a770: 7572 6529 2c0a 2020 2020 2020 2020 2020  ure),.          
+0001a780: 2020 2263 6f64 6579 223a 206c 616d 6264    "codey": lambd
+0001a790: 613a 2043 6f64 6579 2829 2e72 756e 2866  a: Codey().run(f
+0001a7a0: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+0001a7b0: 742c 2074 656d 7065 7261 7475 7265 3d63  t, temperature=c
+0001a7c0: 6f6e 6669 672e 6c6c 6d54 656d 7065 7261  onfig.llmTempera
+0001a7d0: 7475 7265 292c 0a20 2020 2020 2020 207d  ture),.        }
+0001a7e0: 0a20 2020 2020 2020 2069 6620 6368 6174  .        if chat
+0001a7f0: 626f 7420 696e 2063 6861 7462 6f74 733a  bot in chatbots:
+0001a800: 0a20 2020 2020 2020 2020 2020 2063 6861  .            cha
+0001a810: 7462 6f74 735b 6368 6174 626f 745d 2829  tbots[chatbot]()
+0001a820: 0a0a 2020 2020 6465 6620 6164 6450 6167  ..    def addPag
+0001a830: 6572 5465 7874 2873 656c 662c 2074 6578  erText(self, tex
+0001a840: 742c 2077 7261 7057 6f72 6473 3d46 616c  t, wrapWords=Fal
+0001a850: 7365 293a 0a20 2020 2020 2020 2069 6620  se):.        if 
+0001a860: 7772 6170 576f 7264 733a 0a20 2020 2020  wrapWords:.     
+0001a870: 2020 2020 2020 2074 6578 7420 3d20 7365         text = se
+0001a880: 6c66 2e67 6574 5772 6170 7065 6448 544d  lf.getWrappedHTM
+0001a890: 4c54 6578 7428 7465 7874 290a 2020 2020  LText(text).    
+0001a8a0: 2020 2020 636f 6e66 6967 2e70 6167 6572      config.pager
+0001a8b0: 436f 6e74 656e 7420 2b3d 2066 227b 7465  Content += f"{te
+0001a8c0: 7874 7d5c 6e22 0a0a 2020 2020 6465 6620  xt}\n"..    def 
+0001a8d0: 6c61 756e 6368 5061 6765 7228 7365 6c66  launchPager(self
+0001a8e0: 2c20 7061 6765 7243 6f6e 7465 6e74 3d4e  , pagerContent=N
+0001a8f0: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
+0001a900: 2070 6167 6572 436f 6e74 656e 7420 6973   pagerContent is
+0001a910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001a920: 2020 2070 6167 6572 436f 6e74 656e 7420     pagerContent 
+0001a930: 3d20 636f 6e66 6967 2e70 6167 6572 436f  = config.pagerCo
+0001a940: 6e74 656e 740a 2020 2020 2020 2020 6966  ntent.        if
+0001a950: 2070 6167 6572 436f 6e74 656e 743a 0a20   pagerContent:. 
+0001a960: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0001a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a980: 6966 2073 6875 7469 6c2e 7768 6963 6828  if shutil.which(
+0001a990: 2262 6174 2229 3a0a 2020 2020 2020 2020  "bat"):.        
+0001a9a0: 2020 2020 2020 2020 2020 2020 2320 5769              # Wi
+0001a9b0: 6e64 6f77 7320 7573 6572 7320 6361 6e20  ndows users can 
+0001a9c0: 696e 7374 616c 6c20 6261 7420 636f 6d6d  install bat comm
+0001a9d0: 616e 6420 7769 7468 2073 636f 6f70 0a20  and with scoop. 
+0001a9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a9f0: 2020 2023 2072 6561 643a 2068 7474 7073     # read: https
+0001aa00: 3a2f 2f67 6974 6875 622e 636f 6d2f 5363  ://github.com/Sc
+0001aa10: 6f6f 7049 6e73 7461 6c6c 6572 2f53 636f  oopInstaller/Sco
+0001aa20: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
+0001aa30: 2020 2020 2020 2023 203e 2069 7772 202d         # > iwr -
+0001aa40: 7573 6562 2067 6574 2e73 636f 6f70 2e73  useb get.scoop.s
+0001aa50: 6820 7c20 6965 780a 2020 2020 2020 2020  h | iex.        
+0001aa60: 2020 2020 2020 2020 2020 2020 2320 3e20              # > 
+0001aa70: 7363 6f6f 7020 696e 7374 616c 6c20 6172  scoop install ar
+0001aa80: 6961 3220 6261 740a 2020 2020 2020 2020  ia2 bat.        
+0001aa90: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0001aaa0: 652e 7365 6172 6368 2822 3c5b 5e3c 3e5d  e.search("<[^<>]
+0001aab0: 2b3f 3e22 2c20 7061 6765 7243 6f6e 7465  +?>", pagerConte
+0001aac0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+0001aad0: 2020 2020 2020 2020 2020 2020 2070 6167               pag
+0001aae0: 6572 436f 6e74 656e 7420 3d20 5465 7874  erContent = Text
+0001aaf0: 5574 696c 2e63 6f6e 7665 7274 4874 6d6c  Util.convertHtml
+0001ab00: 5461 6754 6f43 6f6c 6f72 616d 6128 7061  TagToColorama(pa
+0001ab10: 6765 7243 6f6e 7465 6e74 290a 2020 2020  gerContent).    
+0001ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab30: 6c61 6e67 7561 6765 203d 2022 5079 7468  language = "Pyth
+0001ab40: 6f6e 2220 6966 2022 6060 6070 7974 686f  on" if "```pytho
+0001ab50: 6e22 2069 6e20 7061 6765 7243 6f6e 7465  n" in pagerConte
+0001ab60: 6e74 2065 6c73 6520 224d 6172 6b64 6f77  nt else "Markdow
+0001ab70: 6e22 0a20 2020 2020 2020 2020 2020 2020  n".             
+0001ab80: 2020 2020 2020 2070 7964 6f63 2e70 6970         pydoc.pip
+0001ab90: 6570 6167 6572 2870 6167 6572 436f 6e74  epager(pagerCont
+0001aba0: 656e 742c 2063 6d64 3d66 2262 6174 202d  ent, cmd=f"bat -
+0001abb0: 6c20 7b6c 616e 6775 6167 657d 202d 2d70  l {language} --p
+0001abc0: 6167 696e 6720 616c 7761 7973 2229 0a20  aging always"). 
+0001abd0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001abe0: 6c69 6620 7368 7574 696c 2e77 6869 6368  lif shutil.which
+0001abf0: 2822 6c65 7373 2229 3a0a 2020 2020 2020  ("less"):.      
+0001ac00: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0001ac10: 5769 6e64 6f77 7320 7573 6572 7320 6361  Windows users ca
+0001ac20: 6e20 696e 7374 616c 6c20 6c65 7373 2063  n install less c
+0001ac30: 6f6d 6d61 6e64 2077 6974 6820 7363 6f6f  ommand with scoo
+0001ac40: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+0001ac50: 2020 2020 2020 2320 7265 6164 3a20 6874        # read: ht
+0001ac60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+0001ac70: 2f53 636f 6f70 496e 7374 616c 6c65 722f  /ScoopInstaller/
+0001ac80: 5363 6f6f 700a 2020 2020 2020 2020 2020  Scoop.          
+0001ac90: 2020 2020 2020 2020 2020 2320 3e20 6977            # > iw
+0001aca0: 7220 2d75 7365 6220 6765 742e 7363 6f6f  r -useb get.scoo
+0001acb0: 702e 7368 207c 2069 6578 0a20 2020 2020  p.sh | iex.     
+0001acc0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001acd0: 203e 2073 636f 6f70 2069 6e73 7461 6c6c   > scoop install
+0001ace0: 2061 7269 6132 206c 6573 730a 2020 2020   aria2 less.    
+0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad00: 6966 2072 652e 7365 6172 6368 2822 3c5b  if re.search("<[
+0001ad10: 5e3c 3e5d 2b3f 3e22 2c20 7061 6765 7243  ^<>]+?>", pagerC
+0001ad20: 6f6e 7465 6e74 293a 0a20 2020 2020 2020  ontent):.       
+0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad40: 2070 6167 6572 436f 6e74 656e 7420 3d20   pagerContent = 
+0001ad50: 5465 7874 5574 696c 2e63 6f6e 7665 7274  TextUtil.convert
+0001ad60: 4874 6d6c 5461 6754 6f43 6f6c 6f72 616d  HtmlTagToColoram
+0001ad70: 6128 7061 6765 7243 6f6e 7465 6e74 290a  a(pagerContent).
+0001ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad90: 2020 2020 7079 646f 632e 7069 7065 7061      pydoc.pipepa
+0001ada0: 6765 7228 7061 6765 7243 6f6e 7465 6e74  ger(pagerContent
+0001adb0: 2c20 636d 643d 276c 6573 7320 2d52 2729  , cmd='less -R')
+0001adc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001add0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001ade0: 2020 2020 2020 2020 2020 2070 7964 6f63             pydoc
+0001adf0: 2e70 6167 6572 2870 6167 6572 436f 6e74  .pager(pagerCont
+0001ae00: 656e 7429 0a20 2020 2020 2020 2020 2020  ent).           
+0001ae10: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+0001ae20: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+0001ae30: 7061 6765 7256 6965 7720 3d20 4661 6c73  pagerView = Fals
+0001ae40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0001ae50: 2020 7368 6f77 4572 726f 7273 2829 0a0a    showErrors()..
+0001ae60: 2020 2020 2320 7772 6170 2068 746d 6c20      # wrap html 
+0001ae70: 7465 7874 2061 7420 7370 6163 6573 0a20  text at spaces. 
+0001ae80: 2020 2064 6566 2067 6574 5772 6170 7065     def getWrappe
+0001ae90: 6448 544d 4c54 6578 7428 7365 6c66 2c20  dHTMLText(self, 
+0001aea0: 7465 7874 2c20 7465 726d 696e 616c 5f77  text, terminal_w
+0001aeb0: 6964 7468 3d4e 6f6e 6529 3a0a 2020 2020  idth=None):.    
+0001aec0: 2020 2020 6966 206e 6f74 2022 2022 2069      if not " " i
+0001aed0: 6e20 7465 7874 3a0a 2020 2020 2020 2020  n text:.        
+0001aee0: 2020 2020 7265 7475 726e 2074 6578 740a      return text.
+0001aef0: 2020 2020 2020 2020 6966 2074 6572 6d69          if termi
+0001af00: 6e61 6c5f 7769 6474 6820 6973 204e 6f6e  nal_width is Non
+0001af10: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0001af20: 6572 6d69 6e61 6c5f 7769 6474 6820 3d20  erminal_width = 
+0001af30: 7368 7574 696c 2e67 6574 5f74 6572 6d69  shutil.get_termi
+0001af40: 6e61 6c5f 7369 7a65 2829 2e63 6f6c 756d  nal_size().colum
+0001af50: 6e73 0a20 2020 2020 2020 2073 656c 662e  ns.        self.
+0001af60: 7772 6170 7065 6454 6578 7420 3d20 2222  wrappedText = ""
+0001af70: 0a20 2020 2020 2020 2073 656c 662e 6c69  .        self.li
+0001af80: 6e65 5769 6474 6820 3d20 300a 0a20 2020  neWidth = 0..   
+0001af90: 2020 2020 2064 6566 2061 6464 576f 7264       def addWord
+0001afa0: 7328 776f 7264 7329 3a0a 2020 2020 2020  s(words):.      
+0001afb0: 2020 2020 2020 776f 7264 7320 3d20 776f        words = wo
+0001afc0: 7264 732e 7370 6c69 7428 2220 2229 0a20  rds.split(" "). 
+0001afd0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+0001afe0: 6e64 6578 2c20 6974 656d 2069 6e20 656e  ndex, item in en
+0001aff0: 756d 6572 6174 6528 776f 7264 7329 3a0a  umerate(words):.
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b010: 6973 4c61 7374 4974 656d 203d 2028 6c65  isLastItem = (le
+0001b020: 6e28 776f 7264 7329 202d 2069 6e64 6578  n(words) - index
+0001b030: 203d 3d20 3129 0a20 2020 2020 2020 2020   == 1).         
+0001b040: 2020 2020 2020 2069 6620 6973 5f43 4a4b         if is_CJK
+0001b050: 2869 7465 6d29 3a0a 2020 2020 2020 2020  (item):.        
+0001b060: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001b070: 6949 6e64 6578 2c20 6920 696e 2065 6e75  iIndex, i in enu
+0001b080: 6d65 7261 7465 2869 7465 6d29 3a0a 2020  merate(item):.  
+0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0a0: 2020 2020 2020 6973 5370 6163 6549 7465        isSpaceIte
+0001b0b0: 6d20 3d20 286e 6f74 2069 734c 6173 7449  m = (not isLastI
+0001b0c0: 7465 6d20 616e 6420 286c 656e 2869 7465  tem and (len(ite
+0001b0d0: 6d29 202d 2069 496e 6465 7820 3d3d 2031  m) - iIndex == 1
+0001b0e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+0001b0f0: 2020 2020 2020 2020 2020 2069 5769 6474             iWidt
+0001b100: 6820 3d20 6765 7453 7472 696e 6757 6964  h = getStringWid
+0001b110: 7468 2869 290a 2020 2020 2020 2020 2020  th(i).          
+0001b120: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b130: 2069 7353 7061 6365 4974 656d 3a0a 2020   isSpaceItem:.  
+0001b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b150: 2020 2020 2020 2020 2020 6e65 774c 696e            newLin
+0001b160: 6557 6964 7468 203d 2073 656c 662e 6c69  eWidth = self.li
+0001b170: 6e65 5769 6474 6820 2b20 6957 6964 7468  neWidth + iWidth
+0001b180: 202b 2031 0a20 2020 2020 2020 2020 2020   + 1.           
+0001b190: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001b1a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001b1b0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0001b1c0: 6577 4c69 6e65 5769 6474 6820 3d20 7365  ewLineWidth = se
+0001b1d0: 6c66 2e6c 696e 6557 6964 7468 202b 2069  lf.lineWidth + i
+0001b1e0: 5769 6474 680a 2020 2020 2020 2020 2020  Width.          
+0001b1f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b200: 206e 6577 4c69 6e65 5769 6474 6820 3e20   newLineWidth > 
+0001b210: 7465 726d 696e 616c 5f77 6964 7468 3a0a  terminal_width:.
+0001b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b230: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b240: 2e77 7261 7070 6564 5465 7874 202b 3d20  .wrappedText += 
+0001b250: 6622 5c6e 7b69 7d20 2220 6966 2069 7353  f"\n{i} " if isS
+0001b260: 7061 6365 4974 656d 2065 6c73 6520 6622  paceItem else f"
+0001b270: 5c6e 7b69 7d22 0a20 2020 2020 2020 2020  \n{i}".         
+0001b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b290: 2020 2073 656c 662e 6c69 6e65 5769 6474     self.lineWidt
+0001b2a0: 6820 3d20 6957 6964 7468 202b 2031 2069  h = iWidth + 1 i
+0001b2b0: 6620 6973 5370 6163 6549 7465 6d20 656c  f isSpaceItem el
+0001b2c0: 7365 2069 5769 6474 680a 2020 2020 2020  se iWidth.      
 0001b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2e0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0001b2f0: 7261 7070 6564 5465 7874 202b 3d20 6622  rappedText += f"
-0001b300: 7b69 7d20 2220 6966 2069 7353 7061 6365  {i} " if isSpace
-0001b310: 4974 656d 2065 6c73 6520 690a 2020 2020  Item else i.    
-0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b330: 2020 2020 2020 2020 7365 6c66 2e6c 696e          self.lin
-0001b340: 6557 6964 7468 202b 3d20 6957 6964 7468  eWidth += iWidth
-0001b350: 202b 2031 2069 6620 6973 5370 6163 6549   + 1 if isSpaceI
-0001b360: 7465 6d20 656c 7365 2069 5769 6474 680a  tem else iWidth.
-0001b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b380: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001b390: 2020 2020 2020 2020 2020 6974 656d 5769            itemWi
-0001b3a0: 6474 6820 3d20 6765 7453 7472 696e 6757  dth = getStringW
-0001b3b0: 6964 7468 2869 7465 6d29 0a20 2020 2020  idth(item).     
-0001b3c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001b3d0: 6620 6973 4c61 7374 4974 656d 3a0a 2020  f isLastItem:.  
-0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3f0: 2020 2020 2020 6e65 774c 696e 6557 6964        newLineWid
-0001b400: 7468 203d 2073 656c 662e 6c69 6e65 5769  th = self.lineWi
-0001b410: 6474 6820 2b20 6974 656d 5769 6474 680a  dth + itemWidth.
-0001b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b430: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b450: 2020 6e65 774c 696e 6557 6964 7468 203d    newLineWidth =
-0001b460: 2073 656c 662e 6c69 6e65 5769 6474 6820   self.lineWidth 
-0001b470: 2b20 6974 656d 5769 6474 6820 2b20 310a  + itemWidth + 1.
-0001b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b490: 2020 2020 6966 206e 6577 4c69 6e65 5769      if newLineWi
-0001b4a0: 6474 6820 3e20 7465 726d 696e 616c 5f77  dth > terminal_w
-0001b4b0: 6964 7468 3a0a 2020 2020 2020 2020 2020  idth:.          
-0001b4c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001b4d0: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
-0001b4e0: 3d20 6622 5c6e 7b69 7465 6d7d 2220 6966  = f"\n{item}" if
-0001b4f0: 2069 734c 6173 7449 7465 6d20 656c 7365   isLastItem else
-0001b500: 2066 225c 6e7b 6974 656d 7d20 220a 2020   f"\n{item} ".  
-0001b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b520: 2020 2020 2020 7365 6c66 2e6c 696e 6557        self.lineW
-0001b530: 6964 7468 203d 2069 7465 6d57 6964 7468  idth = itemWidth
-0001b540: 2069 6620 6973 4c61 7374 4974 656d 2065   if isLastItem e
-0001b550: 6c73 6520 6974 656d 5769 6474 6820 2b20  lse itemWidth + 
-0001b560: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-0001b570: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001b2e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b300: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
+0001b310: 5465 7874 202b 3d20 6622 7b69 7d20 2220  Text += f"{i} " 
+0001b320: 6966 2069 7353 7061 6365 4974 656d 2065  if isSpaceItem e
+0001b330: 6c73 6520 690a 2020 2020 2020 2020 2020  lse i.          
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 2020 7365 6c66 2e6c 696e 6557 6964 7468    self.lineWidth
+0001b360: 202b 3d20 6957 6964 7468 202b 2031 2069   += iWidth + 1 i
+0001b370: 6620 6973 5370 6163 6549 7465 6d20 656c  f isSpaceItem el
+0001b380: 7365 2069 5769 6474 680a 2020 2020 2020  se iWidth.      
+0001b390: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0001b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b3b0: 2020 2020 6974 656d 5769 6474 6820 3d20      itemWidth = 
+0001b3c0: 6765 7453 7472 696e 6757 6964 7468 2869  getStringWidth(i
+0001b3d0: 7465 6d29 0a20 2020 2020 2020 2020 2020  tem).           
+0001b3e0: 2020 2020 2020 2020 2069 6620 6973 4c61           if isLa
+0001b3f0: 7374 4974 656d 3a0a 2020 2020 2020 2020  stItem:.        
+0001b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b410: 6e65 774c 696e 6557 6964 7468 203d 2073  newLineWidth = s
+0001b420: 656c 662e 6c69 6e65 5769 6474 6820 2b20  elf.lineWidth + 
+0001b430: 6974 656d 5769 6474 680a 2020 2020 2020  itemWidth.      
+0001b440: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001b450: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001b460: 2020 2020 2020 2020 2020 2020 6e65 774c              newL
+0001b470: 696e 6557 6964 7468 203d 2073 656c 662e  ineWidth = self.
+0001b480: 6c69 6e65 5769 6474 6820 2b20 6974 656d  lineWidth + item
+0001b490: 5769 6474 6820 2b20 310a 2020 2020 2020  Width + 1.      
+0001b4a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001b4b0: 206e 6577 4c69 6e65 5769 6474 6820 3e20   newLineWidth > 
+0001b4c0: 7465 726d 696e 616c 5f77 6964 7468 3a0a  terminal_width:.
+0001b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4e0: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
+0001b4f0: 7070 6564 5465 7874 202b 3d20 6622 5c6e  ppedText += f"\n
+0001b500: 7b69 7465 6d7d 2220 6966 2069 734c 6173  {item}" if isLas
+0001b510: 7449 7465 6d20 656c 7365 2066 225c 6e7b  tItem else f"\n{
+0001b520: 6974 656d 7d20 220a 2020 2020 2020 2020  item} ".        
+0001b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b540: 7365 6c66 2e6c 696e 6557 6964 7468 203d  self.lineWidth =
+0001b550: 2069 7465 6d57 6964 7468 2069 6620 6973   itemWidth if is
+0001b560: 4c61 7374 4974 656d 2065 6c73 6520 6974  LastItem else it
+0001b570: 656d 5769 6474 6820 2b20 310a 2020 2020  emWidth + 1.    
 0001b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b590: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
-0001b5a0: 5465 7874 202b 3d20 6974 656d 2069 6620  Text += item if 
-0001b5b0: 6973 4c61 7374 4974 656d 2065 6c73 6520  isLastItem else 
-0001b5c0: 6622 7b69 7465 6d7d 2022 0a20 2020 2020  f"{item} ".     
-0001b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b5e0: 2020 2073 656c 662e 6c69 6e65 5769 6474     self.lineWidt
-0001b5f0: 6820 2b3d 2069 7465 6d57 6964 7468 2069  h += itemWidth i
-0001b600: 6620 6973 4c61 7374 4974 656d 2065 6c73  f isLastItem els
-0001b610: 6520 6974 656d 5769 6474 6820 2b20 310a  e itemWidth + 1.
-0001b620: 0a20 2020 2020 2020 2064 6566 2070 726f  .        def pro
-0001b630: 6365 7373 4c69 6e65 286c 696e 6554 6578  cessLine(lineTex
-0001b640: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-0001b650: 6966 2072 652e 7365 6172 6368 2822 3c5b  if re.search("<[
-0001b660: 5e3c 3e5d 2b3f 3e22 2c20 6c69 6e65 5465  ^<>]+?>", lineTe
-0001b670: 7874 293a 0a20 2020 2020 2020 2020 2020  xt):.           
-0001b680: 2020 2020 2023 2068 616e 646c 6520 6874       # handle ht
-0001b690: 6d6c 2f78 6d6c 2074 6167 730a 2020 2020  ml/xml tags.    
-0001b6a0: 2020 2020 2020 2020 2020 2020 6368 756e              chun
-0001b6b0: 6b73 203d 206c 696e 6554 6578 742e 7370  ks = lineText.sp
-0001b6c0: 6c69 7428 223e 2229 0a20 2020 2020 2020  lit(">").       
-0001b6d0: 2020 2020 2020 2020 2074 6f74 616c 4368           totalCh
-0001b6e0: 756e 6b73 203d 206c 656e 2863 6875 6e6b  unks = len(chunk
-0001b6f0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-0001b700: 2020 2066 6f72 2069 6e64 6578 2c20 6368     for index, ch
-0001b710: 756e 6b20 696e 2065 6e75 6d65 7261 7465  unk in enumerate
-0001b720: 2863 6875 6e6b 7329 3a0a 2020 2020 2020  (chunks):.      
-0001b730: 2020 2020 2020 2020 2020 2020 2020 6973                is
-0001b740: 4c61 7374 4368 756e 6b20 3d20 2874 6f74  LastChunk = (tot
-0001b750: 616c 4368 756e 6b73 202d 2069 6e64 6578  alChunks - index
-0001b760: 203d 3d20 3129 0a20 2020 2020 2020 2020   == 1).         
-0001b770: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0001b780: 4c61 7374 4368 756e 6b3a 0a20 2020 2020  LastChunk:.     
-0001b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7a0: 2020 2061 6464 576f 7264 7328 6368 756e     addWords(chun
-0001b7b0: 6b29 0a20 2020 2020 2020 2020 2020 2020  k).             
-0001b7c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001b590: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001b5a0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001b5b0: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
+0001b5c0: 3d20 6974 656d 2069 6620 6973 4c61 7374  = item if isLast
+0001b5d0: 4974 656d 2065 6c73 6520 6622 7b69 7465  Item else f"{ite
+0001b5e0: 6d7d 2022 0a20 2020 2020 2020 2020 2020  m} ".           
+0001b5f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001b600: 662e 6c69 6e65 5769 6474 6820 2b3d 2069  f.lineWidth += i
+0001b610: 7465 6d57 6964 7468 2069 6620 6973 4c61  temWidth if isLa
+0001b620: 7374 4974 656d 2065 6c73 6520 6974 656d  stItem else item
+0001b630: 5769 6474 6820 2b20 310a 0a20 2020 2020  Width + 1..     
+0001b640: 2020 2064 6566 2070 726f 6365 7373 4c69     def processLi
+0001b650: 6e65 286c 696e 6554 6578 7429 3a0a 2020  ne(lineText):.  
+0001b660: 2020 2020 2020 2020 2020 6966 2072 652e            if re.
+0001b670: 7365 6172 6368 2822 3c5b 5e3c 3e5d 2b3f  search("<[^<>]+?
+0001b680: 3e22 2c20 6c69 6e65 5465 7874 293a 0a20  >", lineText):. 
+0001b690: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001b6a0: 2068 616e 646c 6520 6874 6d6c 2f78 6d6c   handle html/xml
+0001b6b0: 2074 6167 730a 2020 2020 2020 2020 2020   tags.          
+0001b6c0: 2020 2020 2020 6368 756e 6b73 203d 206c        chunks = l
+0001b6d0: 696e 6554 6578 742e 7370 6c69 7428 223e  ineText.split(">
+0001b6e0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0001b6f0: 2020 2074 6f74 616c 4368 756e 6b73 203d     totalChunks =
+0001b700: 206c 656e 2863 6875 6e6b 7329 0a20 2020   len(chunks).   
+0001b710: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001b720: 2069 6e64 6578 2c20 6368 756e 6b20 696e   index, chunk in
+0001b730: 2065 6e75 6d65 7261 7465 2863 6875 6e6b   enumerate(chunk
+0001b740: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+0001b750: 2020 2020 2020 2020 6973 4c61 7374 4368          isLastCh
+0001b760: 756e 6b20 3d20 2874 6f74 616c 4368 756e  unk = (totalChun
+0001b770: 6b73 202d 2069 6e64 6578 203d 3d20 3129  ks - index == 1)
+0001b780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b790: 2020 2020 2069 6620 6973 4c61 7374 4368       if isLastCh
+0001b7a0: 756e 6b3a 0a20 2020 2020 2020 2020 2020  unk:.           
+0001b7b0: 2020 2020 2020 2020 2020 2020 2061 6464               add
+0001b7c0: 576f 7264 7328 6368 756e 6b29 0a20 2020  Words(chunk).   
 0001b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7e0: 2020 2020 2074 6167 203d 2054 7275 6520       tag = True 
-0001b7f0: 6966 2022 3c22 2069 6e20 6368 756e 6b20  if "<" in chunk 
-0001b800: 656c 7365 2046 616c 7365 0a20 2020 2020  else False.     
-0001b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b820: 2020 2069 6620 7461 673a 0a20 2020 2020     if tag:.     
-0001b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b840: 2020 2020 2020 206e 6f6e 5461 672c 2074         nonTag, t
-0001b850: 6167 436f 6e74 656e 7420 3d20 6368 756e  agContent = chun
-0001b860: 6b2e 7273 706c 6974 2822 3c22 2c20 3129  k.rsplit("<", 1)
-0001b870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b880: 2020 2020 2020 2020 2020 2020 2061 6464               add
-0001b890: 576f 7264 7328 6e6f 6e54 6167 290a 2020  Words(nonTag).  
-0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8b0: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0001b8c0: 7261 7070 6564 5465 7874 202b 3d20 6622  rappedText += f"
-0001b8d0: 3c7b 7461 6743 6f6e 7465 6e74 7d3e 220a  <{tagContent}>".
-0001b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001b7e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001b7f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001b800: 6167 203d 2054 7275 6520 6966 2022 3c22  ag = True if "<"
+0001b810: 2069 6e20 6368 756e 6b20 656c 7365 2046   in chunk else F
+0001b820: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
+0001b830: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001b840: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b860: 206e 6f6e 5461 672c 2074 6167 436f 6e74   nonTag, tagCont
+0001b870: 656e 7420 3d20 6368 756e 6b2e 7273 706c  ent = chunk.rspl
+0001b880: 6974 2822 3c22 2c20 3129 0a20 2020 2020  it("<", 1).     
+0001b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8a0: 2020 2020 2020 2061 6464 576f 7264 7328         addWords(
+0001b8b0: 6e6f 6e54 6167 290a 2020 2020 2020 2020  nonTag).        
+0001b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8d0: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
+0001b8e0: 5465 7874 202b 3d20 6622 3c7b 7461 6743  Text += f"<{tagC
+0001b8f0: 6f6e 7465 6e74 7d3e 220a 2020 2020 2020  ontent}>".      
 0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 2020 2020 6164 6457 6f72            addWor
-0001b920: 6473 2866 227b 6368 756e 6b7d 3e22 290a  ds(f"{chunk}>").
-0001b930: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001b940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b950: 2020 6164 6457 6f72 6473 286c 696e 6554    addWords(lineT
-0001b960: 6578 7429 0a0a 2020 2020 2020 2020 6c69  ext)..        li
-0001b970: 6e65 7320 3d20 7465 7874 2e73 706c 6974  nes = text.split
-0001b980: 2822 5c6e 2229 0a20 2020 2020 2020 2074  ("\n").        t
-0001b990: 6f74 616c 4c69 6e65 7320 3d20 6c65 6e28  otalLines = len(
-0001b9a0: 6c69 6e65 7329 0a20 2020 2020 2020 2066  lines).        f
-0001b9b0: 6f72 2069 6e64 6578 2c20 6c69 6e65 2069  or index, line i
-0001b9c0: 6e20 656e 756d 6572 6174 6528 6c69 6e65  n enumerate(line
-0001b9d0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0001b9e0: 6973 4c61 7374 4c69 6e65 203d 2028 746f  isLastLine = (to
-0001b9f0: 7461 6c4c 696e 6573 202d 2069 6e64 6578  talLines - index
-0001ba00: 203d 3d20 3129 0a20 2020 2020 2020 2020   == 1).         
-0001ba10: 2020 2070 726f 6365 7373 4c69 6e65 286c     processLine(l
-0001ba20: 696e 6529 0a20 2020 2020 2020 2020 2020  ine).           
-0001ba30: 2069 6620 6e6f 7420 6973 4c61 7374 4c69   if not isLastLi
-0001ba40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001ba50: 2020 2020 7365 6c66 2e77 7261 7070 6564      self.wrapped
-0001ba60: 5465 7874 202b 3d20 225c 6e22 0a20 2020  Text += "\n".   
-0001ba70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001ba80: 662e 6c69 6e65 5769 6474 6820 3d20 300a  f.lineWidth = 0.
-0001ba90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001baa0: 7365 6c66 2e77 7261 7070 6564 5465 7874  self.wrappedText
-0001bab0: 0a                                       .
+0001b910: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b930: 2020 2020 6164 6457 6f72 6473 2866 227b      addWords(f"{
+0001b940: 6368 756e 6b7d 3e22 290a 2020 2020 2020  chunk}>").      
+0001b950: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0001b960: 2020 2020 2020 2020 2020 2020 6164 6457              addW
+0001b970: 6f72 6473 286c 696e 6554 6578 7429 0a0a  ords(lineText)..
+0001b980: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
+0001b990: 7465 7874 2e73 706c 6974 2822 5c6e 2229  text.split("\n")
+0001b9a0: 0a20 2020 2020 2020 2074 6f74 616c 4c69  .        totalLi
+0001b9b0: 6e65 7320 3d20 6c65 6e28 6c69 6e65 7329  nes = len(lines)
+0001b9c0: 0a20 2020 2020 2020 2066 6f72 2069 6e64  .        for ind
+0001b9d0: 6578 2c20 6c69 6e65 2069 6e20 656e 756d  ex, line in enum
+0001b9e0: 6572 6174 6528 6c69 6e65 7329 3a0a 2020  erate(lines):.  
+0001b9f0: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
+0001ba00: 4c69 6e65 203d 2028 746f 7461 6c4c 696e  Line = (totalLin
+0001ba10: 6573 202d 2069 6e64 6578 203d 3d20 3129  es - index == 1)
+0001ba20: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0001ba30: 6365 7373 4c69 6e65 286c 696e 6529 0a20  cessLine(line). 
+0001ba40: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001ba50: 7420 6973 4c61 7374 4c69 6e65 3a0a 2020  t isLastLine:.  
+0001ba60: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001ba70: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
+0001ba80: 3d20 225c 6e22 0a20 2020 2020 2020 2020  = "\n".         
+0001ba90: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+0001baa0: 5769 6474 6820 3d20 300a 0a20 2020 2020  Width = 0..     
+0001bab0: 2020 2072 6574 7572 6e20 7365 6c66 2e77     return self.w
+0001bac0: 7261 7070 6564 5465 7874 0a              rappedText.
```

### Comparing `freegenius-0.2.5/freegenius/utils/call_chatgpt.py` & `freegenius-0.2.6/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/call_gemini.py` & `freegenius-0.2.6/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/call_groq.py` & `freegenius-0.2.6/freegenius/utils/call_groq.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/call_llamacpp.py` & `freegenius-0.2.6/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/call_llm.py` & `freegenius-0.2.6/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/call_ollama.py` & `freegenius-0.2.6/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/config_essential.py` & `freegenius-0.2.6/freegenius/utils/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/config_tools.py` & `freegenius-0.2.6/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/download.py` & `freegenius-0.2.6/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/get_path_prompt.py` & `freegenius-0.2.6/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/ollama_models.py` & `freegenius-0.2.6/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/promptValidator.py` & `freegenius-0.2.6/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.2.6/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.2.6/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/prompts.py` & `freegenius-0.2.6/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/python_utils.py` & `freegenius-0.2.6/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/shared_utils.py` & `freegenius-0.2.6/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/shortcuts.py` & `freegenius-0.2.6/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/single_prompt.py` & `freegenius-0.2.6/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.2.6/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/sttLanguages.py` & `freegenius-0.2.6/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.2.6/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.2.6/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/text_utils.py` & `freegenius-0.2.6/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/tool_plugins.py` & `freegenius-0.2.6/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/ttsLanguages.py` & `freegenius-0.2.6/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius/utils/tts_utils.py` & `freegenius-0.2.6/freegenius/utils/tts_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from freegenius import config, getHideOutputSuffix
-import os, traceback, subprocess, re, sounddevice, soundfile, pydoc, sys
+import os, traceback, subprocess, re, sounddevice, soundfile, pydoc, shutil
 from gtts import gTTS
 from elevenlabs.client import ElevenLabs
 from elevenlabs import play
 from freegenius.utils.vlc_utils import VlcUtil
 try:
     from google.cloud import texttospeech
 except:
@@ -66,15 +66,15 @@
                         text=content,
                         voice=config.elevenlabsVoice,
                         model="eleven_multilingual_v2"
                     )
                     play(audio) # elevanlabs play function
                 elif config.ttsPlatform == "piper":
                     audioFile = os.path.join(config.freeGeniusAIFolder, "temp", "piper.wav")
-                    cmd = f'''{sys.executable} -m piper --model {config.piper_model} --output_file "{audioFile}"{getHideOutputSuffix()}'''
+                    cmd = f'''{shutil.which("piper")} --model {config.piper_model} --output_file "{audioFile}"{getHideOutputSuffix()}'''
                     pydoc.pipepager(content, cmd=cmd)
                     TTSUtil.playAudioFile(audioFile)
                 else:
                     if not config.ttsPlatform == "google":
                         config.ttsPlatform == "google"
                         config.saveConfig()
                     # use gTTS as default as config.ttsCommand is empty by default
```

### Comparing `freegenius-0.2.5/freegenius/utils/vlc_utils.py` & `freegenius-0.2.6/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius.egg-info/PKG-INFO` & `freegenius-0.2.6/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.2.5
+Version: 0.2.6
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.2.5/freegenius.egg-info/SOURCES.txt` & `freegenius-0.2.6/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius.egg-info/entry_points.txt` & `freegenius-0.2.6/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/freegenius.egg-info/requires.txt` & `freegenius-0.2.6/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.2.5/setup.py` & `freegenius-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
     """Pre-installation for installation mode."""
     # setting 'CMAKE_ARGS' for installation of 'llama-cpp-python'
     # read https://github.com/abetlen/llama-cpp-python
     def run(self):
         # https://github.com/abetlen/llama-cpp-python#installation-configuration
         os.system('''$env:CMAKE_ARGS = "-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS"''' if platform.system() == "Windows" else '''CMAKE_ARGS="-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS"''')
         os.environ['CMAKE_ARGS'] = "-DLLAMA_BLAS=ON -DLLAMA_BLAS_VENDOR=OpenBLAS"
-        # install piper-tts for Linux users only
-        os.system(f"{sys.executable} -m pip install piper-tts")
         install.run(self)
 
 # package name
 package_name_0 = os.path.join("package_name.txt")
 with open(package_name_0, "r", encoding="utf-8") as fileObj:
     package = fileObj.read()
 package_name_1 = os.path.join(package, "package_name.txt") # package readme
@@ -49,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.2.05",
+    version="0.2.06",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama or Groq Cloud API, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

