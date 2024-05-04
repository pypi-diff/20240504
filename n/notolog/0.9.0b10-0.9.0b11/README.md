# Comparing `tmp/notolog-0.9.0b10.tar.gz` & `tmp/notolog-0.9.0b11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notolog-0.9.0b10.tar", last modified: Mon Apr 29 04:05:19 2024, max compression
+gzip compressed data, was "notolog-0.9.0b11.tar", last modified: Sat May  4 21:28:01 2024, max compression
```

## Comparing `notolog-0.9.0b10.tar` & `notolog-0.9.0b11.tar`

### file list

```diff
@@ -1,311 +1,400 @@
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.592651 notolog-0.9.0b10/
--rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-04-28 21:48:22.000000 notolog-0.9.0b10/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      119 2024-04-29 03:37:45.000000 notolog-0.9.0b10/MANIFEST.in
--rw-r--r--   0 vadikus    (501) staff       (20)    15934 2024-04-29 04:05:19.591344 notolog-0.9.0b10/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)    14450 2024-04-29 01:01:37.000000 notolog-0.9.0b10/README.md
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.271943 notolog-0.9.0b10/app/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3493 2024-04-28 22:15:01.000000 notolog-0.9.0b10/app/app_config.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.273699 notolog-0.9.0b10/app/assets/
--rw-r--r--   0 vadikus    (501) staff       (20)     4238 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/notolog-example-image.png
--rw-r--r--   0 vadikus    (501) staff       (20)    88269 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/notolog-logo.png
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.226861 notolog-0.9.0b10/app/assets/themes/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.286463 notolog-0.9.0b10/app/assets/themes/calligraphy/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2145 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6307 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/calligraphy/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.313719 notolog-0.9.0b10/app/assets/themes/default/
--rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/editor.css
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.388227 notolog-0.9.0b10/app/assets/themes/default/icons/
--rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/LICENSE
--rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/arrow-clockwise.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/arrow-repeat.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/balloon-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/balloon.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/bandaid-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/bandaid.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up-right.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/caret-down-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/caret-up-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/code-slash.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/cursor-text.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/eyedropper.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/eyeglasses.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-lock2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-plus-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/file-earmark.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-html.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-md.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/filetype-txt.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/floppy2-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/floppy2.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder-symlink.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/folder.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/github.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/link-45deg.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/linkedin.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/pencil-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/power.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/quote.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/robot.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/share-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/star-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/star.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/three-dots.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/trash3-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/trash3.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/twitter-x.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-bold.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-italic.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-strikethrough.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/type-underline.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-circle-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-square-fill.svg
--rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/icons/x-square.svg
--rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7957 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/default/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.398582 notolog-0.9.0b10/app/assets/themes/noir_dark/
--rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     6410 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/noir_dark/viewer.ini
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.413591 notolog-0.9.0b10/app/assets/themes/strawberry/
--rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/about_popup.css
--rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/ai_assistant.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/default.ini
--rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/editor.css
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/md.ini
--rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/settings_dialog.css
--rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/statusbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)     7940 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/styles.css
--rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/toolbar.css
--rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/tree_view.css
--rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/viewer.css
--rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/assets/themes/strawberry/viewer.ini
--rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/edit_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/editor_state.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.421800 notolog-0.9.0b10/app/encrypt/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-04-28 21:48:25.000000 notolog-0.9.0b10/app/encrypt/enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_new_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3149 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/encrypt/enc_password_reset_dialog.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.426868 notolog-0.9.0b10/app/enums/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/ai_model_names.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/colors.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1335 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/languages.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/enums/themes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2866 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/etree_extension.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.428229 notolog-0.9.0b10/app/exceptions/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/exceptions/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/exceptions/file_header_empty_exception.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6945 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/file_system_watcher.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.434431 notolog-0.9.0b10/app/helpers/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/clipboard_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2437 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/file_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/tooltip_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7167 2024-04-28 21:48:26.000000 notolog-0.9.0b10/app/helpers/update_helper.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.438514 notolog-0.9.0b10/app/highlight/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8594 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/main_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)    47898 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/highlight/md_highlighter.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8007 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/highlight/view_highlighter.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.439981 notolog-0.9.0b10/app/lexemes/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/lexemes/__init__.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.442471 notolog-0.9.0b10/app/lexemes/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      164 2024-04-29 00:12:00.000000 notolog-0.9.0b10/app/lexemes/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3221 2024-04-28 22:06:29.000000 notolog-0.9.0b10/app/lexemes/__pycache__/lexemes.cpython-39.pyc
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.449431 notolog-0.9.0b10/app/lexemes/de/
--rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6547 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3514 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/de/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.459138 notolog-0.9.0b10/app/lexemes/en/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.470093 notolog-0.9.0b10/app/lexemes/en/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)      883 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6660 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     5428 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2083 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3248 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2492 2024-04-28 22:11:17.000000 notolog-0.9.0b10/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6009 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3351 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/en/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.478342 notolog-0.9.0b10/app/lexemes/es/
--rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6517 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3615 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/es/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.486162 notolog-0.9.0b10/app/lexemes/fr/
--rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6677 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3690 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/fr/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.492552 notolog-0.9.0b10/app/lexemes/ge/
--rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9689 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5310 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ge/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.499423 notolog-0.9.0b10/app/lexemes/it/
--rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6327 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3562 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/it/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.505811 notolog-0.9.0b10/app/lexemes/ja/
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.517116 notolog-0.9.0b10/app/lexemes/ja/__pycache__/
--rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     6809 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3780 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-04-28 22:06:30.000000 notolog-0.9.0b10/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
--rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7209 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3747 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ja/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.526296 notolog-0.9.0b10/app/lexemes/ko/
--rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ko/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6733 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3414 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ko/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/ko/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.533207 notolog-0.9.0b10/app/lexemes/la/
--rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6204 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3505 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/lexemes/la/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/lexemes.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.539032 notolog-0.9.0b10/app/lexemes/pt/
--rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6315 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3574 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/pt/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.545516 notolog-0.9.0b10/app/lexemes/ru/
--rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7899 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4504 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/ru/toolbar.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.551915 notolog-0.9.0b10/app/lexemes/zh/
--rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5738 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/common.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/main_menu.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3256 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-04-28 21:48:23.000000 notolog-0.9.0b10/app/lexemes/zh/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)   177102 2024-04-29 04:00:35.000000 notolog-0.9.0b10/app/notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)    11239 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5968 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/theme.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.575529 notolog-0.9.0b10/app/ui/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7920 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/about_popup.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/ai_assistant.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/color_picker_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3311 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/common_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/enum_combo_box.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/file_system_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/line_numbers.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2526 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/rename_file_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/rotating_label.py
--rw-r--r--   0 vadikus    (501) staff       (20)    35991 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/settings_dialog.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/sort_filter_proxy_model.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6831 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/statusbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4313 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/toolbar.py
--rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-04-28 21:48:22.000000 notolog-0.9.0b10/app/ui/vertical_line_spacer.py
--rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_decorator.py
--rw-r--r--   0 vadikus    (501) staff       (20)    16031 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_processor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2253 2024-04-28 21:48:24.000000 notolog-0.9.0b10/app/view_widget.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2521 2024-04-29 03:37:45.000000 notolog-0.9.0b10/main.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.590396 notolog-0.9.0b10/notolog.egg-info/
--rw-r--r--   0 vadikus    (501) staff       (20)    15934 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/PKG-INFO
--rw-r--r--   0 vadikus    (501) staff       (20)     9693 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/SOURCES.txt
--rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/dependency_links.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/entry_points.txt
--rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/requires.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-04-29 04:05:19.000000 notolog-0.9.0b10/notolog.egg-info/top_level.txt
--rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-04-29 04:05:19.592872 notolog-0.9.0b10/setup.cfg
--rw-r--r--   0 vadikus    (501) staff       (20)     1650 2024-04-29 03:47:58.000000 notolog-0.9.0b10/setup.py
-drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-04-29 04:05:19.589373 notolog-0.9.0b10/tests/
--rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-04-28 21:48:22.000000 notolog-0.9.0b10/tests/__init__.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_enc_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_enc_password.py
--rw-r--r--   0 vadikus    (501) staff       (20)     9197 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_file_header.py
--rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_html_view.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_lexemes.py
--rw-r--r--   0 vadikus    (501) staff       (20)     5645 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_notolog_editor.py
--rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_settings.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_text_block_data.py
--rw-r--r--   0 vadikus    (501) staff       (20)     4053 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_theme_helper.py
--rw-r--r--   0 vadikus    (501) staff       (20)     6182 2024-04-29 03:30:40.000000 notolog-0.9.0b10/tests/test_themes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.374982 notolog-0.9.0b11/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1073 2024-05-04 21:27:31.000000 notolog-0.9.0b11/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      119 2024-05-04 21:27:32.000000 notolog-0.9.0b11/MANIFEST.in
+-rw-r--r--   0 vadikus    (501) staff       (20)    17291 2024-05-04 21:28:01.373698 notolog-0.9.0b11/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    15145 2024-05-04 21:27:32.000000 notolog-0.9.0b11/README.md
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:00.979927 notolog-0.9.0b11/app/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3924 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/app_config.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:00.981353 notolog-0.9.0b11/app/assets/
+-rw-r--r--   0 vadikus    (501) staff       (20)     4202 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/notolog-example-image.png
+-rw-r--r--   0 vadikus    (501) staff       (20)    88211 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/notolog-logo.png
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:00.953439 notolog-0.9.0b11/app/assets/themes/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:00.990460 notolog-0.9.0b11/app/assets/themes/calligraphy/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      365 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2187 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      903 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6330 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      743 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       80 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/calligraphy/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.001312 notolog-0.9.0b11/app/assets/themes/default/
+-rw-r--r--   0 vadikus    (501) staff       (20)      798 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      253 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      174 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/editor.css
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.053520 notolog-0.9.0b11/app/assets/themes/default/icons/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1093 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/LICENSE
+-rw-r--r--   0 vadikus    (501) staff       (20)      349 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/arrow-clockwise.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      567 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/arrow-repeat.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      736 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/balloon-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      797 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/balloon.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      812 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/bandaid-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      959 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/bandaid.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      528 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/box-arrow-up-right.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      538 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/box-arrow-up.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/caret-down-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      265 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/caret-up-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/code-slash.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      694 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/cursor-text.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      459 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/eyedropper.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      403 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/eyeglasses.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      479 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/file-earmark-lock2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      394 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/file-earmark-plus-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      481 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/file-earmark-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      294 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/file-earmark.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      547 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/filetype-html.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      705 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/filetype-md.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      524 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/filetype-txt.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      401 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/floppy2-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      606 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/floppy2.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      428 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/folder-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/folder-symlink.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      527 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/folder.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      708 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/github.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      518 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/link-45deg.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      666 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/linkedin.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      575 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/pencil-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      261 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/power.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      582 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/quote.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      996 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/robot.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      316 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/share-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      653 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/shield-lock-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     1057 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/shield-lock.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      399 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/star-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      623 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/star.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      272 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/three-dots.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      577 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/trash3-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      656 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/trash3.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      301 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/twitter-x.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      465 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/type-bold.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/type-italic.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      574 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/type-strikethrough.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      319 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/type-underline.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      351 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/x-circle-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      397 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/x-square-fill.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)      491 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/icons/x-square.svg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2250 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      739 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7980 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      744 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       82 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/default/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.068222 notolog-0.9.0b11/app/assets/themes/noir_dark/
+-rw-r--r--   0 vadikus    (501) staff       (20)      777 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      347 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2745 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       56 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2357 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     1435 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     6433 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      280 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      711 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       28 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       76 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/noir_dark/viewer.ini
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.084857 notolog-0.9.0b11/app/assets/themes/strawberry/
+-rw-r--r--   0 vadikus    (501) staff       (20)      790 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/about_popup.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      317 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/ai_assistant.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2775 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/default.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)       50 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/editor.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/md.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)      771 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/settings_dialog.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      115 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/statusbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)     7963 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/styles.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      221 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/toolbar.css
+-rw-r--r--   0 vadikus    (501) staff       (20)      764 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/tree_view.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       60 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/viewer.css
+-rw-r--r--   0 vadikus    (501) staff       (20)       84 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/assets/themes/strawberry/viewer.ini
+-rw-r--r--   0 vadikus    (501) staff       (20)     7823 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/edit_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4196 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/editor_state.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.090122 notolog-0.9.0b11/app/encrypt/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4267 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6133 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/enc_new_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      551 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4229 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/enc_password_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3247 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/encrypt/enc_password_reset_dialog.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.097968 notolog-0.9.0b11/app/enums/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/enums/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1855 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/enums/ai_model_names.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6229 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/enums/colors.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1388 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/enums/languages.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1365 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/enums/themes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3236 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/etree_extension.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.101707 notolog-0.9.0b11/app/exceptions/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/exceptions/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)       52 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/exceptions/file_header_empty_exception.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7388 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2856 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/file_system_watcher.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.107596 notolog-0.9.0b11/app/helpers/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      187 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/clipboard_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/file_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5511 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      696 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/tooltip_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7411 2024-05-04 21:27:31.000000 notolog-0.9.0b11/app/helpers/update_helper.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.111387 notolog-0.9.0b11/app/highlight/
+-rw-r--r--   0 vadikus    (501) staff       (20)      126 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/highlight/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9027 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/highlight/main_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    48888 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/highlight/md_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8475 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/highlight/view_highlighter.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9589 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/image_downloader.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.114930 notolog-0.9.0b11/app/lexemes/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/__init__.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.118324 notolog-0.9.0b11/app/lexemes/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      157 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3221 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/__pycache__/lexemes.cpython-39.pyc
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.134160 notolog-0.9.0b11/app/lexemes/de/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.139369 notolog-0.9.0b11/app/lexemes/de/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6854 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5899 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2183 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2914 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1272 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2730 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      830 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7202 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6579 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2267 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3788 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1225 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2757 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/de/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.155442 notolog-0.9.0b11/app/lexemes/en/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.170291 notolog-0.9.0b11/app/lexemes/en/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      883 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6660 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5459 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2083 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3467 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2492 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      827 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7096 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6044 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2181 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3586 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1201 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2573 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/en/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.175881 notolog-0.9.0b11/app/lexemes/es/
+-rw-r--r--   0 vadikus    (501) staff       (20)      882 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7309 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6549 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2316 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3890 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1222 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2793 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/es/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.188796 notolog-0.9.0b11/app/lexemes/fr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.200861 notolog-0.9.0b11/app/lexemes/fr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      977 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6899 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6212 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2256 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3928 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1274 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2794 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      886 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7247 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6709 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2344 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3978 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1236 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2824 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/fr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.207689 notolog-0.9.0b11/app/lexemes/ge/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.215694 notolog-0.9.0b11/app/lexemes/ge/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1355 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)    10384 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9053 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3389 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5710 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1642 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4138 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1323 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10627 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9721 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ge/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3459 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5742 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ge/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1583 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ge/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4107 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ge/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.221974 notolog-0.9.0b11/app/lexemes/gr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.227969 notolog-0.9.0b11/app/lexemes/gr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1172 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8982 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8175 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2804 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5014 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1528 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3735 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/lexemes/gr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1100 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/lexemes/gr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8990 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/lexemes/gr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8654 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2907 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/lexemes/gr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5016 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1561 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/lexemes/gr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3679 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/gr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.234322 notolog-0.9.0b11/app/lexemes/in/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.251775 notolog-0.9.0b11/app/lexemes/in/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1328 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9403 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     9416 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3029 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5585 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1618 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1208 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9434 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    10062 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3124 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5546 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1549 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3828 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/in/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.264307 notolog-0.9.0b11/app/lexemes/it/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.269434 notolog-0.9.0b11/app/lexemes/it/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      930 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6824 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5639 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2188 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2925 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1290 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2700 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      864 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7263 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6359 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2302 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3825 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1238 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2780 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/it/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.274129 notolog-0.9.0b11/app/lexemes/ja/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.283509 notolog-0.9.0b11/app/lexemes/ja/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)     1020 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     8452 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6837 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2411 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     4046 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1301 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3047 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      931 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8464 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7241 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2443 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4014 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1242 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3000 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ja/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.297515 notolog-0.9.0b11/app/lexemes/ko/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.302990 notolog-0.9.0b11/app/lexemes/ko/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      951 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7559 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     6401 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2274 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3720 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1282 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2732 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      848 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7597 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6765 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2268 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3697 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1221 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2666 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/ko/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.308834 notolog-0.9.0b11/app/lexemes/la/
+-rw-r--r--   0 vadikus    (501) staff       (20)      842 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7538 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6236 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2297 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3753 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1257 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2736 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/la/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3739 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/lexemes.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.315842 notolog-0.9.0b11/app/lexemes/pt/
+-rw-r--r--   0 vadikus    (501) staff       (20)      898 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7304 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6347 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2326 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3830 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1223 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2830 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/pt/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.320490 notolog-0.9.0b11/app/lexemes/ru/
+-rw-r--r--   0 vadikus    (501) staff       (20)      997 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9135 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7931 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2883 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4896 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1428 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3453 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/ru/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.324936 notolog-0.9.0b11/app/lexemes/tr/
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.330388 notolog-0.9.0b11/app/lexemes/tr/__pycache__/
+-rw-r--r--   0 vadikus    (501) staff       (20)      912 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/ai_assistant.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     7114 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/color_picker_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     5741 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2272 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/main_menu.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     3751 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/settings_dialog.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     1297 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/statusbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)     2767 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/__pycache__/toolbar.cpython-39.pyc
+-rw-r--r--   0 vadikus    (501) staff       (20)      809 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7401 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6147 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2276 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3733 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1240 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2735 2024-05-04 21:27:29.000000 notolog-0.9.0b11/app/lexemes/tr/toolbar.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.346417 notolog-0.9.0b11/app/lexemes/zh/
+-rw-r--r--   0 vadikus    (501) staff       (20)      792 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7074 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5770 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/common.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2175 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/main_menu.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3476 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1202 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2559 2024-05-04 21:27:28.000000 notolog-0.9.0b11/app/lexemes/zh/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)   175532 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6260 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3481 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6022 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/theme.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.357097 notolog-0.9.0b11/app/ui/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8280 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/about_popup.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16871 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/ai_assistant.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2134 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/color_picker_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3520 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/common_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1306 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/enum_combo_box.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5635 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/file_system_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     7063 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/line_numbers.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2712 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/rename_file_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1229 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/rotating_label.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    37330 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/settings_dialog.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3207 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/sort_filter_proxy_model.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6896 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/statusbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    12713 2024-05-04 21:27:27.000000 notolog-0.9.0b11/app/ui/toolbar.py
+-rw-r--r--   0 vadikus    (501) staff       (20)      455 2024-05-04 21:27:26.000000 notolog-0.9.0b11/app/ui/vertical_line_spacer.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     8191 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/view_decorator.py
+-rw-r--r--   0 vadikus    (501) staff       (20)    16132 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/view_processor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2446 2024-05-04 21:27:30.000000 notolog-0.9.0b11/app/view_widget.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2702 2024-05-04 21:27:41.000000 notolog-0.9.0b11/main.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.372282 notolog-0.9.0b11/notolog.egg-info/
+-rw-r--r--   0 vadikus    (501) staff       (20)    17291 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/PKG-INFO
+-rw-r--r--   0 vadikus    (501) staff       (20)    13371 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/SOURCES.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)        1 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/dependency_links.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/entry_points.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)      367 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/requires.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       15 2024-05-04 21:28:00.000000 notolog-0.9.0b11/notolog.egg-info/top_level.txt
+-rw-r--r--   0 vadikus    (501) staff       (20)       38 2024-05-04 21:28:01.375167 notolog-0.9.0b11/setup.cfg
+-rw-r--r--   0 vadikus    (501) staff       (20)     2167 2024-05-04 21:27:32.000000 notolog-0.9.0b11/setup.py
+drwxr-xr-x   0 vadikus    (501) staff       (20)        0 2024-05-04 21:28:01.371350 notolog-0.9.0b11/tests/
+-rw-r--r--   0 vadikus    (501) staff       (20)        0 2024-05-04 21:27:31.000000 notolog-0.9.0b11/tests/__init__.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5975 2024-05-04 21:27:31.000000 notolog-0.9.0b11/tests/test_enc_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     2305 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_enc_password.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     9197 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_file_header.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     3962 2024-05-04 21:27:31.000000 notolog-0.9.0b11/tests/test_html_view.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5810 2024-05-04 21:27:31.000000 notolog-0.9.0b11/tests/test_lexemes.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     5823 2024-05-04 21:27:31.000000 notolog-0.9.0b11/tests/test_notolog_editor.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     1154 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_settings.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4971 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_text_block_data.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     4464 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_theme_helper.py
+-rw-r--r--   0 vadikus    (501) staff       (20)     6222 2024-05-04 21:27:32.000000 notolog-0.9.0b11/tests/test_themes.py
```

### Comparing `notolog-0.9.0b10/LICENSE` & `notolog-0.9.0b11/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/PKG-INFO` & `notolog-0.9.0b11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b10
+Version: 0.9.0b11
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
+Keywords: notolog,ai,markdown,editor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Text Editors
+Classifier: Topic :: Text Editors :: Documentation
+Classifier: Topic :: Text Editors :: Emacs
+Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Topic :: Text Editors :: Word Processors
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi==1.16.0
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: emoji==2.11.1
@@ -27,34 +41,40 @@
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
-Requires-Dist: pytest==8.1.2
+Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: qasync==0.27.1
 Requires-Dist: qt6-applications==6.5.0.2.3
 Requires-Dist: qt6-tools==6.5.0.1.3
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-04-29 02:01:37.002734"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
 # Notolog
 
+![Notolog](app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
 ## Overview
 
 Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
 
 In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
 
 The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
 
+---
+![Notolog settings UI example](docs/notolog-ui-settings.png)
+
+
 ## Features
 
 * Open sourced under the MIT license for full transparency and collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
@@ -83,94 +103,102 @@
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 
----
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
-## Prerequisites:
+
+## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
-Check the version of Python available with this command:
-```sh
-python3 -V
-```
+Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
+
 You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
 
+**Virtual Environment**
+
+It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
+
+
 ## Installation
 
-### Using pip installer (Recommended)
+### Method 1: pip installer (Recommended)
 
 ```sh
 pip install notolog
 ```
 
-### Run the Python code
+That's it! Starting the app is as simple as `notolog`.
+
+To update to the latest version, use:
+```sh
+pip install --upgrade notolog
+```
+
+### Method 2: Python source code
 
 0. Open Terminal.
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
-2. Navigate to your project directory using the **cd** command.
-3. Make sure the virtual environment is activated as it's a common practice to isolate project code (described below).
+2. Navigate to the just cloned project's directory using the **cd** command.
+3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
 pip3 install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python3 main.py`
 
-### Using Virtual Environments
+<details>
+<summary>Run tests</summary>
+
+To run all available tests:
+```sh
+pytest
+```
+
+To run a particular file's tests:
+```sh
+pytest tests/test_notolog_editor.py
+```
+</details>
+
+### Virtual Environments
 
-The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html)
+The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
 #### MacOS and Linux
 
 ##### Set Up Virtual Environment
-
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
-Activate Virtual Environment:
+##### Activate Virtual Environment:
 To activate the virtual environment, run:
 ```sh
 source notolog/bin/activate
 ```
 
 To deactivate environment just run this command:
 ```sh
 deactivate
 ```
 
-#### Windows
-
-##### Set Up Virtual Environment
-
-1. Open Command Prompt or PowerShell.
-2. Navigate to your project directory using the `cd` command.
-3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
-
-##### Activate Virtual Environment
-
-To activate the virtual environment, run:
-```
-notolog\Scripts\activate
-```
-_Mind the environment name (**notolog** or any other selected before)._
-
-##### Install venv on Linux systems
+<details>
+<summary>Install venv on Linux systems</summary>
 
 While Python itself comes pre-installed on many Linux distributions, including Ubuntu, some distributions may not include the venv module by default. Therefore, you need to install it separately using the package manager before you can use it to create virtual environments.
 
 **Ubuntu/Debian**
 
 ```sh
 sudo apt-get update
@@ -184,37 +212,32 @@
 ```
 
 **CentOS/RHEL**
 
 ```sh
 sudo yum install python3-venv
 ```
+</details>
 
-### Using IDE
-
-Alternatively, you can execute the Notolog code with your favorite Python code editor.
+#### Windows
 
-## Usage
+##### Set Up Virtual Environment
 
-To start the app simply run this command in a project dir:
-```sh
-python3 main.py
-```
+1. Open Command Prompt or PowerShell.
+2. Navigate to your project directory using the `cd` command.
+3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
 
-### Run tests
+##### Activate Virtual Environment
 
-To run all available tests:
-```sh
-pytest
+To activate the virtual environment, run:
 ```
-
-To run a particular file's tests:
-```sh
-pytest tests/test_notolog_editor.py
+notolog\Scripts\activate
 ```
+_Mind the environment name (**notolog** or any other selected before)._
+
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
 
 ## License
 
@@ -277,10 +300,10 @@
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b10/README.md` & `notolog-0.9.0b11/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-04-29 02:01:37.002734"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
 # Notolog
 
+![Notolog](app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
 ## Overview
 
 Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
 
 In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
 
 The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
 
+---
+![Notolog settings UI example](docs/notolog-ui-settings.png)
+
+
 ## Features
 
 * Open sourced under the MIT license for full transparency and collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
@@ -41,94 +47,102 @@
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 
----
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
-## Prerequisites:
+
+## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
-Check the version of Python available with this command:
-```sh
-python3 -V
-```
+Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
+
 You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
 
+**Virtual Environment**
+
+It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
+
+
 ## Installation
 
-### Using pip installer (Recommended)
+### Method 1: pip installer (Recommended)
 
 ```sh
 pip install notolog
 ```
 
-### Run the Python code
+That's it! Starting the app is as simple as `notolog`.
+
+To update to the latest version, use:
+```sh
+pip install --upgrade notolog
+```
+
+### Method 2: Python source code
 
 0. Open Terminal.
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
-2. Navigate to your project directory using the **cd** command.
-3. Make sure the virtual environment is activated as it's a common practice to isolate project code (described below).
+2. Navigate to the just cloned project's directory using the **cd** command.
+3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
 pip3 install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python3 main.py`
 
-### Using Virtual Environments
+<details>
+<summary>Run tests</summary>
 
-The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html)
+To run all available tests:
+```sh
+pytest
+```
+
+To run a particular file's tests:
+```sh
+pytest tests/test_notolog_editor.py
+```
+</details>
+
+### Virtual Environments
+
+The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
 #### MacOS and Linux
 
 ##### Set Up Virtual Environment
-
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
-Activate Virtual Environment:
+##### Activate Virtual Environment:
 To activate the virtual environment, run:
 ```sh
 source notolog/bin/activate
 ```
 
 To deactivate environment just run this command:
 ```sh
 deactivate
 ```
 
-#### Windows
-
-##### Set Up Virtual Environment
-
-1. Open Command Prompt or PowerShell.
-2. Navigate to your project directory using the `cd` command.
-3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
-
-##### Activate Virtual Environment
-
-To activate the virtual environment, run:
-```
-notolog\Scripts\activate
-```
-_Mind the environment name (**notolog** or any other selected before)._
-
-##### Install venv on Linux systems
+<details>
+<summary>Install venv on Linux systems</summary>
 
 While Python itself comes pre-installed on many Linux distributions, including Ubuntu, some distributions may not include the venv module by default. Therefore, you need to install it separately using the package manager before you can use it to create virtual environments.
 
 **Ubuntu/Debian**
 
 ```sh
 sudo apt-get update
@@ -142,37 +156,32 @@
 ```
 
 **CentOS/RHEL**
 
 ```sh
 sudo yum install python3-venv
 ```
+</details>
 
-### Using IDE
-
-Alternatively, you can execute the Notolog code with your favorite Python code editor.
+#### Windows
 
-## Usage
+##### Set Up Virtual Environment
 
-To start the app simply run this command in a project dir:
-```sh
-python3 main.py
-```
+1. Open Command Prompt or PowerShell.
+2. Navigate to your project directory using the `cd` command.
+3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
 
-### Run tests
+##### Activate Virtual Environment
 
-To run all available tests:
-```sh
-pytest
+To activate the virtual environment, run:
 ```
-
-To run a particular file's tests:
-```sh
-pytest tests/test_notolog_editor.py
+notolog\Scripts\activate
 ```
+_Mind the environment name (**notolog** or any other selected before)._
+
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
 
 ## License
 
@@ -235,10 +244,10 @@
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
-`╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
+`╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b10/app/app_config.py` & `notolog-0.9.0b11/app/app_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Union
 
 import tomli
 
 toml_app_config = """
 [app]
 name = "Notolog"
-version = "0.9.0b0"
+version = "0.9.0b11"
 license = "MIT"
 date = "2024"
 website = "https://notolog.app"
 repository = "https://github.com/notolog/notolog-editor"
+pypi = "https://pypi.org/project/notolog"
 
 [repository]
 
     [repository.github]
     username = "notolog"
     project = "editor"
     release_url = "https://api.github.com/repos/notolog/notolog-editor/releases/latest"
@@ -37,14 +38,17 @@
 
     app_config = tomli.loads(toml_app_config)
 
     # Font settings
     _font_size = app_config['font']['base_size']  # Base value
     _prev_font_size = app_config['font']['base_size']  # Previous value
 
+    # For pytest to allow override some params
+    _test_mode = False
+
     """
     Constant values with getters.
     """
 
     @classmethod
     def get_app_name(cls) -> str:
         return cls.app_config['app']['name']
@@ -62,14 +66,22 @@
         return cls.app_config['app']['date']
 
     @classmethod
     def get_app_website(cls) -> str:
         return cls.app_config['app']['website']
 
     @classmethod
+    def get_app_repository(cls) -> str:
+        return cls.app_config['app']['repository']
+
+    @classmethod
+    def get_app_pypi(cls) -> str:
+        return cls.app_config['app']['pypi']
+
+    @classmethod
     def get_repository_github_username(cls) -> str:
         return cls.app_config['repository']['github']['username']
 
     @classmethod
     def get_repository_github_project(cls) -> str:
         return cls.app_config['repository']['github']['username']
 
@@ -81,18 +93,14 @@
     def get_repository_github_bug_report_url(cls) -> str:
         return cls.app_config['repository']['github']['bug_report_url']
 
     @classmethod
     def get_font_base_size(cls) -> int:
         return cls.app_config['font']['base_size']
 
-    @classmethod
-    def get_app_repository(cls) -> str:
-        return cls.app_config['app']['repository']
-
     """
     Methods with setter to override default value.
     """
 
     @classmethod
     def set_logging(cls, value) -> None:
         cls.app_config['logger']['logging'] = value
@@ -121,14 +129,18 @@
     def set_font_max_size(cls, value) -> None:
         cls.app_config['font']['max_size'] = value
 
     @classmethod
     def get_font_max_size(cls) -> int:
         return cls.app_config['font']['max_size']
 
+    """
+    Class system variables
+    """
+
     @classmethod
     def set_font_size(cls, value) -> None:
         cls._font_size = value
 
     @classmethod
     def get_font_size(cls) -> int:
         return cls._font_size
@@ -136,7 +148,15 @@
     @classmethod
     def set_prev_font_size(cls, value) -> None:
         cls._prev_font_size = value
 
     @classmethod
     def get_prev_font_size(cls) -> int:
         return cls._prev_font_size
+
+    @classmethod
+    def set_test_mode(cls, value) -> None:
+        cls._test_mode = value
+
+    @classmethod
+    def get_test_mode(cls) -> bool:
+        return cls._test_mode
```

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/about_popup.css` & `notolog-0.9.0b11/app/assets/themes/calligraphy/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/default.ini` & `notolog-0.9.0b11/app/assets/themes/calligraphy/default.ini`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 color_palette_mid_light=0x0F0F0F
 color_palette_shadow=0x000000
 color_palette_bright_text=0x000000
 color_palette_link=0xFF0000
 color_palette_link_visited=0xCC0000
 color_palette_placeholder_text=0xBBBBBB
 color_palette_accent=0xFFFFFF
-color_palette_highlight=0x000000
+color_palette_highlight=0xFF0000
 color_palette_highlighted_text=0xFFFFFF
 
 main_menu_icon_color=0xFF0000
 
 # check tree_view.css as well
 main_tree_background=0x000000
 main_tree_file_highlighted_in_transit=0x777777
```

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/md.ini` & `notolog-0.9.0b11/app/assets/themes/calligraphy/md.ini`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 md_background_color_codel=black
 md_color_codelf=white
 md_background_color_codelf=black
 md_color_code_lang=black
 md_color_code_indent=
 md_background_color_code_indent=black
 md_color_code_content=black
+md_background_color_code_content=whitesmoke
 md_color_wrong_indent=
 md_background_color_wrong_indent=black
 md_color_comment=grey
 md_background_color_comment=white
 md_color_img=black
 md_color_ref=white
 md_background_color_ref=black
@@ -62,16 +63,16 @@
 md_background_color_list_indent=black
 md_color_hr=white
 md_background_color_hr=black
 md_color_blockquote=white
 md_background_color_blockquote=grey
 md_background_color_blockquote_friendly=black
 md_color_html=black
-md_color_html_open=black
-md_color_html_close=black
+md_color_html_open=grey
+md_color_html_close=grey
 md_color_html_comment=grey
 md_color_emoji=white
 md_background_color_emoji=black
 md_color_todo=red
 md_background_color_todo=lightGrey
 md_color_coop1=black
 md_background_color_coop1=
```

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/settings_dialog.css` & `notolog-0.9.0b11/app/assets/themes/calligraphy/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/styles.css` & `notolog-0.9.0b11/app/assets/themes/calligraphy/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 body {
     max-width: 100%; /* Page not stretching upon resize without it */
     font-family: 'Arial', 'Liberation Sans', sans-serif;
+    line-height: 23px;
 }
 a { display: inline-block; }
 /* Fix new line issue within the p block */
 p { white-space: pre-line; }
 pre {
     /*display: block;
     white-space: pre;
@@ -91,23 +92,23 @@
     /*word-wrap: break-word;      Internet Explorer 5.5+ */
 }
 .codehilitetable { width: 100%; table-layout: fixed; border: none; border-spacing: unset; border-collapse: collapse;
     margin-top: 3px; }
 td.linenos { padding: 10px 7px 0; border-left: 3px dashed #333333; background: #000000; color: #ffffff;
     font-family: 'Arial', sans-serif; } /*  line-height: should be equal to td.code, code's line height to match */
 td.code, code { padding: 10px 10px 0; background: #555555; color: #ffffff;
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 td.linenos .normal { color: grey; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 div.linenodiv { padding: 0; margin: 0; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: inherit; background-color: #ffffff; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: inherit; background-color: #ffffff; padding-left: 5px; padding-right: 5px; }
 
 .codehilite { overflow-x: auto; line-height: 21px; /* 21px is a min value atm */
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 .codehilite .hll { background: transparent; }
 .codehilite .c { font-style: italic } /* Comment */
 .codehilite .err { border: 1px solid #FF0000 } /* Error */
 .codehilite .k { font-weight: bold } /* Keyword */
 .codehilite .ch { font-style: italic } /* Comment.Hashbang */
 .codehilite .cm { font-style: italic } /* Comment.Multiline */
 .codehilite .cpf { font-style: italic } /* Comment.PreprocFile */
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 body { max-width: 100%; /* Page not stretching upon resize without it */ font-
-family: 'Arial', 'Liberation Sans', sans-serif; } a { display: inline-block; }
-/* Fix new line issue within the p block */ p { white-space: pre-line; } pre
-{ /*display: block; white-space: pre; max-width: 100%; text-indent: 20px;
-margin: 10px;*/ } img { max-width: 100%; } a { color: red; } /* Somehow h5 and
-h6 are not balanced. Hence h6 adjusted in pt */ h1 { font-size: xx-large; } h2
-{ font-size: x-large; } h3 { font-size: large; } h4 { font-size: medium; } h5
-{ font-size: small; } h6 { font-size: 8pt; font-weight: bold; } /* Expandable
-block, which replaces the ...... with:
+family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
+{ display: inline-block; } /* Fix new line issue within the p block */ p
+{ white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
+100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
+red; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */ h1
+{ font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; } h4
+{ font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
+weight: bold; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
@@ -32,24 +32,24 @@
 -pre-wrap; Opera 4-6 */ /*white-space: -o-pre-wrap; Opera 7 */ /*word-wrap:
 break-word; Internet Explorer 5.5+ */ } .codehilitetable { width: 100%; table-
 layout: fixed; border: none; border-spacing: unset; border-collapse: collapse;
 margin-top: 3px; } td.linenos { padding: 10px 7px 0; border-left: 3px dashed
 #333333; background: #000000; color: #ffffff; font-family: 'Arial', sans-serif;
 } /* line-height: should be equal to td.code, code's line height to match */
 td.code, code { padding: 10px 10px 0; background: #555555; color: #ffffff;
-font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation
+font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation
 Mono', 'DejaVu Sans Mono', 'Courier New', monospace; } td.linenos .normal
 { color: grey; background-color: transparent; padding-left: 5px; padding-right:
 5px; } div.linenodiv { padding: 0; margin: 0; } span.linenos { color: inherit;
 background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: inherit; background-color: #ffffff; padding-left:
 5px; padding-right: 5px; } span.linenos.special { color: inherit; background-
 color: #ffffff; padding-left: 5px; padding-right: 5px; } .codehilite
 { overflow-x: auto; line-height: 21px; /* 21px is a min value atm */ font-
-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono',
+family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono',
 'DejaVu Sans Mono', 'Courier New', monospace; } .codehilite .hll { background:
 transparent; } .codehilite .c { font-style: italic } /* Comment */ .codehilite
 .err { border: 1px solid #FF0000 } /* Error */ .codehilite .k { font-weight:
 bold } /* Keyword */ .codehilite .ch { font-style: italic } /* Comment.Hashbang
 */ .codehilite .cm { font-style: italic } /* Comment.Multiline */ .codehilite
 .cpf { font-style: italic } /* Comment.PreprocFile */ .codehilite .c1 { font-
 style: italic } /* Comment.Single */ .codehilite .cs { font-style: italic } /
```

### Comparing `notolog-0.9.0b10/app/assets/themes/calligraphy/tree_view.css` & `notolog-0.9.0b11/app/assets/themes/calligraphy/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/about_popup.css` & `notolog-0.9.0b11/app/assets/themes/default/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/default.ini` & `notolog-0.9.0b11/app/assets/themes/default/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/LICENSE` & `notolog-0.9.0b11/app/assets/themes/default/icons/LICENSE`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/arrow-repeat.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/arrow-repeat.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/balloon-fill.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/balloon-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/balloon.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/balloon.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/bandaid-fill.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/bandaid-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/bandaid.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/bandaid.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up-right.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/box-arrow-up-right.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/box-arrow-up.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/box-arrow-up.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/cursor-text.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/cursor-text.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-html.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/filetype-html.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-md.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/filetype-md.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/filetype-txt.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/filetype-txt.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/floppy2.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/floppy2.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/folder-symlink.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/folder-symlink.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/folder.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/folder.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/github.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/github.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/link-45deg.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/link-45deg.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/linkedin.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/linkedin.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/pencil-square.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/pencil-square.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/quote.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/robot.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/robot.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock-fill.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/shield-lock-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/shield-lock.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/shield-lock.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/star.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/star.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/trash3-fill.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/trash3-fill.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/trash3.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/trash3.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/icons/type-strikethrough.svg` & `notolog-0.9.0b11/app/assets/themes/default/icons/type-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/md.ini` & `notolog-0.9.0b11/app/assets/themes/default/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/settings_dialog.css` & `notolog-0.9.0b11/app/assets/themes/default/settings_dialog.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/default/styles.css` & `notolog-0.9.0b11/app/assets/themes/default/styles.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 body {
     max-width: 100%; /* Page not stretching upon resize without it */
     font-family: 'Arial', 'Liberation Sans', sans-serif;
+    line-height: 23px;
 }
 a { display: inline-block; }
 /* Fix new line issue within the p block */
 p { white-space: pre-line; }
 pre {
     /*display: block;
     white-space: pre;
@@ -91,23 +92,23 @@
     /*word-wrap: break-word;      Internet Explorer 5.5+ */
 }
 .codehilitetable { width: 100%; table-layout: fixed; border: none; border-spacing: unset; border-collapse: collapse;
     margin-top: 3px; }
 td.linenos { padding: 10px 7px 0; border-left: 3px solid #eec357; background: #373737; color: #eeeeee;
     font-family: 'Arial', sans-serif; } /*  line-height: should be equal to td.code, code's line height to match */
 td.code, code { padding: 10px 10px 0; background: dimgrey; color: #f8f8f2;
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 td.linenos .normal { color: grey; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 div.linenodiv { padding: 0; margin: 0; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: inherit; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: inherit; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 
 .codehilite { overflow-x: auto; line-height: 21px; /* 21px is a min value atm */
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 .codehilite .hll { background-color: transparent; }
 .codehilite .c { color: #85816e } /* Comment */
 .codehilite .err { color: #960050; background-color: #1e0010 } /* Error */
 .codehilite .k { color: #66d9ef } /* Keyword */
 .codehilite .l { color: #ae81ff } /* Literal */
 .codehilite .n { color: #f8f8f2 } /* Name */
 .codehilite .o { color: #f92672 } /* Operator */
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 body { max-width: 100%; /* Page not stretching upon resize without it */ font-
-family: 'Arial', 'Liberation Sans', sans-serif; } a { display: inline-block; }
-/* Fix new line issue within the p block */ p { white-space: pre-line; } pre
-{ /*display: block; white-space: pre; max-width: 100%; text-indent: 20px;
-margin: 10px;*/ } img { max-width: 100%; } a { color: royalblue; } /* Somehow
-h5 and h6 are not balanced. Hence h6 adjusted in pt */ h1 { font-size: xx-
-large; } h2 { font-size: x-large; } h3 { font-size: large; } h4 { font-size:
-medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-weight: bold; } /
-* Expandable block, which replaces the ...... with:
+family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
+{ display: inline-block; } /* Fix new line issue within the p block */ p
+{ white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
+100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
+royalblue; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */
+h1 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; }
+h4 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
+weight: bold; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
@@ -32,24 +32,24 @@
 /*white-space: -pre-wrap; Opera 4-6 */ /*white-space: -o-pre-wrap; Opera 7 */ /
 *word-wrap: break-word; Internet Explorer 5.5+ */ } .codehilitetable { width:
 100%; table-layout: fixed; border: none; border-spacing: unset; border-
 collapse: collapse; margin-top: 3px; } td.linenos { padding: 10px 7px 0;
 border-left: 3px solid #eec357; background: #373737; color: #eeeeee; font-
 family: 'Arial', sans-serif; } /* line-height: should be equal to td.code,
 code's line height to match */ td.code, code { padding: 10px 10px 0;
-background: dimgrey; color: #f8f8f2; font-family: 'Consolas', 'Menlo',
-'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier
+background: dimgrey; color: #f8f8f2; font-family: 'Menlo', 'Monaco',
+'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier
 New', monospace; } td.linenos .normal { color: grey; background-color:
 transparent; padding-left: 5px; padding-right: 5px; } div.linenodiv { padding:
 0; margin: 0; } span.linenos { color: inherit; background-color: transparent;
 padding-left: 5px; padding-right: 5px; } td.linenos .special { color: inherit;
 background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: inherit; background-color: #ffffc0; padding-left:
 5px; padding-right: 5px; } .codehilite { overflow-x: auto; line-height: 21px; /
-* 21px is a min value atm */ font-family: 'Consolas', 'Menlo', 'Monaco',
+* 21px is a min value atm */ font-family: 'Menlo', 'Monaco', 'Consolas',
 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New',
 monospace; } .codehilite .hll { background-color: transparent; } .codehilite .c
 { color: #85816e } /* Comment */ .codehilite .err { color: #960050; background-
 color: #1e0010 } /* Error */ .codehilite .k { color: #66d9ef } /* Keyword */
 .codehilite .l { color: #ae81ff } /* Literal */ .codehilite .n { color: #f8f8f2
 } /* Name */ .codehilite .o { color: #f92672 } /* Operator */ .codehilite .p
 { color: #f8f8f2 } /* Punctuation */ .codehilite .ch { color: #85816e } /
```

### Comparing `notolog-0.9.0b10/app/assets/themes/default/tree_view.css` & `notolog-0.9.0b11/app/assets/themes/default/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/about_popup.css` & `notolog-0.9.0b11/app/assets/themes/noir_dark/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/default.ini` & `notolog-0.9.0b11/app/assets/themes/noir_dark/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/md.ini` & `notolog-0.9.0b11/app/assets/themes/noir_dark/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/settings_dialog.css` & `notolog-0.9.0b11/app/assets/themes/noir_dark/settings_dialog.css`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,19 @@
     color: lightgray;
 }
 /* Active tab */
 QTabBar::tab:selected {
     color: red;
 }
 QComboBox {}
+QComboBox::separator {
+    height: 1px;
+    background: #555555;
+}
+/*QComboBox::down-arrow { top: 1px; }*/
 QLabel {
     color: #eeeeee;
 }
 QLineEdit {
     color: #eeeeee;
 }
 /* Group titles */
```

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/styles.css` & `notolog-0.9.0b11/app/assets/themes/noir_dark/styles.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 body {
     max-width: 100%; /* Page not stretching upon resize without it */
     font-family: 'Arial', 'Liberation Sans', sans-serif;
+    line-height: 23px;
 }
 a { display: inline-block; }
 /* Fix new line issue within the p block */
 p { white-space: pre-line; }
 pre {
     /*display: block;
     white-space: pre;
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 body { max-width: 100%; /* Page not stretching upon resize without it */ font-
-family: 'Arial', 'Liberation Sans', sans-serif; } a { display: inline-block; }
-/* Fix new line issue within the p block */ p { white-space: pre-line; } pre
-{ /*display: block; white-space: pre; max-width: 100%; text-indent: 20px;
-margin: 10px;*/ } img { max-width: 100%; } a { color: red; } /* Somehow h5 and
-h6 are not balanced. Hence h6 adjusted in pt */ h1 { font-size: xx-large; } h2
-{ font-size: x-large; } h3 { font-size: large; } h4 { font-size: medium; } h5
-{ font-size: small; } h6 { font-size: 8pt; font-weight: bold; } /* Expandable
-block, which replaces the ...... with:
+family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
+{ display: inline-block; } /* Fix new line issue within the p block */ p
+{ white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
+100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
+red; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */ h1
+{ font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; } h4
+{ font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
+weight: bold; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: whitesmoke; text-decoration: none; font-weight: bold;
```

### Comparing `notolog-0.9.0b10/app/assets/themes/noir_dark/tree_view.css` & `notolog-0.9.0b11/app/assets/themes/noir_dark/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/about_popup.css` & `notolog-0.9.0b11/app/assets/themes/strawberry/about_popup.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/default.ini` & `notolog-0.9.0b11/app/assets/themes/strawberry/default.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/md.ini` & `notolog-0.9.0b11/app/assets/themes/strawberry/md.ini`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/settings_dialog.css` & `notolog-0.9.0b11/app/assets/themes/strawberry/settings_dialog.css`

 * *Files 8% similar despite different names*

```diff
@@ -19,8 +19,10 @@
     color: gray;
 }
 QCheckBox {}
 /* Custom slider (no ticks color supported) */
 QSlider::groove:horizontal {}
 QSlider::handle:horizontal {}
 /* Request submit button */
-QPushButton#settings_dialog_button_close {}
+QPushButton#settings_dialog_button_close {
+    background-color: crimson;
+}
```

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/styles.css` & `notolog-0.9.0b11/app/assets/themes/strawberry/styles.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 body {
     max-width: 100%; /* Page not stretching upon resize without it */
     font-family: 'Arial', 'Liberation Sans', sans-serif;
+    line-height: 23px;
 }
 a { display: inline-block; }
 /* Fix new line issue within the p block */
 p { white-space: pre-line; }
 pre {
     /*display: block;
     white-space: pre;
@@ -91,23 +92,23 @@
     /*word-wrap: break-word;      Internet Explorer 5.5+ */
 }
 .codehilitetable { width: 100%; border: none; border-spacing: unset; border-collapse: collapse;
     margin-top: 3px; }
 td.linenos { padding: 10px 7px 0; border-left: 3px solid salmon; background: #373737; color: #eeeeee;
     font-family: 'Arial', sans-serif; } /*  line-height: should be equal to td.code, code's line height to match */
 td.code, code { padding: 10px 10px 0; background: #a1426d; color: #f8f8f2;
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 td.linenos .normal { color: grey; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 div.linenodiv { padding: 0; margin: 0; }
 span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: inherit; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 span.linenos.special { color: inherit; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
 
 .codehilite { overflow-x: auto; line-height: 21px; /* 21px is a min value atm */
-    font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
+    font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono', 'DejaVu Sans Mono', 'Courier New', monospace; }
 .codehilite .hll { background-color: #49483e; }
 .codehilite .c { color: lightpink } /* Comment */
 .codehilite .err { color: darkred; background-color: palevioletred; } /* Error */
 .codehilite .k { color: #66d9ef } /* Keyword */
 .codehilite .l { color: #db81ff
 } /* Literal */
 .codehilite .n { color: #f8f8f2 } /* Name */
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 body { max-width: 100%; /* Page not stretching upon resize without it */ font-
-family: 'Arial', 'Liberation Sans', sans-serif; } a { display: inline-block; }
-/* Fix new line issue within the p block */ p { white-space: pre-line; } pre
-{ /*display: block; white-space: pre; max-width: 100%; text-indent: 20px;
-margin: 10px;*/ } img { max-width: 100%; } a { color: deeppink; } /* Somehow h5
-and h6 are not balanced. Hence h6 adjusted in pt */ h1 { font-size: xx-large; }
-h2 { font-size: x-large; } h3 { font-size: large; } h4 { font-size: medium; }
-h5 { font-size: small; } h6 { font-size: 8pt; font-weight: bold; } /
-* Expandable block, which replaces the ...... with:
+family: 'Arial', 'Liberation Sans', sans-serif; line-height: 23px; } a
+{ display: inline-block; } /* Fix new line issue within the p block */ p
+{ white-space: pre-line; } pre { /*display: block; white-space: pre; max-width:
+100%; text-indent: 20px; margin: 10px;*/ } img { max-width: 100%; } a { color:
+deeppink; } /* Somehow h5 and h6 are not balanced. Hence h6 adjusted in pt */
+h1 { font-size: xx-large; } h2 { font-size: x-large; } h3 { font-size: large; }
+h4 { font-size: medium; } h5 { font-size: small; } h6 { font-size: 8pt; font-
+weight: bold; } /* Expandable block, which replaces the ...... with:
 _â__¼_{_}
 */ /* Expanded block (collapsible), which appears after expandable block click:
 {}
 {}
 */ /* anchor details-summary common */ ._ds_expand { border: 1px solid grey
 !important; background: transparent; } /* anchor details-summary expandable */
 ._ds_expand > a { color: black; text-decoration: none; font-weight: bold; }
@@ -32,24 +32,24 @@
 /*white-space: -pre-wrap; Opera 4-6 */ /*white-space: -o-pre-wrap; Opera 7 */ /
 *word-wrap: break-word; Internet Explorer 5.5+ */ } .codehilitetable { width:
 100%; border: none; border-spacing: unset; border-collapse: collapse; margin-
 top: 3px; } td.linenos { padding: 10px 7px 0; border-left: 3px solid salmon;
 background: #373737; color: #eeeeee; font-family: 'Arial', sans-serif; } /
 * line-height: should be equal to td.code, code's line height to match */
 td.code, code { padding: 10px 10px 0; background: #a1426d; color: #f8f8f2;
-font-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation
+font-family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation
 Mono', 'DejaVu Sans Mono', 'Courier New', monospace; } td.linenos .normal
 { color: grey; background-color: transparent; padding-left: 5px; padding-right:
 5px; } div.linenodiv { padding: 0; margin: 0; } span.linenos { color: inherit;
 background-color: transparent; padding-left: 5px; padding-right: 5px; }
 td.linenos .special { color: inherit; background-color: #ffffc0; padding-left:
 5px; padding-right: 5px; } span.linenos.special { color: inherit; background-
 color: #ffffc0; padding-left: 5px; padding-right: 5px; } .codehilite
 { overflow-x: auto; line-height: 21px; /* 21px is a min value atm */ font-
-family: 'Consolas', 'Menlo', 'Monaco', 'Lucida Console', 'Liberation Mono',
+family: 'Menlo', 'Monaco', 'Consolas', 'Lucida Console', 'Liberation Mono',
 'DejaVu Sans Mono', 'Courier New', monospace; } .codehilite .hll { background-
 color: #49483e; } .codehilite .c { color: lightpink } /* Comment */ .codehilite
 .err { color: darkred; background-color: palevioletred; } /* Error */
 .codehilite .k { color: #66d9ef } /* Keyword */ .codehilite .l { color: #db81ff
 } /* Literal */ .codehilite .n { color: #f8f8f2 } /* Name */ .codehilite .o
 { color: #ff005c } /* Operator */ .codehilite .p { color: #f8f8f2 } /
 * Punctuation */ .codehilite .ch { color: lightpink } /* Comment.Hashbang */
```

### Comparing `notolog-0.9.0b10/app/assets/themes/strawberry/tree_view.css` & `notolog-0.9.0b11/app/assets/themes/strawberry/tree_view.css`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/edit_widget.py` & `notolog-0.9.0b11/app/edit_widget.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/editor_state.py` & `notolog-0.9.0b11/app/editor_state.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_helper.py` & `notolog-0.9.0b11/app/encrypt/enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_new_password_dialog.py` & `notolog-0.9.0b11/app/encrypt/enc_new_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password.py` & `notolog-0.9.0b11/app/encrypt/enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password_dialog.py` & `notolog-0.9.0b11/app/encrypt/enc_password_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/encrypt/enc_password_reset_dialog.py` & `notolog-0.9.0b11/app/encrypt/enc_password_reset_dialog.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox
+from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox, QSizePolicy
 from PySide6.QtGui import QFontMetrics
 
 from typing import Optional, Callable, Any
 
 from ..settings import Settings
 from ..app_config import AppConfig
 from ..lexemes.lexemes import Lexemes
@@ -32,15 +32,16 @@
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         title = self.lexemes.get('dialog_encrypt_password_reset_title')
         self.setWindowTitle(title)
         self.setObjectName('dialog_encrypt_password_reset_title')
 
-        self.resize(256, 96)
+        # Adjust dialog size
+        self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
         if self.sizeHint().isValid():
             self.setMinimumSize(self.sizeHint())
 
         label = QLabel()
         label.setObjectName('dialog_encrypt_password_reset_text')
         label.setText(self.lexemes.get('dialog_encrypt_password_reset_text'))
         label.setAlignment(Qt.AlignmentFlag.AlignCenter)
```

### Comparing `notolog-0.9.0b10/app/enums/ai_model_names.py` & `notolog-0.9.0b11/app/enums/ai_model_names.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/colors.py` & `notolog-0.9.0b11/app/enums/colors.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/enums/languages.py` & `notolog-0.9.0b11/app/enums/languages.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 
 class Languages(Enum):
 
     # Override _generate_next_value_ to allow for custom attributes on enum members (mostly for default).
     def _generate_next_value_(name, start, count, last_values):
         return name, False  # The second value in the tuple is the custom attribute indicating whether it's the default
 
+    DE = "German"
     EN = ("English", True)
+    ES = "Spanish"
     FR = "French"
-    DE = "German"
     GE = "Georgian"
+    GR = "Greek"
+    IN = "Hindi"
     IT = "Italian"
     JA = "Japanese"
     KO = "Korean"
+    LA = "Latin"
     PT = "Portuguese"
     RU = "Russian"
-    ES = "Spanish"
-    LA = "Latin"
+    TR = "Turkish"
     ZH = "Chinese"
 
     def __init__(self, value, is_default=False):
         self._value_ = value
         self.is_default = is_default
 
     def __str__(self):
```

### Comparing `notolog-0.9.0b10/app/enums/themes.py` & `notolog-0.9.0b11/app/enums/themes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/etree_extension.py` & `notolog-0.9.0b11/app/etree_extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,67 +12,73 @@
 class ElementTreeExtension(Extension):
     """
     Custom markdown extension
     """
 
     logger = logging.getLogger('tree_extension')
 
+    logging = AppConfig.get_logging()
     debug = AppConfig.get_debug()
 
     def extendMarkdown(self, md: Markdown) -> None:
         if self.debug:
             self.logger.info('%s extension engaged' % self . __class__ . __qualname__)
 
         md.registerExtension(self)
-        md.treeprocessors.register(ElementTreeProcessor(md), 'custom', 1)
+        # noinspection SpellCheckingInspection
+        md.treeprocessors.register(ElementTreeProcessor(md), 'notolog_extension', 1)
 
 
 class ElementTreeProcessor(Treeprocessor):
     """
     Custom markdown extension processor
     """
 
     logger = logging.getLogger('tree_processor')
 
+    logging = AppConfig.get_logging()
     debug = AppConfig.get_debug()
 
     def run(self, root):
         # Customize elements tree here
         for idx, elem in enumerate(root.iter()):
             if self.debug:
-                self.logger.info('%s > %d: %s' % (self . __class__ . __qualname__, idx, elem.tag))
+                self.logger.debug('%s > %d: %s' % (self . __class__ . __qualname__, idx, elem.tag))
+            # noinspection SpellCheckingInspection
             """
             Works when `codehilite` is switched off:
             if elem.tag == 'pre':
-                for idxy, celem in enumerate(elem):
-                    if celem.tag == 'code':
-                        celem.set('style', 'background-color: #373737; color: #f5f5f5; padding: 10px;')
+                for id_xy, c_elem in enumerate(elem):
+                    if c_elem.tag == 'code':
+                        c_elem.set('style', 'background-color: #373737; color: #f5f5f5; padding: 10px;')
             """
+            # if elem.tag == 'img':
+            #    elem.set('title', '...')
+            #    elem.set('onerror', "this.onerror=null;this.src='app/assets/themes/default/icons/...';")
             if elem.tag == 'p' and len(elem) > 0:
-                for idxy, celem in enumerate(elem):
+                for id_xy, c_elem in enumerate(elem):
                     if self.debug:
-                        self.logger.info('%s > Inner element > %d: %s'
-                                         % (self . __class__ . __qualname__, idxy, celem.tag))
+                        self.logger.debug('%s > Inner element > %d: %s'
+                                          % (self . __class__ . __qualname__, id_xy, c_elem.tag))
                     # Example of how to update elements tree
-                    if celem.tag == 'a' and False:
+                    if c_elem.tag == 'a' and False:
                         # Skip element that was already re-inserted
-                        if celem.get('class') == '_re-inserted':
+                        if c_elem.get('class') == '_re-inserted':
                             continue
                         # Add break space before the element
-                        br_str = "<hr/>"
+                        br_str = "<br/>"
                         br_elem = ElementTree.fromstring(br_str)
                         # Remove `a` element
-                        elem.remove(celem)
+                        elem.remove(c_elem)
                         # Insert `br` element
-                        elem.insert(idxy, br_elem)
+                        elem.insert(id_xy, br_elem)
                         # Setup class as a flag to determine re-inserted `a` element
-                        celem.set('class', '_re-inserted')
+                        c_elem.set('class', '_re-inserted')
                         # Re-insert the `a` element with a new class
-                        elem.insert(idxy + 1, celem)
+                        elem.insert(id_xy + 1, c_elem)
 
     def get_index(self, root, element):
         for idx, child in enumerate(root):
             if element == child:
                 return idx
         else:
-            raise ValueError("No inner '%s' tag found in '%s'" %
-                 (element.tag, root.tag))
+            raise ValueError("No inner '%s' tag found in '%s'" % (element.tag, root.tag))
```

### Comparing `notolog-0.9.0b10/app/file_header.py` & `notolog-0.9.0b11/app/file_header.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,25 +136,32 @@
             raise FileHeaderEmptyException()
 
     def pack(self, content: str = None, encode: bool = False) -> str:
         header_line = repr(self)
         delimiter = '\n'
 
         if encode:
-            delimiter = delimiter.encode()
+            delimiter = delimiter.encode("utf-8")
             if header_line and type(header_line) is not bytes:
-                header_line = header_line.encode()
-            if content and type(content) is not bytes:
-                content = content.encode()
+                header_line = header_line.encode("utf-8")
+            if content is not None and type(content) is not bytes:
+                content = content.encode("utf-8")
 
-        if header_line and content:
+        if header_line and content is not None:
+            # Return header and content, even if the content is empty
             return header_line + delimiter + content
-        elif content:
+        elif content is not None:
+            if self.logging:
+                self.logger.warning(f'File content exist but header is None {self}')
+            # Return content without header
             return content
         else:
+            if self.logging:
+                self.logger.warning(f'File header exist but content is None {self}')
+            # Return header without content
             return header_line
 
     def load_file(self, file_path: str) -> tuple[Any, str]:
         file_data = read_file(file_path)
         return self.load(file_data)
 
     def load(self, file_data: str) -> tuple[Any, str]:
```

### Comparing `notolog-0.9.0b10/app/file_system_watcher.py` & `notolog-0.9.0b11/app/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/file_helper.py` & `notolog-0.9.0b11/app/helpers/file_helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from PySide6.QtCore import QFile, QDir
 
 import os
 import sys
 
 from typing import Union
 
+
 def res_path(rel_path):
     # Get absolute path for resources which works either for dev and for build
     try:
         # PyInstaller creates a temporary folder and store its path in _MEIPASS
         base_path = sys._MEIPASS
     except Exception:
         # base_path = os.path.abspath(".")
         base_path = os.path.abspath(QDir.currentPath())
 
     return os.path.join(base_path, rel_path)
 
+
 def size_f(size: int, suffix: str="B") -> str:
     """
     Human-readable file/content size
     @param size: size in bytes
     @param suffix: suffix at the end of the formatted string
     @return: formatted string of file size
     """
@@ -31,42 +33,51 @@
     unit_size = 1024.0
     i = 0
     while abs(size) >= unit_size and i < len(units) - 1:
         size /= unit_size
         i += 1
     return f"{round(size, 1)}{units[i]}{suffix}"
 
+
 def read_file(file_path: str, b: bool=False) -> Union[str, bytearray]:
     """
     Read file content
     @param file_path: file path string
     @param b: as a bytearray
     @return: file content either as a string, bytearray or None
+
+    # Qt implementation could be like
+    file = QFile(file_path)
+    if file.open(QIODevice.OpenModeFlag.ReadOnly):
+        # file.size()
+        return file.readAll()
     """
     # a bytes-like object or string
     mode = 'rb' if b else 'r'
     # without 3-char extension: file_path[:-4]
-    with open(file_path, mode, encoding='utf-8') as file:
+    with open(file_path, mode) if b else open(file_path, mode, encoding='utf-8') as file:  # No encoding in bin mode
         return file.read()
 
+
 def save_file(file_path: str, data: Union[str, bytearray], b: bool=False) -> bool:
     """
     Save content to the file
     @param file_path: file path string
     @param data: file content either as a string or bytearray
     @param b: as a bytearray
     @return: boolean result
     """
     # a bytes-like object or string
     mode = 'wb' if b else 'w'
     # without 3-char extension: crypted_file_path[:-4]
-    with open(file_path, mode, encoding='utf-8') as file:
+    with open(file_path, mode) if b else open(file_path, mode, encoding='utf-8') as file:  # No encoding in bin mode
         file.write(data)
         return True
 
+
 def remove_trailing_numbers(text) -> str:
     """
     Remove trailing numbers from text, mostly file extension with incremental digital addon.
     @param text: text to remove trailing digits from
     @return: string without trailing digits if they are exist
     """
     # Start from the end of the string and find the first non-digit character
```

### Comparing `notolog-0.9.0b10/app/helpers/theme_helper.py` & `notolog-0.9.0b11/app/helpers/theme_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/tooltip_helper.py` & `notolog-0.9.0b11/app/helpers/tooltip_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/helpers/update_helper.py` & `notolog-0.9.0b11/app/helpers/update_helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PySide6.QtCore import QObject, Signal, Slot, QUrl, QByteArray
-from PySide6.QtNetwork import QNetworkAccessManager, QNetworkRequest, QNetworkReply
+from PySide6.QtNetwork import QNetworkAccessManager, QNetworkRequest, QNetworkReply, QSslSocket
 
 from packaging import version
 
 import json
 import logging
 
 from ..settings import Settings
@@ -33,14 +33,17 @@
         self.settings = Settings(parent=self)
 
         self.logger = logging.getLogger('update_helper')
 
         self.logging = AppConfig.get_logging()
         self.debug = AppConfig.get_debug()
 
+        if self.logging:
+            self.logger.info("SSL supported: %s" % QSslSocket.supportsSsl())
+
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='common')
 
         self.current_version = version.parse(AppConfig.get_app_version())
 
         self.manager = QNetworkAccessManager(self)
 
@@ -58,15 +61,15 @@
         reply.finished.connect(lambda _reply=reply: self.handle_network_reply(_reply))
         # Connect error signal
         reply.errorOccurred.connect(lambda error, _reply=reply: self.handle_network_reply(_reply, error))
 
     @Slot()
     def handle_network_reply(self, reply: QNetworkReply, error_code=None):
         # Get received status code, say 200
-        status_code = reply.attribute(QNetworkRequest.HttpStatusCodeAttribute)
+        status_code = reply.attribute(QNetworkRequest.Attribute.HttpStatusCodeAttribute)
 
         if self.debug:
             self.logger.debug(f'Update response, reply: {reply}, error_code: {error_code}, status_code: {status_code}')
 
         reply.deleteLater()  # Clean up the QNetworkReply object
 
         # Make sure there is no error
@@ -103,16 +106,17 @@
                 if self.debug:
                     self.logger.debug(f"Result JSON: {json_data}")
 
                 latest_version_str = json_data['tag_name']
                 latest_version = version.parse(latest_version_str)
 
                 if latest_version > self.current_version:
+                    update_link = '<a href="%s">%s</a>' % (AppConfig.get_repository_github_release_url(), latest_version)
                     result_message = self.lexemes.get('update_helper_new_version_is_available',
-                                                      latest_version=latest_version)
+                                                      latest_version=update_link)
                     if self.logging:
                         self.logger.info("New version of the app is available: %s. Current version is %s. Response: %s}"
                                          % (latest_version, self.current_version, reply.errorString()))
                     # Emit the new version signal
                     self.new_version_check_response.emit(
                         {'status': self.STATUS_OK, 'msg': result_message,
                          'current_version': self.current_version,
```

### Comparing `notolog-0.9.0b10/app/highlight/main_highlighter.py` & `notolog-0.9.0b11/app/highlight/main_highlighter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+# Notolog
+# An open-source markdown editor written in Python.
+
+# Base Syntax Highlighter class tailored for Notolog
+
+"""
+This module contains shared functionality for subclasses like the MdHighlighter.
+"""
+
+# - GitHub Repository: https://github.com/notolog/notolog-editor
+# - PyPI: https://pypi.org/project/notolog
+# - WebSite: https://notolog.app
+# - Author: Vadim Bakhrenkov
+# - Copyright 2024 Vadim Bakhrenkov
+# - License: MIT License
+
 from PySide6.QtCore import Qt, QRegularExpression
 from PySide6.QtGui import QTextDocument, QSyntaxHighlighter, QTextBlockUserData, QTextBlock, QTextCharFormat
 from PySide6.QtGui import QColor, QBrush, QFont
 
 from typing import Union
 
-from ..app_config import AppConfig
-from ..text_block_data import TextBlockData
-from ..helpers.theme_helper import ThemeHelper
+from . import AppConfig
+from . import TextBlockData
+from . import ThemeHelper
 
 import logging
 
 
 class MainHighlighter(QSyntaxHighlighter):
     """
     Syntax highlighter class
@@ -130,21 +146,21 @@
         if color:
             color_obj = QColor()
             color_obj.setNamedColor(color)
             cformat.setForeground(color_obj)
 
         # Background
         if bg:
-            bg_color = None
+            bg_color = None  # type: Union[str, None]
             """
             Qt::BrushStyle https://doc.qt.io/qt-6/qt.html#BrushStyle-enum
             """
             bg_pattern = Qt.BrushStyle.SolidPattern
             if type(bg) is str:
-                bg_color = bg
+                bg_color = bg  # type: ignore
             elif type(bg) is dict:
                 if 'color' in bg:
                     bg_color = bg['color']
                 if 'pattern' in bg and bg['pattern'] in Qt.BrushStyle:
                     bg_pattern = bg['pattern']
             # Color required
             if bg_color is not None:
```

### Comparing `notolog-0.9.0b10/app/highlight/md_highlighter.py` & `notolog-0.9.0b11/app/highlight/md_highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,33 @@
+# Notolog
+# An open-source markdown editor written in Python.
+
+# Markdown Syntax Highlighter class tailored for Notolog
+
+"""
+This module combines regular expression patterns with integrated code logic. This approach provides a balanced result
+and reduces reliance on complex regular expressions as much as possible. It particularly aids in processing multiline
+blocks, such as code blocks, where stability in detection is crucial for accurate visual representation. Avoiding
+precise detection may lead to "blinking highlighting." While the author has attempted to cover most cases, the primary
+goal was to meet the common needs expected from a markdown editor.
+
+This module may be subject to changes in future releases. Currently, it serves more as a proof of concept.
+"""
+
+# - GitHub Repository: https://github.com/notolog/notolog-editor
+# - PyPI: https://pypi.org/project/notolog
+# - WebSite: https://notolog.app
+# - Author: Vadim Bakhrenkov
+# - Copyright 2024 Vadim Bakhrenkov
+# - License: MIT License
+
 from PySide6.QtCore import Qt
 
 from .main_highlighter import MainHighlighter
-from ..text_block_data import TextBlockData
+from . import TextBlockData
 
 import re
 
 
 class MdHighlighter(MainHighlighter):
     """
     Syntax highlighter class for the Markdown language
```

### Comparing `notolog-0.9.0b10/app/highlight/view_highlighter.py` & `notolog-0.9.0b11/app/highlight/view_highlighter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+# Notolog
+# An open-source markdown editor written in Python.
+
+# View mode Syntax Highlighter class tailored for Notolog
+
+"""
+This module includes functionality specifically needed for view mode, such as detecting strikethrough and todo elements.
+"""
+
+# - GitHub Repository: https://github.com/notolog/notolog-editor
+# - PyPI: https://pypi.org/project/notolog
+# - WebSite: https://notolog.app
+# - Author: Vadim Bakhrenkov
+# - Copyright 2024 Vadim Bakhrenkov
+# - License: MIT License
+
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QTextBlock
 
 from .main_highlighter import MainHighlighter
-from ..text_block_data import TextBlockData
+from . import TextBlockData
 
 from typing import Match
 
 import re
 
 
 class ViewHighlighter(MainHighlighter):
```

### Comparing `notolog-0.9.0b10/app/lexemes/__pycache__/lexemes.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/__pycache__/lexemes.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 3739 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 9b0e 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 9b0e 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 6d06 5a06 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000060: 8302 5a07 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2902 da05 556e 696f 6eda 0444 6963 7463  )...Union..Dictc
@@ -31,15 +31,15 @@
 000001e0: 720a 0000 00da 076c 6f67 6769 6e67 da09  r......logging..
 000001f0: 6765 744c 6f67 6765 72da 066c 6f67 6765  getLogger..logge
 00000200: 72da 0c6c 6f61 645f 6c65 7865 6d65 7329  r..load_lexemes)
 00000210: 03da 0473 656c 6672 0700 0000 7208 0000  ...selfr....r...
 00000220: 00a9 0072 1100 0000 fa41 2f55 7365 7273  ...r.....A/Users
 00000230: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
 00000240: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-00000250: 2f6e 6f74 6f6c 6f67 2f6c 6578 656d 6573  /notolog/lexemes
+00000250: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
 00000260: 2f6c 6578 656d 6573 2e70 79da 085f 5f69  /lexemes.py..__i
 00000270: 6e69 745f 5f09 0000 0073 0e00 0000 0001  nit__....s......
 00000280: 0c01 0402 0601 0603 0602 0c02 7a10 4c65  ............z.Le
 00000290: 7865 6d65 732e 5f5f 696e 6974 5f5f 6301  xemes.__init__c.
 000002a0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
 000002b0: 0000 0043 0000 0073 1800 0000 7400 6a01  ...C...s....t.j.
 000002c0: a002 7400 6a01 a003 7404 a101 7c00 6a05  ..t.j...t...|.j.
@@ -147,15 +147,15 @@
 00000920: 0cda 1167 6574 5f64 6566 6175 6c74 5f73  ...get_default_s
 00000930: 636f 7065 720a 0000 00da 0367 6574 da0a  coper......get..
 00000940: 6973 696e 7374 616e 6365 da05 6279 7465  isinstance..byte
 00000950: 73da 0664 6563 6f64 65da 0666 6f72 6d61  s..decode..forma
 00000960: 74da 084b 6579 4572 726f 7272 0e00 0000  t..KeyErrorr....
 00000970: da07 7761 726e 696e 6772 1700 0000 da04  ..warningr......
 00000980: 6b65 7973 2905 7210 0000 00da 046e 616d  keys).r......nam
-00000990: 6572 2f00 0000 da06 6b77 6172 6773 da06  er/.....kwargs..
+00000990: 6572 2f00 0000 da06 6b77 6172 6773 5a06  er/.....kwargsZ.
 000009a0: 6c65 7865 6d65 7211 0000 0072 1100 0000  lexemer....r....
 000009b0: 7212 0000 0072 3200 0000 3c00 0000 731a  r....r2...<...s.
 000009c0: 0000 0000 0704 0208 0220 010a 010a 0204  ......... ......
 000009d0: 0202 0114 010c 0108 0110 ff0c 027a 0b4c  .............z.L
 000009e0: 6578 656d 6573 2e67 6574 6301 0000 0000  exemes.getc.....
 000009f0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
 00000a00: 0000 0073 0600 0000 7c00 6a00 5300 7214  ...s....|.j.S.r.
@@ -184,16 +184,16 @@
 00000b70: 0802 7a14 4c65 7865 6d65 732e 6765 745f  ..z.Lexemes.get_
 00000b80: 6675 6c6c 5f6b 6579 2902 7205 0000 0072  full_key).r....r
 00000b90: 0600 0000 2901 4e29 014e 290e da08 5f5f  ....).N).N)...__
 00000ba0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
 00000bb0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
 00000bc0: da03 7374 7272 1300 0000 721b 0000 0072  ..strr....r....r
 00000bd0: 0300 0000 720f 0000 0072 2e00 0000 7202  ....r....r....r.
-00000be0: 0000 0072 3200 0000 723d 0000 0072 3100  ...r2...r=...r1.
-00000bf0: 0000 723f 0000 0072 1100 0000 7211 0000  ..r?...r....r...
+00000be0: 0000 0072 3200 0000 723c 0000 0072 3100  ...r2...r<...r1.
+00000bf0: 0000 723e 0000 0072 1100 0000 7211 0000  ..r>...r....r...
 00000c00: 0072 1100 0000 7212 0000 0072 0400 0000  .r....r....r....
 00000c10: 0800 0000 7310 0000 0008 0112 0e08 0316  ....s...........
 00000c20: 1910 091a 1808 0408 0b72 0400 0000 2908  .........r....).
 00000c30: 7215 0000 00da 0e69 6d70 6f72 746c 6962  r......importlib
 00000c40: 2e75 7469 6c72 2300 0000 720c 0000 00da  .utilr#...r.....
 00000c50: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
 00000c60: 0072 0400 0000 7211 0000 0072 1100 0000  .r....r....r....
```

### Comparing `notolog-0.9.0b10/app/lexemes/de/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/de/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/de/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/common.py` & `notolog-0.9.0b11/app/lexemes/de/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Anwendungsinfo",
     "popup_about_app_name_description": "Markdown Editor",
 
     "popup_about_version": "Version",
     "popup_about_license": "Lizenz",
     "popup_about_website": "Webseite",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Datum",
 
     "update_helper_new_version_is_available": "Eine neue Version '{latest_version}' der App ist verfügbar",
     "update_helper_latest_version_installed": "Die neueste Version der App ist installiert",
 
     "network_connection_error_empty": "Antwortinformationen können nicht abgerufen werden",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/de/main_menu.py` & `notolog-0.9.0b11/app/lexemes/de/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/de/settings_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     "viewer_config_process_emojis_checkbox": "Text-Emojis in Grafiken umwandeln",
     "viewer_config_process_emojis_checkbox_accessible_description": "Text-Emojis in grafische Darstellungen umwandeln",
     "viewer_config_highlight_todos_checkbox": "TODOs hervorheben",
     "viewer_config_highlight_todos_checkbox_accessible_description": "TODOs im Text hervorheben",
     "viewer_config_open_link_confirmation_checkbox": "Bestätigung vor dem Öffnen von Links erforderlich",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "Vor dem Öffnen von Links eine Bestätigung anfordern",
+    "viewer_config_save_resources_checkbox": "Externe Bilder automatisch auf Festplatte speichern",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Speichert automatisch Kopien von externen Bildern auf der Festplatte für den Offline-Zugriff.",
 
     "ai_config_openai_api_label": "OpenAI-API",
     "ai_config_openai_api_url_input_placeholder_text": "API-URL",
     "ai_config_openai_api_url_input_accessible_description": "URL der OpenAI-API",
     "ai_config_openai_api_key_input_placeholder_text": "API-Schlüssel",
     "ai_config_openai_api_key_input_accessible_description": "API-Schlüssel von OpenAI",
     "ai_config_openai_api_supported_models_label": "Unterstützte Modelle",
```

### Comparing `notolog-0.9.0b10/app/lexemes/de/statusbar.py` & `notolog-0.9.0b11/app/lexemes/de/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/de/toolbar.py` & `notolog-0.9.0b11/app/lexemes/de/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/ai_assistant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 827 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 3b03 0000  a.......(..f;...
+00000000: 610d 0d0a 0000 0000 020f 3066 3b03 0000  a.........0f;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 9c0c 5a00 640d 5300  d.d.d.d...Z.d.S.
 00000050: 290e 7a0d 5265 7175 6573 7420 746f 2041  ).z.Request to A
 00000060: 495a 0752 6571 7565 7374 7a33 496e 7075  IZ.Requestz3Inpu
 00000070: 7420 7265 7175 6573 7420 746f 2067 6976  t request to giv
@@ -35,22 +35,22 @@
 00000220: 7265 7370 6f6e 7365 5f6f 7574 7075 745f  response_output_
 00000230: 6e6f 7469 6365 5f65 6d70 7479 5f74 6578  notice_empty_tex
 00000240: 74da 1864 6961 6c6f 675f 7573 6167 655f  t..dialog_usage_
 00000250: 6d6f 6465 6c5f 6c61 6265 6cda 1964 6961  model_label..dia
 00000260: 6c6f 675f 7573 6167 655f 746f 6b65 6e73  log_usage_tokens
 00000270: 5f6c 6162 656c da1a 6469 616c 6f67 5f75  _label..dialog_u
 00000280: 7361 6765 5f74 6f6b 656e 735f 7072 6f6d  sage_tokens_prom
-00000290: 7074 5a1a 6469 616c 6f67 5f75 7361 6765  ptZ.dialog_usage
+00000290: 7074 da1a 6469 616c 6f67 5f75 7361 6765  pt..dialog_usage
 000002a0: 5f74 6f6b 656e 735f 616e 7377 6572 da19  _tokens_answer..
 000002b0: 6469 616c 6f67 5f75 7361 6765 5f74 6f6b  dialog_usage_tok
 000002c0: 656e 735f 746f 7461 6cda 1a64 6961 6c6f  ens_total..dialo
 000002d0: 675f 6275 7474 6f6e 5f73 656e 645f 7265  g_button_send_re
 000002e0: 7175 6573 744e 2901 da07 6c65 7865 6d65  questN)...lexeme
-000002f0: 73a9 0072 0d00 0000 720d 0000 00fa 492f  s..r....r.....I/
+000002f0: 73a9 0072 0e00 0000 720e 0000 00fa 492f  s..r....r.....I/
 00000300: 5573 6572 732f 7661 6469 6b75 732f 5079  Users/vadikus/Py
 00000310: 6368 6172 6d50 726f 6a65 6374 732f 6e6f  charmProjects/no
-00000320: 746f 6c6f 672f 6e6f 746f 6c6f 672f 6c65  tolog/notolog/le
+00000320: 746f 6c6f 672d 6465 762f 6170 702f 6c65  tolog-dev/app/le
 00000330: 7865 6d65 732f 656e 2f61 695f 6173 7369  xemes/en/ai_assi
 00000340: 7374 616e 742e 7079 da08 3c6d 6f64 756c  stant.py..<modul
 00000350: 653e 0400 0000 7318 0000 0002 0102 0102  e>....s.........
 00000360: 0102 0102 0102 0202 0102 0102 0102 0102  ................
 00000370: 0102 f2                                  ...
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 7096 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 b81b 0000  a.......(..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 b81b 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 008f 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
@@ -120,284 +120,284 @@
 00000770: 6e6f 777a 0c53 7072 696e 6720 4772 6565  nowz.Spring Gree
 00000780: 6e7a 0a53 7465 656c 2042 6c75 655a 0354  nz.Steel BlueZ.T
 00000790: 616e da07 5468 6973 746c 65da 0654 6f6d  an..Thistle..Tom
 000007a0: 6174 6fda 0954 7572 7175 6f69 7365 da06  ato..Turquoise..
 000007b0: 5669 6f6c 6574 da05 5768 6561 747a 0b57  Violet..Wheatz.W
 000007c0: 6869 7465 2053 6d6f 6b65 7a0c 5965 6c6c  hite Smokez.Yell
 000007d0: 6f77 2047 7265 656e 298e da12 636f 6c6f  ow Green)...colo
-000007e0: 725f 7069 636b 6572 5f74 6974 6c65 5a18  r_picker_titleZ.
+000007e0: 725f 7069 636b 6572 5f74 6974 6c65 da18  r_picker_title..
 000007f0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000800: 6f72 5f62 6c61 636b 5a19 636f 6c6f 725f  or_blackZ.color_
+00000800: 6f72 5f62 6c61 636b da19 636f 6c6f 725f  or_black..color_
 00000810: 7069 636b 6572 5f63 6f6c 6f72 5f73 696c  picker_color_sil
-00000820: 7665 725a 1763 6f6c 6f72 5f70 6963 6b65  verZ.color_picke
-00000830: 725f 636f 6c6f 725f 6772 6179 5a18 636f  r_color_grayZ.co
+00000820: 7665 72da 1763 6f6c 6f72 5f70 6963 6b65  ver..color_picke
+00000830: 725f 636f 6c6f 725f 6772 6179 da18 636f  r_color_gray..co
 00000840: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000850: 5f77 6869 7465 5a19 636f 6c6f 725f 7069  _whiteZ.color_pi
+00000850: 5f77 6869 7465 da19 636f 6c6f 725f 7069  _white..color_pi
 00000860: 636b 6572 5f63 6f6c 6f72 5f6d 6172 6f6f  cker_color_maroo
-00000870: 6e5a 1663 6f6c 6f72 5f70 6963 6b65 725f  nZ.color_picker_
-00000880: 636f 6c6f 725f 7265 645a 1963 6f6c 6f72  color_redZ.color
+00000870: 6eda 1663 6f6c 6f72 5f70 6963 6b65 725f  n..color_picker_
+00000880: 636f 6c6f 725f 7265 64da 1963 6f6c 6f72  color_red..color
 00000890: 5f70 6963 6b65 725f 636f 6c6f 725f 7075  _picker_color_pu
-000008a0: 7270 6c65 5a1a 636f 6c6f 725f 7069 636b  rpleZ.color_pick
+000008a0: 7270 6c65 da1a 636f 6c6f 725f 7069 636b  rple..color_pick
 000008b0: 6572 5f63 6f6c 6f72 5f66 7563 6873 6961  er_color_fuchsia
-000008c0: 5a18 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-000008d0: 6f6c 6f72 5f67 7265 656e 5a17 636f 6c6f  olor_greenZ.colo
+000008c0: da18 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+000008d0: 6f6c 6f72 5f67 7265 656e da17 636f 6c6f  olor_green..colo
 000008e0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
-000008f0: 696d 655a 1863 6f6c 6f72 5f70 6963 6b65  imeZ.color_picke
-00000900: 725f 636f 6c6f 725f 6f6c 6976 655a 1963  r_color_oliveZ.c
+000008f0: 696d 65da 1863 6f6c 6f72 5f70 6963 6b65  ime..color_picke
+00000900: 725f 636f 6c6f 725f 6f6c 6976 65da 1963  r_color_olive..c
 00000910: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000920: 725f 7965 6c6c 6f77 5a17 636f 6c6f 725f  r_yellowZ.color_
+00000920: 725f 7965 6c6c 6f77 da17 636f 6c6f 725f  r_yellow..color_
 00000930: 7069 636b 6572 5f63 6f6c 6f72 5f6e 6176  picker_color_nav
-00000940: 795a 1763 6f6c 6f72 5f70 6963 6b65 725f  yZ.color_picker_
-00000950: 636f 6c6f 725f 626c 7565 5a17 636f 6c6f  color_blueZ.colo
+00000940: 79da 1763 6f6c 6f72 5f70 6963 6b65 725f  y..color_picker_
+00000950: 636f 6c6f 725f 626c 7565 da17 636f 6c6f  color_blue..colo
 00000960: 725f 7069 636b 6572 5f63 6f6c 6f72 5f74  r_picker_color_t
-00000970: 6561 6c5a 1763 6f6c 6f72 5f70 6963 6b65  ealZ.color_picke
-00000980: 725f 636f 6c6f 725f 6171 7561 5a1c 636f  r_color_aquaZ.co
+00000970: 6561 6cda 1763 6f6c 6f72 5f70 6963 6b65  eal..color_picke
+00000980: 725f 636f 6c6f 725f 6171 7561 da1c 636f  r_color_aqua..co
 00000990: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-000009a0: 5f61 6c69 6365 626c 7565 5a1f 636f 6c6f  _aliceblueZ.colo
+000009a0: 5f61 6c69 6365 626c 7565 da1f 636f 6c6f  _aliceblue..colo
 000009b0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f61  r_picker_color_a
-000009c0: 6e74 6971 7565 7768 6974 655a 1d63 6f6c  ntiquewhiteZ.col
+000009c0: 6e74 6971 7565 7768 6974 65da 1d63 6f6c  ntiquewhite..col
 000009d0: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-000009e0: 6171 7561 6d61 7269 6e65 5a18 636f 6c6f  aquamarineZ.colo
+000009e0: 6171 7561 6d61 7269 6e65 da18 636f 6c6f  aquamarine..colo
 000009f0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f61  r_picker_color_a
-00000a00: 7a75 7265 5a18 636f 6c6f 725f 7069 636b  zureZ.color_pick
-00000a10: 6572 5f63 6f6c 6f72 5f62 6569 6765 5a19  er_color_beigeZ.
+00000a00: 7a75 7265 da18 636f 6c6f 725f 7069 636b  zure..color_pick
+00000a10: 6572 5f63 6f6c 6f72 5f62 6569 6765 da19  er_color_beige..
 00000a20: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000a30: 6f72 5f62 6973 7175 655a 2163 6f6c 6f72  or_bisqueZ!color
+00000a30: 6f72 5f62 6973 7175 65da 2163 6f6c 6f72  or_bisque.!color
 00000a40: 5f70 6963 6b65 725f 636f 6c6f 725f 626c  _picker_color_bl
-00000a50: 616e 6368 6564 616c 6d6f 6e64 5a1d 636f  anchedalmondZ.co
+00000a50: 616e 6368 6564 616c 6d6f 6e64 da1d 636f  anchedalmond..co
 00000a60: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000a70: 5f62 6c75 6576 696f 6c65 745a 1863 6f6c  _bluevioletZ.col
+00000a70: 5f62 6c75 6576 696f 6c65 74da 1863 6f6c  _blueviolet..col
 00000a80: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000a90: 6272 6f77 6e5a 1c63 6f6c 6f72 5f70 6963  brownZ.color_pic
+00000a90: 6272 6f77 6eda 1c63 6f6c 6f72 5f70 6963  brown..color_pic
 00000aa0: 6b65 725f 636f 6c6f 725f 6275 726c 7977  ker_color_burlyw
-00000ab0: 6f6f 645a 1c63 6f6c 6f72 5f70 6963 6b65  oodZ.color_picke
+00000ab0: 6f6f 64da 1c63 6f6c 6f72 5f70 6963 6b65  ood..color_picke
 00000ac0: 725f 636f 6c6f 725f 6361 6465 7462 6c75  r_color_cadetblu
-00000ad0: 655a 1d63 6f6c 6f72 5f70 6963 6b65 725f  eZ.color_picker_
+00000ad0: 65da 1d63 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
 00000ae0: 636f 6c6f 725f 6368 6172 7472 6575 7365  color_chartreuse
-00000af0: 5a1c 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-00000b00: 6f6c 6f72 5f63 686f 636f 6c61 7465 5a18  olor_chocolateZ.
+00000af0: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000b00: 6f6c 6f72 5f63 686f 636f 6c61 7465 da18  olor_chocolate..
 00000b10: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000b20: 6f72 5f63 6f72 616c 5a21 636f 6c6f 725f  or_coralZ!color_
+00000b20: 6f72 5f63 6f72 616c da21 636f 6c6f 725f  or_coral.!color_
 00000b30: 7069 636b 6572 5f63 6f6c 6f72 5f63 6f72  picker_color_cor
-00000b40: 6e66 6c6f 7765 7262 6c75 655a 1b63 6f6c  nflowerblueZ.col
+00000b40: 6e66 6c6f 7765 7262 6c75 65da 1b63 6f6c  nflowerblue..col
 00000b50: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000b60: 636f 726e 7369 6c6b 5a1a 636f 6c6f 725f  cornsilkZ.color_
+00000b60: 636f 726e 7369 6c6b da1a 636f 6c6f 725f  cornsilk..color_
 00000b70: 7069 636b 6572 5f63 6f6c 6f72 5f63 7269  picker_color_cri
-00000b80: 6d73 6f6e 5a17 636f 6c6f 725f 7069 636b  msonZ.color_pick
-00000b90: 6572 5f63 6f6c 6f72 5f63 7961 6e5a 1b63  er_color_cyanZ.c
+00000b80: 6d73 6f6e da17 636f 6c6f 725f 7069 636b  mson..color_pick
+00000b90: 6572 5f63 6f6c 6f72 5f63 7961 6eda 1b63  er_color_cyan..c
 00000ba0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000bb0: 725f 6461 726b 626c 7565 5a1b 636f 6c6f  r_darkblueZ.colo
+00000bb0: 725f 6461 726b 626c 7565 da1b 636f 6c6f  r_darkblue..colo
 00000bc0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f64  r_picker_color_d
-00000bd0: 6172 6b63 7961 6e5a 2063 6f6c 6f72 5f70  arkcyanZ color_p
+00000bd0: 6172 6b63 7961 6eda 2063 6f6c 6f72 5f70  arkcyan. color_p
 00000be0: 6963 6b65 725f 636f 6c6f 725f 6461 726b  icker_color_dark
-00000bf0: 676f 6c64 656e 726f 645a 1b63 6f6c 6f72  goldenrodZ.color
+00000bf0: 676f 6c64 656e 726f 64da 1b63 6f6c 6f72  goldenrod..color
 00000c00: 5f70 6963 6b65 725f 636f 6c6f 725f 6461  _picker_color_da
-00000c10: 726b 6772 6179 5a1c 636f 6c6f 725f 7069  rkgrayZ.color_pi
+00000c10: 726b 6772 6179 da1c 636f 6c6f 725f 7069  rkgray..color_pi
 00000c20: 636b 6572 5f63 6f6c 6f72 5f64 6172 6b67  cker_color_darkg
-00000c30: 7265 656e 5a1c 636f 6c6f 725f 7069 636b  reenZ.color_pick
+00000c30: 7265 656e da1c 636f 6c6f 725f 7069 636b  reen..color_pick
 00000c40: 6572 5f63 6f6c 6f72 5f64 6172 6b6b 6861  er_color_darkkha
-00000c50: 6b69 5a1e 636f 6c6f 725f 7069 636b 6572  kiZ.color_picker
+00000c50: 6b69 da1e 636f 6c6f 725f 7069 636b 6572  ki..color_picker
 00000c60: 5f63 6f6c 6f72 5f64 6172 6b6d 6167 656e  _color_darkmagen
-00000c70: 7461 5a21 636f 6c6f 725f 7069 636b 6572  taZ!color_picker
+00000c70: 7461 da21 636f 6c6f 725f 7069 636b 6572  ta.!color_picker
 00000c80: 5f63 6f6c 6f72 5f64 6172 6b6f 6c69 7665  _color_darkolive
-00000c90: 6772 6565 6e5a 1d63 6f6c 6f72 5f70 6963  greenZ.color_pic
+00000c90: 6772 6565 6eda 1d63 6f6c 6f72 5f70 6963  green..color_pic
 00000ca0: 6b65 725f 636f 6c6f 725f 6461 726b 6f72  ker_color_darkor
-00000cb0: 616e 6765 5a1d 636f 6c6f 725f 7069 636b  angeZ.color_pick
+00000cb0: 616e 6765 da1d 636f 6c6f 725f 7069 636b  ange..color_pick
 00000cc0: 6572 5f63 6f6c 6f72 5f64 6172 6b6f 7263  er_color_darkorc
-00000cd0: 6869 645a 1a63 6f6c 6f72 5f70 6963 6b65  hidZ.color_picke
-00000ce0: 725f 636f 6c6f 725f 6461 726b 7265 645a  r_color_darkredZ
+00000cd0: 6869 64da 1a63 6f6c 6f72 5f70 6963 6b65  hid..color_picke
+00000ce0: 725f 636f 6c6f 725f 6461 726b 7265 64da  r_color_darkred.
 00000cf0: 1d63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00000d00: 6c6f 725f 6461 726b 7361 6c6d 6f6e 5a1f  lor_darksalmonZ.
+00000d00: 6c6f 725f 6461 726b 7361 6c6d 6f6e da1f  lor_darksalmon..
 00000d10: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000d20: 6f72 5f64 6172 6b73 6561 6772 6565 6e5a  or_darkseagreenZ
+00000d20: 6f72 5f64 6172 6b73 6561 6772 6565 6eda  or_darkseagreen.
 00000d30: 2063 6f6c 6f72 5f70 6963 6b65 725f 636f   color_picker_co
 00000d40: 6c6f 725f 6461 726b 736c 6174 6562 6c75  lor_darkslateblu
-00000d50: 655a 2063 6f6c 6f72 5f70 6963 6b65 725f  eZ color_picker_
+00000d50: 65da 2063 6f6c 6f72 5f70 6963 6b65 725f  e. color_picker_
 00000d60: 636f 6c6f 725f 6461 726b 736c 6174 6567  color_darkslateg
-00000d70: 7261 795a 2063 6f6c 6f72 5f70 6963 6b65  rayZ color_picke
+00000d70: 7261 79da 2063 6f6c 6f72 5f70 6963 6b65  ray. color_picke
 00000d80: 725f 636f 6c6f 725f 6461 726b 7475 7271  r_color_darkturq
-00000d90: 756f 6973 655a 1d63 6f6c 6f72 5f70 6963  uoiseZ.color_pic
+00000d90: 756f 6973 65da 1d63 6f6c 6f72 5f70 6963  uoise..color_pic
 00000da0: 6b65 725f 636f 6c6f 725f 6461 726b 7669  ker_color_darkvi
-00000db0: 6f6c 6574 5a1b 636f 6c6f 725f 7069 636b  oletZ.color_pick
+00000db0: 6f6c 6574 da1b 636f 6c6f 725f 7069 636b  olet..color_pick
 00000dc0: 6572 5f63 6f6c 6f72 5f64 6565 7070 696e  er_color_deeppin
-00000dd0: 6b5a 1e63 6f6c 6f72 5f70 6963 6b65 725f  kZ.color_picker_
+00000dd0: 6bda 1e63 6f6c 6f72 5f70 6963 6b65 725f  k..color_picker_
 00000de0: 636f 6c6f 725f 6465 6570 736b 7962 6c75  color_deepskyblu
-00000df0: 655a 1a63 6f6c 6f72 5f70 6963 6b65 725f  eZ.color_picker_
-00000e00: 636f 6c6f 725f 6469 6d67 7261 795a 1d63  color_dimgrayZ.c
+00000df0: 65da 1a63 6f6c 6f72 5f70 6963 6b65 725f  e..color_picker_
+00000e00: 636f 6c6f 725f 6469 6d67 7261 79da 1d63  color_dimgray..c
 00000e10: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00000e20: 725f 646f 6467 6572 626c 7565 5a1c 636f  r_dodgerblueZ.co
+00000e20: 725f 646f 6467 6572 626c 7565 da1c 636f  r_dodgerblue..co
 00000e30: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00000e40: 5f66 6972 6562 7269 636b 5a1e 636f 6c6f  _firebrickZ.colo
+00000e40: 5f66 6972 6562 7269 636b da1e 636f 6c6f  _firebrick..colo
 00000e50: 725f 7069 636b 6572 5f63 6f6c 6f72 5f66  r_picker_color_f
-00000e60: 6c6f 7261 6c77 6869 7465 5a1e 636f 6c6f  loralwhiteZ.colo
+00000e60: 6c6f 7261 6c77 6869 7465 da1e 636f 6c6f  loralwhite..colo
 00000e70: 725f 7069 636b 6572 5f63 6f6c 6f72 5f66  r_picker_color_f
-00000e80: 6f72 6573 7467 7265 656e 5a1c 636f 6c6f  orestgreenZ.colo
+00000e80: 6f72 6573 7467 7265 656e da1c 636f 6c6f  orestgreen..colo
 00000e90: 725f 7069 636b 6572 5f63 6f6c 6f72 5f67  r_picker_color_g
-00000ea0: 6169 6e73 626f 726f 5a1d 636f 6c6f 725f  ainsboroZ.color_
+00000ea0: 6169 6e73 626f 726f da1d 636f 6c6f 725f  ainsboro..color_
 00000eb0: 7069 636b 6572 5f63 6f6c 6f72 5f67 686f  picker_color_gho
-00000ec0: 7374 7768 6974 655a 1763 6f6c 6f72 5f70  stwhiteZ.color_p
+00000ec0: 7374 7768 6974 65da 1763 6f6c 6f72 5f70  stwhite..color_p
 00000ed0: 6963 6b65 725f 636f 6c6f 725f 676f 6c64  icker_color_gold
-00000ee0: 5a1c 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-00000ef0: 6f6c 6f72 5f67 6f6c 6465 6e72 6f64 5a1e  olor_goldenrodZ.
+00000ee0: da1c 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000ef0: 6f6c 6f72 5f67 6f6c 6465 6e72 6f64 da1e  olor_goldenrod..
 00000f00: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000f10: 6f72 5f67 7265 656e 7965 6c6c 6f77 5a1b  or_greenyellowZ.
+00000f10: 6f72 5f67 7265 656e 7965 6c6c 6f77 da1b  or_greenyellow..
 00000f20: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00000f30: 6f72 5f68 6f6e 6579 6465 775a 1a63 6f6c  or_honeydewZ.col
+00000f30: 6f72 5f68 6f6e 6579 6465 77da 1a63 6f6c  or_honeydew..col
 00000f40: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00000f50: 686f 7470 696e 6b5a 1c63 6f6c 6f72 5f70  hotpinkZ.color_p
+00000f50: 686f 7470 696e 6bda 1c63 6f6c 6f72 5f70  hotpink..color_p
 00000f60: 6963 6b65 725f 636f 6c6f 725f 696e 6469  icker_color_indi
-00000f70: 616e 7265 645a 1963 6f6c 6f72 5f70 6963  anredZ.color_pic
+00000f70: 616e 7265 64da 1963 6f6c 6f72 5f70 6963  anred..color_pic
 00000f80: 6b65 725f 636f 6c6f 725f 696e 6469 676f  ker_color_indigo
-00000f90: 5a18 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-00000fa0: 6f6c 6f72 5f69 766f 7279 5a18 636f 6c6f  olor_ivoryZ.colo
+00000f90: da18 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00000fa0: 6f6c 6f72 5f69 766f 7279 da18 636f 6c6f  olor_ivory..colo
 00000fb0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6b  r_picker_color_k
-00000fc0: 6861 6b69 5a1b 636f 6c6f 725f 7069 636b  hakiZ.color_pick
+00000fc0: 6861 6b69 da1b 636f 6c6f 725f 7069 636b  haki..color_pick
 00000fd0: 6572 5f63 6f6c 6f72 5f6c 6176 656e 6465  er_color_lavende
-00000fe0: 725a 2063 6f6c 6f72 5f70 6963 6b65 725f  rZ color_picker_
+00000fe0: 72da 2063 6f6c 6f72 5f70 6963 6b65 725f  r. color_picker_
 00000ff0: 636f 6c6f 725f 6c61 7665 6e64 6572 626c  color_lavenderbl
-00001000: 7573 685a 1c63 6f6c 6f72 5f70 6963 6b65  ushZ.color_picke
+00001000: 7573 68da 1c63 6f6c 6f72 5f70 6963 6b65  ush..color_picke
 00001010: 725f 636f 6c6f 725f 6c61 776e 6772 6565  r_color_lawngree
-00001020: 6e5a 1f63 6f6c 6f72 5f70 6963 6b65 725f  nZ.color_picker_
+00001020: 6eda 1f63 6f6c 6f72 5f70 6963 6b65 725f  n..color_picker_
 00001030: 636f 6c6f 725f 6c65 6d6f 6e63 6869 6666  color_lemonchiff
-00001040: 6f6e 5a1c 636f 6c6f 725f 7069 636b 6572  onZ.color_picker
+00001040: 6f6e da1c 636f 6c6f 725f 7069 636b 6572  on..color_picker
 00001050: 5f63 6f6c 6f72 5f6c 6967 6874 626c 7565  _color_lightblue
-00001060: 5a1d 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-00001070: 6f6c 6f72 5f6c 6967 6874 636f 7261 6c5a  olor_lightcoralZ
+00001060: da1d 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001070: 6f6c 6f72 5f6c 6967 6874 636f 7261 6cda  olor_lightcoral.
 00001080: 1c63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00001090: 6c6f 725f 6c69 6768 7463 7961 6e5a 2763  lor_lightcyanZ'c
+00001090: 6c6f 725f 6c69 6768 7463 7961 6eda 2763  lor_lightcyan.'c
 000010a0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
 000010b0: 725f 6c69 6768 7467 6f6c 6465 6e72 6f64  r_lightgoldenrod
-000010c0: 7965 6c6c 6f77 5a1c 636f 6c6f 725f 7069  yellowZ.color_pi
+000010c0: 7965 6c6c 6f77 da1c 636f 6c6f 725f 7069  yellow..color_pi
 000010d0: 636b 6572 5f63 6f6c 6f72 5f6c 6967 6874  cker_color_light
-000010e0: 6772 6179 5a1d 636f 6c6f 725f 7069 636b  grayZ.color_pick
+000010e0: 6772 6179 da1d 636f 6c6f 725f 7069 636b  gray..color_pick
 000010f0: 6572 5f63 6f6c 6f72 5f6c 6967 6874 6772  er_color_lightgr
-00001100: 6565 6e5a 1c63 6f6c 6f72 5f70 6963 6b65  eenZ.color_picke
+00001100: 6565 6eda 1c63 6f6c 6f72 5f70 6963 6b65  een..color_picke
 00001110: 725f 636f 6c6f 725f 6c69 6768 7470 696e  r_color_lightpin
-00001120: 6b5a 1e63 6f6c 6f72 5f70 6963 6b65 725f  kZ.color_picker_
+00001120: 6bda 1e63 6f6c 6f72 5f70 6963 6b65 725f  k..color_picker_
 00001130: 636f 6c6f 725f 6c69 6768 7473 616c 6d6f  color_lightsalmo
-00001140: 6e5a 2063 6f6c 6f72 5f70 6963 6b65 725f  nZ color_picker_
+00001140: 6eda 2063 6f6c 6f72 5f70 6963 6b65 725f  n. color_picker_
 00001150: 636f 6c6f 725f 6c69 6768 7473 6561 6772  color_lightseagr
-00001160: 6565 6e5a 1f63 6f6c 6f72 5f70 6963 6b65  eenZ.color_picke
+00001160: 6565 6eda 1f63 6f6c 6f72 5f70 6963 6b65  een..color_picke
 00001170: 725f 636f 6c6f 725f 6c69 6768 7473 6b79  r_color_lightsky
-00001180: 626c 7565 5a21 636f 6c6f 725f 7069 636b  blueZ!color_pick
+00001180: 626c 7565 da21 636f 6c6f 725f 7069 636b  blue.!color_pick
 00001190: 6572 5f63 6f6c 6f72 5f6c 6967 6874 736c  er_color_lightsl
-000011a0: 6174 6567 7261 795a 2163 6f6c 6f72 5f70  ategrayZ!color_p
+000011a0: 6174 6567 7261 79da 2163 6f6c 6f72 5f70  ategray.!color_p
 000011b0: 6963 6b65 725f 636f 6c6f 725f 6c69 6768  icker_color_ligh
-000011c0: 7473 7465 656c 626c 7565 5a1e 636f 6c6f  tsteelblueZ.colo
+000011c0: 7473 7465 656c 626c 7565 da1e 636f 6c6f  tsteelblue..colo
 000011d0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
-000011e0: 6967 6874 7965 6c6c 6f77 5a1c 636f 6c6f  ightyellowZ.colo
+000011e0: 6967 6874 7965 6c6c 6f77 da1c 636f 6c6f  ightyellow..colo
 000011f0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6c  r_picker_color_l
-00001200: 696d 6567 7265 656e 5a18 636f 6c6f 725f  imegreenZ.color_
+00001200: 696d 6567 7265 656e da18 636f 6c6f 725f  imegreen..color_
 00001210: 7069 636b 6572 5f63 6f6c 6f72 5f6c 696e  picker_color_lin
-00001220: 656e 5a1a 636f 6c6f 725f 7069 636b 6572  enZ.color_picker
-00001230: 5f63 6f6c 6f72 5f6d 6167 656e 7461 5a23  _color_magentaZ#
+00001220: 656e da1a 636f 6c6f 725f 7069 636b 6572  en..color_picker
+00001230: 5f63 6f6c 6f72 5f6d 6167 656e 7461 da23  _color_magenta.#
 00001240: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
 00001250: 6f72 5f6d 6564 6975 6d61 7175 616d 6172  or_mediumaquamar
-00001260: 696e 655a 1d63 6f6c 6f72 5f70 6963 6b65  ineZ.color_picke
+00001260: 696e 65da 1d63 6f6c 6f72 5f70 6963 6b65  ine..color_picke
 00001270: 725f 636f 6c6f 725f 6d65 6469 756d 626c  r_color_mediumbl
-00001280: 7565 5a1f 636f 6c6f 725f 7069 636b 6572  ueZ.color_picker
+00001280: 7565 da1f 636f 6c6f 725f 7069 636b 6572  ue..color_picker
 00001290: 5f63 6f6c 6f72 5f6d 6564 6975 6d6f 7263  _color_mediumorc
-000012a0: 6869 645a 1f63 6f6c 6f72 5f70 6963 6b65  hidZ.color_picke
+000012a0: 6869 64da 1f63 6f6c 6f72 5f70 6963 6b65  hid..color_picke
 000012b0: 725f 636f 6c6f 725f 6d65 6469 756d 7075  r_color_mediumpu
-000012c0: 7270 6c65 5a21 636f 6c6f 725f 7069 636b  rpleZ!color_pick
+000012c0: 7270 6c65 da21 636f 6c6f 725f 7069 636b  rple.!color_pick
 000012d0: 6572 5f63 6f6c 6f72 5f6d 6564 6975 6d73  er_color_mediums
-000012e0: 6561 6772 6565 6e5a 2263 6f6c 6f72 5f70  eagreenZ"color_p
+000012e0: 6561 6772 6565 6eda 2263 6f6c 6f72 5f70  eagreen."color_p
 000012f0: 6963 6b65 725f 636f 6c6f 725f 6d65 6469  icker_color_medi
-00001300: 756d 736c 6174 6562 6c75 655a 2463 6f6c  umslateblueZ$col
+00001300: 756d 736c 6174 6562 6c75 65da 2463 6f6c  umslateblue.$col
 00001310: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
 00001320: 6d65 6469 756d 7370 7269 6e67 6772 6565  mediumspringgree
-00001330: 6e5a 2263 6f6c 6f72 5f70 6963 6b65 725f  nZ"color_picker_
+00001330: 6eda 2263 6f6c 6f72 5f70 6963 6b65 725f  n."color_picker_
 00001340: 636f 6c6f 725f 6d65 6469 756d 7475 7271  color_mediumturq
-00001350: 756f 6973 655a 2263 6f6c 6f72 5f70 6963  uoiseZ"color_pic
+00001350: 756f 6973 65da 2263 6f6c 6f72 5f70 6963  uoise."color_pic
 00001360: 6b65 725f 636f 6c6f 725f 6d65 6469 756d  ker_color_medium
-00001370: 7669 6f6c 6574 7265 645a 1f63 6f6c 6f72  violetredZ.color
+00001370: 7669 6f6c 6574 7265 64da 1f63 6f6c 6f72  violetred..color
 00001380: 5f70 6963 6b65 725f 636f 6c6f 725f 6d69  _picker_color_mi
-00001390: 646e 6967 6874 626c 7565 5a1c 636f 6c6f  dnightblueZ.colo
+00001390: 646e 6967 6874 626c 7565 da1c 636f 6c6f  dnightblue..colo
 000013a0: 725f 7069 636b 6572 5f63 6f6c 6f72 5f6d  r_picker_color_m
-000013b0: 696e 7463 7265 616d 5a1c 636f 6c6f 725f  intcreamZ.color_
+000013b0: 696e 7463 7265 616d da1c 636f 6c6f 725f  intcream..color_
 000013c0: 7069 636b 6572 5f63 6f6c 6f72 5f6d 6973  picker_color_mis
-000013d0: 7479 726f 7365 5a1b 636f 6c6f 725f 7069  tyroseZ.color_pi
+000013d0: 7479 726f 7365 da1b 636f 6c6f 725f 7069  tyrose..color_pi
 000013e0: 636b 6572 5f63 6f6c 6f72 5f6d 6f63 6361  cker_color_mocca
-000013f0: 7369 6e5a 1e63 6f6c 6f72 5f70 6963 6b65  sinZ.color_picke
+000013f0: 7369 6eda 1e63 6f6c 6f72 5f70 6963 6b65  sin..color_picke
 00001400: 725f 636f 6c6f 725f 6e61 7661 6a6f 7768  r_color_navajowh
-00001410: 6974 655a 1a63 6f6c 6f72 5f70 6963 6b65  iteZ.color_picke
-00001420: 725f 636f 6c6f 725f 6f6c 646c 6163 655a  r_color_oldlaceZ
+00001410: 6974 65da 1a63 6f6c 6f72 5f70 6963 6b65  ite..color_picke
+00001420: 725f 636f 6c6f 725f 6f6c 646c 6163 65da  r_color_oldlace.
 00001430: 1c63 6f6c 6f72 5f70 6963 6b65 725f 636f  .color_picker_co
-00001440: 6c6f 725f 6f6c 6976 6564 7261 625a 1963  lor_olivedrabZ.c
+00001440: 6c6f 725f 6f6c 6976 6564 7261 62da 1963  lor_olivedrab..c
 00001450: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-00001460: 725f 6f72 616e 6765 5a1c 636f 6c6f 725f  r_orangeZ.color_
+00001460: 725f 6f72 616e 6765 da1c 636f 6c6f 725f  r_orange..color_
 00001470: 7069 636b 6572 5f63 6f6c 6f72 5f6f 7261  picker_color_ora
-00001480: 6e67 6572 6564 5a19 636f 6c6f 725f 7069  ngeredZ.color_pi
+00001480: 6e67 6572 6564 da19 636f 6c6f 725f 7069  ngered..color_pi
 00001490: 636b 6572 5f63 6f6c 6f72 5f6f 7263 6869  cker_color_orchi
-000014a0: 645a 2063 6f6c 6f72 5f70 6963 6b65 725f  dZ color_picker_
+000014a0: 64da 2063 6f6c 6f72 5f70 6963 6b65 725f  d. color_picker_
 000014b0: 636f 6c6f 725f 7061 6c65 676f 6c64 656e  color_palegolden
-000014c0: 726f 645a 1c63 6f6c 6f72 5f70 6963 6b65  rodZ.color_picke
+000014c0: 726f 64da 1c63 6f6c 6f72 5f70 6963 6b65  rod..color_picke
 000014d0: 725f 636f 6c6f 725f 7061 6c65 6772 6565  r_color_palegree
-000014e0: 6e5a 2063 6f6c 6f72 5f70 6963 6b65 725f  nZ color_picker_
+000014e0: 6eda 2063 6f6c 6f72 5f70 6963 6b65 725f  n. color_picker_
 000014f0: 636f 6c6f 725f 7061 6c65 7475 7271 756f  color_paleturquo
-00001500: 6973 655a 2063 6f6c 6f72 5f70 6963 6b65  iseZ color_picke
+00001500: 6973 65da 2063 6f6c 6f72 5f70 6963 6b65  ise. color_picke
 00001510: 725f 636f 6c6f 725f 7061 6c65 7669 6f6c  r_color_paleviol
-00001520: 6574 7265 645a 1d63 6f6c 6f72 5f70 6963  etredZ.color_pic
+00001520: 6574 7265 64da 1d63 6f6c 6f72 5f70 6963  etred..color_pic
 00001530: 6b65 725f 636f 6c6f 725f 7061 7061 7961  ker_color_papaya
-00001540: 7768 6970 5a1c 636f 6c6f 725f 7069 636b  whipZ.color_pick
+00001540: 7768 6970 da1c 636f 6c6f 725f 7069 636b  whip..color_pick
 00001550: 6572 5f63 6f6c 6f72 5f70 6561 6368 7075  er_color_peachpu
-00001560: 6666 5a17 636f 6c6f 725f 7069 636b 6572  ffZ.color_picker
-00001570: 5f63 6f6c 6f72 5f70 6572 755a 1763 6f6c  _color_peruZ.col
+00001560: 6666 da17 636f 6c6f 725f 7069 636b 6572  ff..color_picker
+00001570: 5f63 6f6c 6f72 5f70 6572 75da 1763 6f6c  _color_peru..col
 00001580: 6f72 5f70 6963 6b65 725f 636f 6c6f 725f  or_picker_color_
-00001590: 7069 6e6b 5a17 636f 6c6f 725f 7069 636b  pinkZ.color_pick
-000015a0: 6572 5f63 6f6c 6f72 5f70 6c75 6d5a 1d63  er_color_plumZ.c
+00001590: 7069 6e6b da17 636f 6c6f 725f 7069 636b  pink..color_pick
+000015a0: 6572 5f63 6f6c 6f72 5f70 6c75 6dda 1d63  er_color_plum..c
 000015b0: 6f6c 6f72 5f70 6963 6b65 725f 636f 6c6f  olor_picker_colo
-000015c0: 725f 706f 7764 6572 626c 7565 5a20 636f  r_powderblueZ co
+000015c0: 725f 706f 7764 6572 626c 7565 da20 636f  r_powderblue. co
 000015d0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-000015e0: 5f72 6562 6563 6361 7075 7270 6c65 5a1c  _rebeccapurpleZ.
+000015e0: 5f72 6562 6563 6361 7075 7270 6c65 da1c  _rebeccapurple..
 000015f0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-00001600: 6f72 5f72 6f73 7962 726f 776e 5a1c 636f  or_rosybrownZ.co
+00001600: 6f72 5f72 6f73 7962 726f 776e da1c 636f  or_rosybrown..co
 00001610: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-00001620: 5f72 6f79 616c 626c 7565 5a1e 636f 6c6f  _royalblueZ.colo
+00001620: 5f72 6f79 616c 626c 7565 da1e 636f 6c6f  _royalblue..colo
 00001630: 725f 7069 636b 6572 5f63 6f6c 6f72 5f73  r_picker_color_s
-00001640: 6164 646c 6562 726f 776e 5a19 636f 6c6f  addlebrownZ.colo
+00001640: 6164 646c 6562 726f 776e da19 636f 6c6f  addlebrown..colo
 00001650: 725f 7069 636b 6572 5f63 6f6c 6f72 5f73  r_picker_color_s
-00001660: 616c 6d6f 6e5a 1d63 6f6c 6f72 5f70 6963  almonZ.color_pic
+00001660: 616c 6d6f 6eda 1d63 6f6c 6f72 5f70 6963  almon..color_pic
 00001670: 6b65 725f 636f 6c6f 725f 7361 6e64 7962  ker_color_sandyb
-00001680: 726f 776e 5a1b 636f 6c6f 725f 7069 636b  rownZ.color_pick
+00001680: 726f 776e da1b 636f 6c6f 725f 7069 636b  rown..color_pick
 00001690: 6572 5f63 6f6c 6f72 5f73 6561 6772 6565  er_color_seagree
-000016a0: 6e5a 1b63 6f6c 6f72 5f70 6963 6b65 725f  nZ.color_picker_
-000016b0: 636f 6c6f 725f 7365 6173 6865 6c6c 5a19  color_seashellZ.
+000016a0: 6eda 1b63 6f6c 6f72 5f70 6963 6b65 725f  n..color_picker_
+000016b0: 636f 6c6f 725f 7365 6173 6865 6c6c da19  color_seashell..
 000016c0: 636f 6c6f 725f 7069 636b 6572 5f63 6f6c  color_picker_col
-000016d0: 6f72 5f73 6965 6e6e 615a 1a63 6f6c 6f72  or_siennaZ.color
+000016d0: 6f72 5f73 6965 6e6e 61da 1a63 6f6c 6f72  or_sienna..color
 000016e0: 5f70 6963 6b65 725f 636f 6c6f 725f 736b  _picker_color_sk
-000016f0: 7962 6c75 655a 1c63 6f6c 6f72 5f70 6963  yblueZ.color_pic
+000016f0: 7962 6c75 65da 1c63 6f6c 6f72 5f70 6963  yblue..color_pic
 00001700: 6b65 725f 636f 6c6f 725f 736c 6174 6562  ker_color_slateb
-00001710: 6c75 655a 1c63 6f6c 6f72 5f70 6963 6b65  lueZ.color_picke
+00001710: 6c75 65da 1c63 6f6c 6f72 5f70 6963 6b65  lue..color_picke
 00001720: 725f 636f 6c6f 725f 736c 6174 6567 7261  r_color_slategra
-00001730: 795a 1763 6f6c 6f72 5f70 6963 6b65 725f  yZ.color_picker_
-00001740: 636f 6c6f 725f 736e 6f77 5a1e 636f 6c6f  color_snowZ.colo
+00001730: 79da 1763 6f6c 6f72 5f70 6963 6b65 725f  y..color_picker_
+00001740: 636f 6c6f 725f 736e 6f77 da1e 636f 6c6f  color_snow..colo
 00001750: 725f 7069 636b 6572 5f63 6f6c 6f72 5f73  r_picker_color_s
-00001760: 7072 696e 6767 7265 656e 5a1c 636f 6c6f  pringgreenZ.colo
+00001760: 7072 696e 6767 7265 656e da1c 636f 6c6f  pringgreen..colo
 00001770: 725f 7069 636b 6572 5f63 6f6c 6f72 5f73  r_picker_color_s
-00001780: 7465 656c 626c 7565 5a16 636f 6c6f 725f  teelblueZ.color_
+00001780: 7465 656c 626c 7565 da16 636f 6c6f 725f  teelblue..color_
 00001790: 7069 636b 6572 5f63 6f6c 6f72 5f74 616e  picker_color_tan
-000017a0: 5a1a 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-000017b0: 6f6c 6f72 5f74 6869 7374 6c65 5a19 636f  olor_thistleZ.co
+000017a0: da1a 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+000017b0: 6f6c 6f72 5f74 6869 7374 6c65 da19 636f  olor_thistle..co
 000017c0: 6c6f 725f 7069 636b 6572 5f63 6f6c 6f72  lor_picker_color
-000017d0: 5f74 6f6d 6174 6f5a 1c63 6f6c 6f72 5f70  _tomatoZ.color_p
+000017d0: 5f74 6f6d 6174 6fda 1c63 6f6c 6f72 5f70  _tomato..color_p
 000017e0: 6963 6b65 725f 636f 6c6f 725f 7475 7271  icker_color_turq
-000017f0: 756f 6973 655a 1963 6f6c 6f72 5f70 6963  uoiseZ.color_pic
+000017f0: 756f 6973 65da 1963 6f6c 6f72 5f70 6963  uoise..color_pic
 00001800: 6b65 725f 636f 6c6f 725f 7669 6f6c 6574  ker_color_violet
-00001810: 5a18 636f 6c6f 725f 7069 636b 6572 5f63  Z.color_picker_c
-00001820: 6f6c 6f72 5f77 6865 6174 5a1d 636f 6c6f  olor_wheatZ.colo
+00001810: da18 636f 6c6f 725f 7069 636b 6572 5f63  ..color_picker_c
+00001820: 6f6c 6f72 5f77 6865 6174 da1d 636f 6c6f  olor_wheat..colo
 00001830: 725f 7069 636b 6572 5f63 6f6c 6f72 5f77  r_picker_color_w
-00001840: 6869 7465 736d 6f6b 655a 1e63 6f6c 6f72  hitesmokeZ.color
+00001840: 6869 7465 736d 6f6b 65da 1e63 6f6c 6f72  hitesmoke..color
 00001850: 5f70 6963 6b65 725f 636f 6c6f 725f 7965  _picker_color_ye
 00001860: 6c6c 6f77 6772 6565 6e4e 2901 da07 6c65  llowgreenN)...le
-00001870: 7865 6d65 73a9 0072 2e00 0000 722e 0000  xemes..r....r...
+00001870: 7865 6d65 73a9 0072 bb00 0000 72bb 0000  xemes..r....r...
 00001880: 00fa 502f 5573 6572 732f 7661 6469 6b75  ..P/Users/vadiku
 00001890: 732f 5079 6368 6172 6d50 726f 6a65 6374  s/PycharmProject
-000018a0: 732f 6e6f 746f 6c6f 672f 6e6f 746f 6c6f  s/notolog/notolo
-000018b0: 672f 6c65 7865 6d65 732f 656e 2f63 6f6c  g/lexemes/en/col
+000018a0: 732f 6e6f 746f 6c6f 672d 6465 762f 6170  s/notolog-dev/ap
+000018b0: 702f 6c65 7865 6d65 732f 656e 2f63 6f6c  p/lexemes/en/col
 000018c0: 6f72 5f70 6963 6b65 725f 6469 616c 6f67  or_picker_dialog
 000018d0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
 000018e0: 0073 1e01 0000 0202 0201 0201 0201 0201  .s..............
 000018f0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00001900: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00001910: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00001920: 0201 0201 0201 0201 0201 0201 0201 0201  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/common.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 6009 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,340 +1,342 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 7917 0000  a.......(..fy...
+00000000: 610d 0d0a 0000 0000 42a9 3566 9c17 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0054 0000 0040 0000 0073 b000 0000 6400  .T...@...s....d.
+00000020: 0055 0000 0040 0000 0073 b200 0000 6400  .U...@...s....d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6403 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 641e 641f 6423 6424 6425  d d!d"d.d.d#d$d%
 00000080: 6426 6427 6428 6429 642a 642b 642c 642b  d&d'd(d)d*d+d,d+
 00000090: 642d 642e 6424 642e 6426 6429 642a 642f  d-d.d$d.d&d)d*d/
 000000a0: 6430 642a 6431 6432 6433 6434 6435 6436  d0d*d1d2d3d4d5d6
 000000b0: 6437 6438 6439 643a 643b 643c 643d 643e  d7d8d9d:d;d<d=d>
 000000c0: 643f 6440 6441 6442 6443 6444 6445 6446  d?d@dAdBdCdDdEdF
-000000d0: 6447 6448 6449 9c53 5a00 644a 5300 294b  dGdHdI.SZ.dJS.)K
-000000e0: 7a0b 4e61 6d65 2045 6469 746f 727a 197b  z.Name Editorz.{
-000000f0: 6170 705f 7469 746c 657d 202d 207b 7375  app_title} - {su
-00000100: 625f 7469 746c 657d 7a11 4669 6c65 2066  b_title}z.File f
-00000110: 696c 7465 7220 6669 656c 645a 0652 656e  ilter fieldZ.Ren
-00000120: 616d 65da 0644 656c 6574 657a 1144 656c  ame..Deletez.Del
-00000130: 6574 6520 636f 6d70 6c65 7465 6c79 5a07  ete completelyZ.
-00000140: 5265 7374 6f72 657a 0b52 656e 616d 6520  Restorez.Rename 
-00000150: 6669 6c65 7a13 456e 7465 7220 6e65 7720  filez.Enter new 
-00000160: 6669 6c65 206e 616d 657a 2646 696c 6520  file namez&File 
-00000170: 7769 7468 2074 6865 2073 616d 6520 6e61  with the same na
-00000180: 6d65 2061 6c72 6561 6479 2065 7869 7374  me already exist
-00000190: 737a 0b44 656c 6574 6520 6669 6c65 7a1a  sz.Delete filez.
-000001a0: 4465 6c65 7465 2066 696c 6520 227b 6669  Delete file "{fi
-000001b0: 6c65 5f6e 616d 657d 223f 7a16 4465 6c65  le_name}"?z.Dele
-000001c0: 7465 2066 696c 6520 636f 6d70 6c65 7465  te file complete
-000001d0: 6c79 7a25 4465 6c65 7465 2066 696c 6520  lyz%Delete file 
-000001e0: 227b 6669 6c65 5f6e 616d 657d 2220 636f  "{file_name}" co
-000001f0: 6d70 6c65 7465 6c79 3f7a 2243 616e 6e6f  mpletely?z"Canno
-00000200: 7420 6465 6c65 7465 2066 696c 652c 2065  t delete file, e
-00000210: 7272 6f72 206f 6363 7572 7265 647a 0e46  rror occurredz.F
-00000220: 696c 6520 6e6f 7420 666f 756e 647a 0c52  ile not foundz.R
-00000230: 6573 746f 7265 2066 696c 657a 1b52 6573  estore filez.Res
-00000240: 746f 7265 2066 696c 6520 227b 6669 6c65  tore file "{file
-00000250: 5f6e 616d 657d 223f 7a23 4361 6e6e 6f74  _name}"?z#Cannot
-00000260: 2072 6573 746f 7265 2066 696c 652c 2065   restore file, e
-00000270: 7272 6f72 206f 6363 7572 7265 647a 2d46  rror occurredz-F
-00000280: 696c 6520 7769 7468 2074 6865 206e 616d  ile with the nam
-00000290: 6520 7b66 696c 655f 6e61 6d65 7d20 616c  e {file_name} al
-000002a0: 7265 6164 7920 6578 6973 7473 da07 4d65  ready exists..Me
-000002b0: 7373 6167 65da 0543 6c6f 7365 7a0c 4e65  ssage..Closez.Ne
-000002c0: 7720 646f 6375 6d65 6e74 7a09 4f70 656e  w documentz.Open
-000002d0: 2046 696c 657a 0953 6176 6520 4669 6c65   Filez.Save File
-000002e0: 7a0f 5361 7665 2065 6d70 7479 2066 696c  z.Save empty fil
-000002f0: 657a 2d41 6c6c 6f77 2074 6f20 7361 7665  ez-Allow to save
-00000300: 2074 6865 2066 696c 6520 7769 7468 2061   the file with a
-00000310: 6e20 656d 7074 7920 636f 6e74 656e 743f  n empty content?
-00000320: 7a0c 456e 6372 7970 7420 6669 6c65 7a1b  z.Encrypt filez.
-00000330: 456e 6372 7970 7420 6669 6c65 2022 7b66  Encrypt file "{f
-00000340: 696c 655f 6e61 6d65 7d22 3f7a 1e54 6865  ile_name}"?z.The
-00000350: 2066 696c 6520 6973 2061 6c72 6561 6479   file is already
-00000360: 2065 6e63 7279 7074 6564 217a 1552 6577   encrypted!z.Rew
-00000370: 7269 7465 2065 7869 7374 696e 6720 6669  rite existing fi
-00000380: 6c65 7a24 5265 7772 6974 6520 6578 6973  lez$Rewrite exis
-00000390: 7469 6e67 2066 696c 6520 227b 6669 6c65  ting file "{file
-000003a0: 5f70 6174 687d 223f 7a0c 4465 6372 7970  _path}"?z.Decryp
-000003b0: 7420 6669 6c65 7a1b 4465 6372 7970 7420  t filez.Decrypt 
-000003c0: 6669 6c65 2022 7b66 696c 655f 6e61 6d65  file "{file_name
-000003d0: 7d22 3f7a 1a54 6865 2066 696c 6520 6973  }"?z.The file is
-000003e0: 206e 6f74 2065 6e63 7279 7074 6564 217a   not encrypted!z
-000003f0: 0c4e 6577 2050 6173 7377 6f72 647a 0950  .New Passwordz.P
-00000400: 6173 7377 6f72 643a 7a12 456e 7465 7220  assword:z.Enter 
-00000410: 4e65 7720 5061 7373 776f 7264 7a05 4869  New Passwordz.Hi
-00000420: 6e74 3a7a bc54 6865 2068 696e 7420 6973  nt:z.The hint is
-00000430: 206e 6f74 2065 6e63 7279 7074 6564 2061   not encrypted a
-00000440: 6e64 2063 616e 2062 6520 7265 6164 2066  nd can be read f
-00000450: 726f 6d20 7468 6520 6669 6c65 210a 4176  rom the file!.Av
-00000460: 6f69 6420 6f62 7669 6f75 7320 6869 6e74  oid obvious hint
-00000470: 7320 7468 6174 2063 616e 2062 6520 6561  s that can be ea
-00000480: 7369 6c79 2067 7565 7373 6564 2c20 7375  sily guessed, su
-00000490: 6368 2061 7320 6269 7274 6820 6461 7465  ch as birth date
-000004a0: 732e 0a54 7279 2074 6f20 7573 6520 6120  s..Try to use a 
-000004b0: 7265 6665 7265 6e63 6520 7468 6174 2069  reference that i
-000004c0: 7320 6e6f 7420 6561 7369 6c79 2061 7373  s not easily ass
-000004d0: 6f63 6961 7465 6420 7769 7468 2079 6f75  ociated with you
-000004e0: 2e7a 1545 6e74 6572 2048 696e 7420 284f  .z.Enter Hint (O
-000004f0: 7074 696f 6e61 6c29 da02 4f4b da06 4361  ptional)..OK..Ca
-00000500: 6e63 656c da07 5761 726e 696e 677a 2354  ncel..Warningz#T
-00000510: 6865 2070 6173 7377 6f72 6420 6669 656c  he password fiel
-00000520: 6420 6361 6e6e 6f74 2062 6520 656d 7074  d cannot be empt
-00000530: 7921 7a39 5468 6520 6869 6e74 2066 6965  y!z9The hint fie
-00000540: 6c64 2069 7320 746f 6f20 6c6f 6e67 2c20  ld is too long, 
-00000550: 6d61 7869 6d75 6d20 7b73 796d 626f 6c73  maximum {symbols
-00000560: 7d20 6368 6172 6163 7465 7273 217a 0e45  } characters!z.E
-00000570: 6e74 6572 2050 6173 7377 6f72 647a 1952  nter Passwordz.R
-00000580: 6573 6574 2045 6e63 7279 7074 696f 6e20  eset Encryption 
-00000590: 5061 7373 776f 7264 7a3f 4172 6520 796f  Passwordz?Are yo
-000005a0: 7520 7375 7265 2079 6f75 2077 616e 7420  u sure you want 
-000005b0: 746f 2072 6573 6574 2074 6865 2063 7572  to reset the cur
-000005c0: 7265 6e74 2065 6e63 7279 7074 696f 6e20  rent encryption 
-000005d0: 7061 7373 776f 7264 3fda 0359 6573 da04  password?..Yes..
-000005e0: 4c69 6e6b 7a1f 4f70 656e 206c 696e 6b20  Linkz.Open link 
-000005f0: 227b 7572 6c7d 2220 696e 2061 2062 726f  "{url}" in a bro
-00000600: 7773 6572 3f7a 1d45 6e63 7279 7074 696f  wser?z.Encryptio
-00000610: 6e20 7061 7373 776f 7264 206d 6973 6d61  n password misma
-00000620: 7463 6821 7a1e 496e 636f 7272 6563 7420  tch!z.Incorrect 
-00000630: 656e 6372 7970 7469 6f6e 2070 6173 7377  encryption passw
-00000640: 6f72 6421 7a16 4669 6c65 2063 616e 6e6f  ord!z.File canno
-00000650: 7420 6265 206c 6f61 6465 642e 7a20 4361  t be loaded.z Ca
-00000660: 6e6e 6f74 2073 6176 6520 6669 6c65 2c20  nnot save file, 
-00000670: 6572 726f 7220 6f63 6375 7272 6564 7a0c  error occurredz.
-00000680: 4d6f 7265 2069 6e66 6f2e 2e2e 7a2f 466f  More info...z/Fo
-00000690: 726d 6174 7465 6420 7465 7874 2068 6173  rmatted text has
-000006a0: 2062 6565 6e20 636f 7069 6564 2074 6f20   been copied to 
-000006b0: 7468 6520 636c 6970 626f 6172 647a 1041  the clipboardz.A
-000006c0: 7070 6c69 6361 7469 6f6e 2049 6e66 6f7a  pplication Infoz
-000006d0: 0f4d 6172 6b64 6f77 6e20 4564 6974 6f72  .Markdown Editor
-000006e0: da07 5665 7273 696f 6e5a 074c 6963 656e  ..VersionZ.Licen
-000006f0: 7365 5a07 5765 6273 6974 655a 0647 6974  seZ.WebsiteZ.Git
-00000700: 4875 625a 0444 6174 657a 3841 206e 6577  HubZ.Datez8A new
-00000710: 2076 6572 7369 6f6e 2027 7b6c 6174 6573   version '{lates
-00000720: 745f 7665 7273 696f 6e7d 2720 6f66 2074  t_version}' of t
-00000730: 6865 2061 7070 2069 7320 6176 6169 6c61  he app is availa
-00000740: 626c 657a 2a54 6865 206c 6174 6573 7420  blez*The latest 
-00000750: 7665 7273 696f 6e20 6f66 2074 6865 2061  version of the a
-00000760: 7070 2069 7320 696e 7374 616c 6c65 647a  pp is installedz
-00000770: 2243 616e 6e6f 7420 6f62 7461 696e 2072  "Cannot obtain r
-00000780: 6573 706f 6e73 6520 696e 666f 726d 6174  esponse informat
-00000790: 696f 6e7a 4a48 6f73 7420 6e6f 7420 666f  ionzJHost not fo
-000007a0: 756e 642e 2054 6865 7265 206d 6179 2062  und. There may b
-000007b0: 6520 616e 2069 7373 7565 2077 6974 6820  e an issue with 
-000007c0: 7468 6520 696e 7465 726e 6574 2063 6f6e  the internet con
-000007d0: 6e65 6374 696f 6e20 6f72 2044 4e53 2e7a  nection or DNS.z
-000007e0: 4d43 6f6e 6e65 6374 696f 6e20 7265 6675  MConnection refu
-000007f0: 7365 642e 2054 6865 2073 6572 7665 7220  sed. The server 
-00000800: 6d69 6768 7420 6265 2064 6f77 6e2c 206f  might be down, o
-00000810: 7220 7468 6572 6520 6d61 7920 6265 206e  r there may be n
-00000820: 6574 776f 726b 2069 7373 7565 732e 7a32  etwork issues.z2
-00000830: 436f 6e6e 6563 7469 6f6e 2074 696d 6564  Connection timed
-00000840: 206f 7574 2e20 5468 6572 6520 6d61 7920   out. There may 
-00000850: 6265 206e 6574 776f 726b 2069 7373 7565  be network issue
-00000860: 732e 7a42 436f 6e6e 6563 7469 6f6e 2034  s.zBConnection 4
-00000870: 3034 2065 7272 6f72 2e20 5468 6520 7265  04 error. The re
-00000880: 7175 6573 7465 6420 7061 6765 206f 7220  quested page or 
-00000890: 7265 736f 7572 6365 2069 7320 6e6f 7420  resource is not 
-000008a0: 666f 756e 642e 7a2e 5265 7175 6573 7420  found.z.Request 
-000008b0: 6661 696c 6564 2077 6974 6820 7374 6174  failed with stat
-000008c0: 7573 2063 6f64 653a 207b 7374 6174 7573  us code: {status
-000008d0: 5f63 6f64 657d 2953 da09 6170 705f 7469  _code})S..app_ti
-000008e0: 746c 65da 1261 7070 5f74 6974 6c65 5f77  tle..app_title_w
-000008f0: 6974 685f 7375 62da 1b74 7265 655f 6669  ith_sub..tree_fi
-00000900: 6c74 6572 5f61 6363 6573 7369 626c 655f  lter_accessible_
-00000910: 6465 7363 da12 6d65 6e75 5f61 6374 696f  desc..menu_actio
-00000920: 6e5f 7265 6e61 6d65 da12 6d65 6e75 5f61  n_rename..menu_a
-00000930: 6374 696f 6e5f 6465 6c65 7465 da1d 6d65  ction_delete..me
-00000940: 6e75 5f61 6374 696f 6e5f 6465 6c65 7465  nu_action_delete
-00000950: 5f63 6f6d 706c 6574 656c 79da 136d 656e  _completely..men
-00000960: 755f 6163 7469 6f6e 5f72 6573 746f 7265  u_action_restore
-00000970: da18 6469 616c 6f67 5f66 696c 655f 7265  ..dialog_file_re
-00000980: 6e61 6d65 5f74 6974 6c65 da1e 6469 616c  name_title..dial
-00000990: 6f67 5f66 696c 655f 7265 6e61 6d65 5f66  og_file_rename_f
-000009a0: 6965 6c64 5f6c 6162 656c da1c 6469 616c  ield_label..dial
-000009b0: 6f67 5f66 696c 655f 7265 6e61 6d65 5f62  og_file_rename_b
-000009c0: 7574 746f 6e5f 6f6b da21 6469 616c 6f67  utton_ok.!dialog
-000009d0: 5f66 696c 655f 7265 6e61 6d65 5f77 6172  _file_rename_war
-000009e0: 6e69 6e67 5f65 7869 7374 73da 1864 6961  ning_exists..dia
-000009f0: 6c6f 675f 6669 6c65 5f64 656c 6574 655f  log_file_delete_
-00000a00: 7469 746c 65da 1764 6961 6c6f 675f 6669  title..dialog_fi
-00000a10: 6c65 5f64 656c 6574 655f 7465 7874 da23  le_delete_text.#
-00000a20: 6469 616c 6f67 5f66 696c 655f 6465 6c65  dialog_file_dele
-00000a30: 7465 5f63 6f6d 706c 6574 656c 795f 7469  te_completely_ti
-00000a40: 746c 65da 2264 6961 6c6f 675f 6669 6c65  tle."dialog_file
-00000a50: 5f64 656c 6574 655f 636f 6d70 6c65 7465  _delete_complete
-00000a60: 6c79 5f74 6578 74da 1864 6961 6c6f 675f  ly_text..dialog_
-00000a70: 6669 6c65 5f64 656c 6574 655f 6572 726f  file_delete_erro
-00000a80: 72da 2264 6961 6c6f 675f 6669 6c65 5f64  r."dialog_file_d
-00000a90: 656c 6574 655f 6572 726f 725f 6e6f 745f  elete_error_not_
-00000aa0: 666f 756e 64da 1964 6961 6c6f 675f 6669  found..dialog_fi
-00000ab0: 6c65 5f72 6573 746f 7265 5f74 6974 6c65  le_restore_title
-00000ac0: da18 6469 616c 6f67 5f66 696c 655f 7265  ..dialog_file_re
-00000ad0: 7374 6f72 655f 7465 7874 5a19 6469 616c  store_textZ.dial
-00000ae0: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
-00000af0: 6572 726f 72da 2264 6961 6c6f 675f 6669  error."dialog_fi
-00000b00: 6c65 5f72 6573 746f 7265 5f77 6172 6e69  le_restore_warni
-00000b10: 6e67 5f65 7869 7374 73da 1864 6961 6c6f  ng_exists..dialo
-00000b20: 675f 6d65 7373 6167 655f 626f 785f 7469  g_message_box_ti
-00000b30: 746c 65da 1c64 6961 6c6f 675f 6d65 7373  tle..dialog_mess
-00000b40: 6167 655f 626f 785f 6275 7474 6f6e 5f6f  age_box_button_o
-00000b50: 6bda 2861 6374 696f 6e5f 6e65 775f 6669  k.(action_new_fi
-00000b60: 6c65 5f66 6972 7374 5f6c 696e 655f 7465  le_first_line_te
-00000b70: 6d70 6c61 7465 5f74 6578 74da 1f61 6374  mplate_text..act
-00000b80: 696f 6e5f 6f70 656e 5f66 696c 655f 6469  ion_open_file_di
-00000b90: 616c 6f67 5f63 6170 7469 6f6e da22 6163  alog_caption."ac
-00000ba0: 7469 6f6e 5f73 6176 655f 6173 5f66 696c  tion_save_as_fil
-00000bb0: 655f 6469 616c 6f67 5f63 6170 7469 6f6e  e_dialog_caption
-00000bc0: da1c 6469 616c 6f67 5f73 6176 655f 656d  ..dialog_save_em
-00000bd0: 7074 795f 6669 6c65 5f74 6974 6c65 da1b  pty_file_title..
-00000be0: 6469 616c 6f67 5f73 6176 655f 656d 7074  dialog_save_empt
-00000bf0: 795f 6669 6c65 5f74 6578 74da 1964 6961  y_file_text..dia
-00000c00: 6c6f 675f 656e 6372 7970 745f 6669 6c65  log_encrypt_file
-00000c10: 5f74 6974 6c65 da18 6469 616c 6f67 5f65  _title..dialog_e
-00000c20: 6e63 7279 7074 5f66 696c 655f 7465 7874  ncrypt_file_text
-00000c30: da2e 656e 6372 7970 745f 6669 6c65 5f77  ..encrypt_file_w
-00000c40: 6172 6e69 6e67 5f66 696c 655f 6973 5f61  arning_file_is_a
-00000c50: 6c72 6561 6479 5f65 6e63 7279 7074 6564  lready_encrypted
-00000c60: da2a 6469 616c 6f67 5f65 6e63 7279 7074  .*dialog_encrypt
-00000c70: 5f66 696c 655f 7265 7772 6974 655f 6578  _file_rewrite_ex
-00000c80: 6973 7469 6e67 5f74 6974 6c65 da29 6469  isting_title.)di
-00000c90: 616c 6f67 5f65 6e63 7279 7074 5f66 696c  alog_encrypt_fil
-00000ca0: 655f 7265 7772 6974 655f 6578 6973 7469  e_rewrite_existi
-00000cb0: 6e67 5f74 6578 74da 1964 6961 6c6f 675f  ng_text..dialog_
-00000cc0: 6465 6372 7970 745f 6669 6c65 5f74 6974  decrypt_file_tit
-00000cd0: 6c65 da18 6469 616c 6f67 5f64 6563 7279  le..dialog_decry
-00000ce0: 7074 5f66 696c 655f 7465 7874 da2a 6465  pt_file_text.*de
-00000cf0: 6372 7970 745f 6669 6c65 5f77 6172 6e69  crypt_file_warni
-00000d00: 6e67 5f66 696c 655f 6973 5f6e 6f74 5f65  ng_file_is_not_e
-00000d10: 6e63 7279 7074 6564 da2a 6469 616c 6f67  ncrypted.*dialog
-00000d20: 5f64 6563 7279 7074 5f66 696c 655f 7265  _decrypt_file_re
-00000d30: 7772 6974 655f 6578 6973 7469 6e67 5f74  write_existing_t
-00000d40: 6974 6c65 da29 6469 616c 6f67 5f64 6563  itle.)dialog_dec
-00000d50: 7279 7074 5f66 696c 655f 7265 7772 6974  rypt_file_rewrit
-00000d60: 655f 6578 6973 7469 6e67 5f74 6578 74da  e_existing_text.
-00000d70: 2164 6961 6c6f 675f 656e 6372 7970 745f  !dialog_encrypt_
-00000d80: 6e65 775f 7061 7373 776f 7264 5f74 6974  new_password_tit
-00000d90: 6c65 da21 6469 616c 6f67 5f65 6e63 7279  le.!dialog_encry
-00000da0: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
-00000db0: 6c61 6265 6cda 3264 6961 6c6f 675f 656e  label.2dialog_en
-00000dc0: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00000dd0: 7264 5f69 6e70 7574 5f70 6c61 6365 686f  rd_input_placeho
-00000de0: 6c64 6572 5f74 6578 74da 2664 6961 6c6f  lder_text.&dialo
-00000df0: 675f 656e 6372 7970 745f 6e65 775f 7061  g_encrypt_new_pa
-00000e00: 7373 776f 7264 5f68 696e 745f 6c61 6265  ssword_hint_labe
-00000e10: 6cda 3264 6961 6c6f 675f 656e 6372 7970  l.2dialog_encryp
-00000e20: 745f 6e65 775f 7061 7373 776f 7264 5f68  t_new_password_h
-00000e30: 696e 745f 6c61 6265 6c5f 6465 7363 7269  int_label_descri
-00000e40: 7074 696f 6eda 3764 6961 6c6f 675f 656e  ption.7dialog_en
-00000e50: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00000e60: 7264 5f68 696e 745f 696e 7075 745f 706c  rd_hint_input_pl
-00000e70: 6163 6568 6f6c 6465 725f 7465 7874 da25  aceholder_text.%
-00000e80: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
-00000e90: 6577 5f70 6173 7377 6f72 645f 6275 7474  ew_password_butt
-00000ea0: 6f6e 5f6f 6bda 2964 6961 6c6f 675f 656e  on_ok.)dialog_en
-00000eb0: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00000ec0: 7264 5f62 7574 746f 6e5f 6361 6e63 656c  rd_button_cancel
-00000ed0: da2f 6469 616c 6f67 5f65 6e63 7279 7074  ./dialog_encrypt
-00000ee0: 5f6e 6577 5f70 6173 7377 6f72 645f 7761  _new_password_wa
-00000ef0: 726e 696e 675f 656d 7074 795f 7469 746c  rning_empty_titl
-00000f00: 65da 2e64 6961 6c6f 675f 656e 6372 7970  e..dialog_encryp
-00000f10: 745f 6e65 775f 7061 7373 776f 7264 5f77  t_new_password_w
-00000f20: 6172 6e69 6e67 5f65 6d70 7479 5f74 6578  arning_empty_tex
-00000f30: 74da 3264 6961 6c6f 675f 656e 6372 7970  t.2dialog_encryp
-00000f40: 745f 6e65 775f 7061 7373 776f 7264 5f77  t_new_password_w
-00000f50: 6172 6e69 6e67 5f74 6f6f 5f6c 6f6e 675f  arning_too_long_
-00000f60: 7469 746c 65da 3164 6961 6c6f 675f 656e  title.1dialog_en
-00000f70: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00000f80: 7264 5f77 6172 6e69 6e67 5f74 6f6f 5f6c  rd_warning_too_l
-00000f90: 6f6e 675f 7465 7874 da1d 6469 616c 6f67  ong_text..dialog
-00000fa0: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
-00000fb0: 645f 7469 746c 65da 1d64 6961 6c6f 675f  d_title..dialog_
-00000fc0: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
-00000fd0: 5f6c 6162 656c da2e 6469 616c 6f67 5f65  _label..dialog_e
-00000fe0: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
-00000ff0: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
-00001000: 725f 7465 7874 da22 6469 616c 6f67 5f65  r_text."dialog_e
-00001010: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
-00001020: 6869 6e74 5f6c 6162 656c da21 6469 616c  hint_label.!dial
-00001030: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
-00001040: 6f72 645f 6275 7474 6f6e 5f6f 6bda 2564  ord_button_ok.%d
-00001050: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
-00001060: 7373 776f 7264 5f62 7574 746f 6e5f 6361  ssword_button_ca
-00001070: 6e63 656c da23 6469 616c 6f67 5f65 6e63  ncel.#dialog_enc
-00001080: 7279 7074 5f70 6173 7377 6f72 645f 7265  rypt_password_re
-00001090: 7365 745f 7469 746c 65da 2264 6961 6c6f  set_title."dialo
-000010a0: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
-000010b0: 7264 5f72 6573 6574 5f74 6578 74da 2b64  rd_reset_text.+d
-000010c0: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
-000010d0: 7373 776f 7264 5f72 6573 6574 5f62 7574  ssword_reset_but
-000010e0: 746f 6e5f 6361 6e63 656c da28 6469 616c  ton_cancel.(dial
-000010f0: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
-00001100: 6f72 645f 7265 7365 745f 6275 7474 6f6e  ord_reset_button
-00001110: 5f79 6573 da16 6469 616c 6f67 5f6f 7065  _yes..dialog_ope
-00001120: 6e5f 6c69 6e6b 5f74 6974 6c65 da15 6469  n_link_title..di
-00001130: 616c 6f67 5f6f 7065 6e5f 6c69 6e6b 5f74  alog_open_link_t
-00001140: 6578 74da 266c 6f61 645f 6669 6c65 5f65  ext.&load_file_e
-00001150: 6e63 7279 7074 696f 6e5f 7061 7373 776f  ncryption_passwo
-00001160: 7264 5f6d 6973 6d61 7463 68da 276c 6f61  rd_mismatch.'loa
-00001170: 645f 6669 6c65 5f65 6e63 7279 7074 696f  d_file_encryptio
-00001180: 6e5f 7061 7373 776f 7264 5f69 6e63 6f72  n_password_incor
-00001190: 7265 6374 da1c 6c6f 6164 5f66 696c 655f  rect..load_file_
-000011a0: 6e6f 6e65 5f63 6f6e 7465 6e74 5f65 7272  none_content_err
-000011b0: 6f72 da1f 7361 7665 5f61 6374 6976 655f  or..save_active_
-000011c0: 6669 6c65 5f65 7272 6f72 5f6f 6363 7572  file_error_occur
-000011d0: 7265 64da 1e65 7870 616e 6461 626c 655f  red..expandable_
-000011e0: 626c 6f63 6b5f 6465 6661 756c 745f 7469  block_default_ti
-000011f0: 746c 65da 3164 6961 6c6f 675f 636f 6c6f  tle.1dialog_colo
-00001200: 725f 7069 636b 6572 5f63 6f6c 6f72 5f63  r_picker_color_c
-00001210: 6f70 6965 645f 746f 5f74 6865 5f63 6c69  opied_to_the_cli
-00001220: 7062 6f61 7264 da11 706f 7075 705f 6162  pboard..popup_ab
-00001230: 6f75 745f 7469 746c 65da 2070 6f70 7570  out_title. popup
-00001240: 5f61 626f 7574 5f61 7070 5f6e 616d 655f  _about_app_name_
-00001250: 6465 7363 7269 7074 696f 6eda 1370 6f70  description..pop
-00001260: 7570 5f61 626f 7574 5f76 6572 7369 6f6e  up_about_version
-00001270: da13 706f 7075 705f 6162 6f75 745f 6c69  ..popup_about_li
-00001280: 6365 6e73 65da 1370 6f70 7570 5f61 626f  cense..popup_abo
-00001290: 7574 5f77 6562 7369 7465 da16 706f 7075  ut_website..popu
-000012a0: 705f 6162 6f75 745f 7265 706f 7369 746f  p_about_reposito
-000012b0: 7279 da10 706f 7075 705f 6162 6f75 745f  ry..popup_about_
-000012c0: 6461 7465 da26 7570 6461 7465 5f68 656c  date.&update_hel
-000012d0: 7065 725f 6e65 775f 7665 7273 696f 6e5f  per_new_version_
-000012e0: 6973 5f61 7661 696c 6162 6c65 da26 7570  is_available.&up
-000012f0: 6461 7465 5f68 656c 7065 725f 6c61 7465  date_helper_late
-00001300: 7374 5f76 6572 7369 6f6e 5f69 6e73 7461  st_version_insta
-00001310: 6c6c 6564 da1e 6e65 7477 6f72 6b5f 636f  lled..network_co
-00001320: 6e6e 6563 7469 6f6e 5f65 7272 6f72 5f65  nnection_error_e
-00001330: 6d70 7479 da2a 6e65 7477 6f72 6b5f 636f  mpty.*network_co
-00001340: 6e6e 6563 7469 6f6e 5f65 7272 6f72 5f63  nnection_error_c
-00001350: 6f6e 6e65 6374 696f 6e5f 6f72 5f64 6e73  onnection_or_dns
-00001360: da2b 6e65 7477 6f72 6b5f 636f 6e6e 6563  .+network_connec
-00001370: 7469 6f6e 5f65 7272 6f72 5f63 6f6e 6e65  tion_error_conne
-00001380: 6374 696f 6e5f 7265 6675 7365 64da 2d6e  ction_refused.-n
-00001390: 6574 776f 726b 5f63 6f6e 6e65 6374 696f  etwork_connectio
-000013a0: 6e5f 6572 726f 725f 636f 6e6e 6563 7469  n_error_connecti
-000013b0: 6f6e 5f74 696d 6564 5f6f 7574 da2d 6e65  on_timed_out.-ne
-000013c0: 7477 6f72 6b5f 636f 6e6e 6563 7469 6f6e  twork_connection
-000013d0: 5f65 7272 6f72 5f63 6f6e 6e65 6374 696f  _error_connectio
-000013e0: 6e5f 3430 345f 6572 726f 72da 316e 6574  n_404_error.1net
-000013f0: 776f 726b 5f63 6f6e 6e65 6374 696f 6e5f  work_connection_
-00001400: 6572 726f 725f 6765 6e65 7269 635f 7769  error_generic_wi
-00001410: 7468 5f73 7461 7475 735f 636f 6465 4e29  th_status_codeN)
-00001420: 01da 076c 6578 656d 6573 a900 725d 0000  ...lexemes..r]..
-00001430: 0072 5d00 0000 fa43 2f55 7365 7273 2f76  .r]....C/Users/v
-00001440: 6164 696b 7573 2f50 7963 6861 726d 5072  adikus/PycharmPr
-00001450: 6f6a 6563 7473 2f6e 6f74 6f6c 6f67 2f6e  ojects/notolog/n
-00001460: 6f74 6f6c 6f67 2f6c 6578 656d 6573 2f65  otolog/lexemes/e
-00001470: 6e2f 636f 6d6d 6f6e 2e70 79da 083c 6d6f  n/common.py..<mo
-00001480: 6475 6c65 3e03 0000 0073 a600 0000 0201  dule>....s......
-00001490: 0202 0202 0201 0201 0201 0202 0201 0201  ................
-000014a0: 0201 0202 0201 0201 0201 0201 0201 0202  ................
-000014b0: 0201 0201 0201 0202 0201 0202 0201 0201  ................
-000014c0: 0202 0201 0202 0201 0201 0201 0201 0202  ................
-000014d0: 0201 0201 0201 0201 0202 0201 0201 0201  ................
-000014e0: 0201 0204 0201 0201 0201 0201 0201 0201  ................
-000014f0: 0202 0201 0201 0201 0201 0201 0202 0201  ................
-00001500: 0201 0201 0202 0201 0202 0201 0201 0202  ................
-00001510: 0202 0202 0202 0201 0202 0201 0201 0201  ................
-00001520: 0201 0202 0201 0202 0202 0202 0201 0202  ................
-00001530: 0201 0291                                ....
+000000d0: 6447 6448 6449 644a 9c54 5a00 644b 5300  dGdHdIdJ.TZ.dKS.
+000000e0: 294c 7a0e 4e6f 746f 6c6f 6720 4564 6974  )Lz.Notolog Edit
+000000f0: 6f72 7a19 7b61 7070 5f74 6974 6c65 7d20  orz.{app_title} 
+00000100: 2d20 7b73 7562 5f74 6974 6c65 7d7a 1146  - {sub_title}z.F
+00000110: 696c 6520 6669 6c74 6572 2066 6965 6c64  ile filter field
+00000120: 5a06 5265 6e61 6d65 da06 4465 6c65 7465  Z.Rename..Delete
+00000130: 7a11 4465 6c65 7465 2063 6f6d 706c 6574  z.Delete complet
+00000140: 656c 795a 0752 6573 746f 7265 7a0b 5265  elyZ.Restorez.Re
+00000150: 6e61 6d65 2066 696c 657a 1345 6e74 6572  name filez.Enter
+00000160: 206e 6577 2066 696c 6520 6e61 6d65 7a26   new file namez&
+00000170: 4669 6c65 2077 6974 6820 7468 6520 7361  File with the sa
+00000180: 6d65 206e 616d 6520 616c 7265 6164 7920  me name already 
+00000190: 6578 6973 7473 7a0b 4465 6c65 7465 2066  existsz.Delete f
+000001a0: 696c 657a 1a44 656c 6574 6520 6669 6c65  ilez.Delete file
+000001b0: 2022 7b66 696c 655f 6e61 6d65 7d22 3f7a   "{file_name}"?z
+000001c0: 1644 656c 6574 6520 6669 6c65 2063 6f6d  .Delete file com
+000001d0: 706c 6574 656c 797a 2544 656c 6574 6520  pletelyz%Delete 
+000001e0: 6669 6c65 2022 7b66 696c 655f 6e61 6d65  file "{file_name
+000001f0: 7d22 2063 6f6d 706c 6574 656c 793f 7a22  }" completely?z"
+00000200: 4361 6e6e 6f74 2064 656c 6574 6520 6669  Cannot delete fi
+00000210: 6c65 2c20 6572 726f 7220 6f63 6375 7272  le, error occurr
+00000220: 6564 7a0e 4669 6c65 206e 6f74 2066 6f75  edz.File not fou
+00000230: 6e64 7a0c 5265 7374 6f72 6520 6669 6c65  ndz.Restore file
+00000240: 7a1b 5265 7374 6f72 6520 6669 6c65 2022  z.Restore file "
+00000250: 7b66 696c 655f 6e61 6d65 7d22 3f7a 2343  {file_name}"?z#C
+00000260: 616e 6e6f 7420 7265 7374 6f72 6520 6669  annot restore fi
+00000270: 6c65 2c20 6572 726f 7220 6f63 6375 7272  le, error occurr
+00000280: 6564 7a2d 4669 6c65 2077 6974 6820 7468  edz-File with th
+00000290: 6520 6e61 6d65 207b 6669 6c65 5f6e 616d  e name {file_nam
+000002a0: 657d 2061 6c72 6561 6479 2065 7869 7374  e} already exist
+000002b0: 73da 074d 6573 7361 6765 da05 436c 6f73  s..Message..Clos
+000002c0: 657a 0c4e 6577 2064 6f63 756d 656e 747a  ez.New documentz
+000002d0: 094f 7065 6e20 4669 6c65 7a09 5361 7665  .Open Filez.Save
+000002e0: 2046 696c 657a 0f53 6176 6520 656d 7074   Filez.Save empt
+000002f0: 7920 6669 6c65 7a2d 416c 6c6f 7720 746f  y filez-Allow to
+00000300: 2073 6176 6520 7468 6520 6669 6c65 2077   save the file w
+00000310: 6974 6820 616e 2065 6d70 7479 2063 6f6e  ith an empty con
+00000320: 7465 6e74 3f7a 0c45 6e63 7279 7074 2066  tent?z.Encrypt f
+00000330: 696c 657a 1b45 6e63 7279 7074 2066 696c  ilez.Encrypt fil
+00000340: 6520 227b 6669 6c65 5f6e 616d 657d 223f  e "{file_name}"?
+00000350: 7a1e 5468 6520 6669 6c65 2069 7320 616c  z.The file is al
+00000360: 7265 6164 7920 656e 6372 7970 7465 6421  ready encrypted!
+00000370: 7a15 5265 7772 6974 6520 6578 6973 7469  z.Rewrite existi
+00000380: 6e67 2066 696c 657a 2452 6577 7269 7465  ng filez$Rewrite
+00000390: 2065 7869 7374 696e 6720 6669 6c65 2022   existing file "
+000003a0: 7b66 696c 655f 7061 7468 7d22 3f7a 0c44  {file_path}"?z.D
+000003b0: 6563 7279 7074 2066 696c 657a 1b44 6563  ecrypt filez.Dec
+000003c0: 7279 7074 2066 696c 6520 227b 6669 6c65  rypt file "{file
+000003d0: 5f6e 616d 657d 223f 7a1a 5468 6520 6669  _name}"?z.The fi
+000003e0: 6c65 2069 7320 6e6f 7420 656e 6372 7970  le is not encryp
+000003f0: 7465 6421 7a0c 4e65 7720 5061 7373 776f  ted!z.New Passwo
+00000400: 7264 7a09 5061 7373 776f 7264 3a7a 1245  rdz.Password:z.E
+00000410: 6e74 6572 204e 6577 2050 6173 7377 6f72  nter New Passwor
+00000420: 647a 0548 696e 743a 7abc 5468 6520 6869  dz.Hint:z.The hi
+00000430: 6e74 2069 7320 6e6f 7420 656e 6372 7970  nt is not encryp
+00000440: 7465 6420 616e 6420 6361 6e20 6265 2072  ted and can be r
+00000450: 6561 6420 6672 6f6d 2074 6865 2066 696c  ead from the fil
+00000460: 6521 0a41 766f 6964 206f 6276 696f 7573  e!.Avoid obvious
+00000470: 2068 696e 7473 2074 6861 7420 6361 6e20   hints that can 
+00000480: 6265 2065 6173 696c 7920 6775 6573 7365  be easily guesse
+00000490: 642c 2073 7563 6820 6173 2062 6972 7468  d, such as birth
+000004a0: 2064 6174 6573 2e0a 5472 7920 746f 2075   dates..Try to u
+000004b0: 7365 2061 2072 6566 6572 656e 6365 2074  se a reference t
+000004c0: 6861 7420 6973 206e 6f74 2065 6173 696c  hat is not easil
+000004d0: 7920 6173 736f 6369 6174 6564 2077 6974  y associated wit
+000004e0: 6820 796f 752e 7a15 456e 7465 7220 4869  h you.z.Enter Hi
+000004f0: 6e74 2028 4f70 7469 6f6e 616c 29da 024f  nt (Optional)..O
+00000500: 4bda 0643 616e 6365 6cda 0757 6172 6e69  K..Cancel..Warni
+00000510: 6e67 7a23 5468 6520 7061 7373 776f 7264  ngz#The password
+00000520: 2066 6965 6c64 2063 616e 6e6f 7420 6265   field cannot be
+00000530: 2065 6d70 7479 217a 3954 6865 2068 696e   empty!z9The hin
+00000540: 7420 6669 656c 6420 6973 2074 6f6f 206c  t field is too l
+00000550: 6f6e 672c 206d 6178 696d 756d 207b 7379  ong, maximum {sy
+00000560: 6d62 6f6c 737d 2063 6861 7261 6374 6572  mbols} character
+00000570: 7321 7a0e 456e 7465 7220 5061 7373 776f  s!z.Enter Passwo
+00000580: 7264 7a19 5265 7365 7420 456e 6372 7970  rdz.Reset Encryp
+00000590: 7469 6f6e 2050 6173 7377 6f72 647a 3f41  tion Passwordz?A
+000005a0: 7265 2079 6f75 2073 7572 6520 796f 7520  re you sure you 
+000005b0: 7761 6e74 2074 6f20 7265 7365 7420 7468  want to reset th
+000005c0: 6520 6375 7272 656e 7420 656e 6372 7970  e current encryp
+000005d0: 7469 6f6e 2070 6173 7377 6f72 643f da03  tion password?..
+000005e0: 5965 73da 044c 696e 6b7a 1f4f 7065 6e20  Yes..Linkz.Open 
+000005f0: 6c69 6e6b 2022 7b75 726c 7d22 2069 6e20  link "{url}" in 
+00000600: 6120 6272 6f77 7365 723f 7a1d 456e 6372  a browser?z.Encr
+00000610: 7970 7469 6f6e 2070 6173 7377 6f72 6420  yption password 
+00000620: 6d69 736d 6174 6368 217a 1e49 6e63 6f72  mismatch!z.Incor
+00000630: 7265 6374 2065 6e63 7279 7074 696f 6e20  rect encryption 
+00000640: 7061 7373 776f 7264 217a 1646 696c 6520  password!z.File 
+00000650: 6361 6e6e 6f74 2062 6520 6c6f 6164 6564  cannot be loaded
+00000660: 2e7a 2043 616e 6e6f 7420 7361 7665 2066  .z Cannot save f
+00000670: 696c 652c 2065 7272 6f72 206f 6363 7572  ile, error occur
+00000680: 7265 647a 0c4d 6f72 6520 696e 666f 2e2e  redz.More info..
+00000690: 2e7a 2f46 6f72 6d61 7474 6564 2074 6578  .z/Formatted tex
+000006a0: 7420 6861 7320 6265 656e 2063 6f70 6965  t has been copie
+000006b0: 6420 746f 2074 6865 2063 6c69 7062 6f61  d to the clipboa
+000006c0: 7264 7a10 4170 706c 6963 6174 696f 6e20  rdz.Application 
+000006d0: 496e 666f 7a0f 4d61 726b 646f 776e 2045  Infoz.Markdown E
+000006e0: 6469 746f 72da 0756 6572 7369 6f6e 5a07  ditor..VersionZ.
+000006f0: 4c69 6365 6e73 655a 0757 6562 7369 7465  LicenseZ.Website
+00000700: da06 4769 7448 7562 da04 5079 5069 5a04  ..GitHub..PyPiZ.
+00000710: 4461 7465 7a38 4120 6e65 7720 7665 7273  Datez8A new vers
+00000720: 696f 6e20 277b 6c61 7465 7374 5f76 6572  ion '{latest_ver
+00000730: 7369 6f6e 7d27 206f 6620 7468 6520 6170  sion}' of the ap
+00000740: 7020 6973 2061 7661 696c 6162 6c65 7a2a  p is availablez*
+00000750: 5468 6520 6c61 7465 7374 2076 6572 7369  The latest versi
+00000760: 6f6e 206f 6620 7468 6520 6170 7020 6973  on of the app is
+00000770: 2069 6e73 7461 6c6c 6564 7a22 4361 6e6e   installedz"Cann
+00000780: 6f74 206f 6274 6169 6e20 7265 7370 6f6e  ot obtain respon
+00000790: 7365 2069 6e66 6f72 6d61 7469 6f6e 7a4a  se informationzJ
+000007a0: 486f 7374 206e 6f74 2066 6f75 6e64 2e20  Host not found. 
+000007b0: 5468 6572 6520 6d61 7920 6265 2061 6e20  There may be an 
+000007c0: 6973 7375 6520 7769 7468 2074 6865 2069  issue with the i
+000007d0: 6e74 6572 6e65 7420 636f 6e6e 6563 7469  nternet connecti
+000007e0: 6f6e 206f 7220 444e 532e 7a4d 436f 6e6e  on or DNS.zMConn
+000007f0: 6563 7469 6f6e 2072 6566 7573 6564 2e20  ection refused. 
+00000800: 5468 6520 7365 7276 6572 206d 6967 6874  The server might
+00000810: 2062 6520 646f 776e 2c20 6f72 2074 6865   be down, or the
+00000820: 7265 206d 6179 2062 6520 6e65 7477 6f72  re may be networ
+00000830: 6b20 6973 7375 6573 2e7a 3243 6f6e 6e65  k issues.z2Conne
+00000840: 6374 696f 6e20 7469 6d65 6420 6f75 742e  ction timed out.
+00000850: 2054 6865 7265 206d 6179 2062 6520 6e65   There may be ne
+00000860: 7477 6f72 6b20 6973 7375 6573 2e7a 4243  twork issues.zBC
+00000870: 6f6e 6e65 6374 696f 6e20 3430 3420 6572  onnection 404 er
+00000880: 726f 722e 2054 6865 2072 6571 7565 7374  ror. The request
+00000890: 6564 2070 6167 6520 6f72 2072 6573 6f75  ed page or resou
+000008a0: 7263 6520 6973 206e 6f74 2066 6f75 6e64  rce is not found
+000008b0: 2e7a 2e52 6571 7565 7374 2066 6169 6c65  .z.Request faile
+000008c0: 6420 7769 7468 2073 7461 7475 7320 636f  d with status co
+000008d0: 6465 3a20 7b73 7461 7475 735f 636f 6465  de: {status_code
+000008e0: 7d29 54da 0961 7070 5f74 6974 6c65 da12  })T..app_title..
+000008f0: 6170 705f 7469 746c 655f 7769 7468 5f73  app_title_with_s
+00000900: 7562 da1b 7472 6565 5f66 696c 7465 725f  ub..tree_filter_
+00000910: 6163 6365 7373 6962 6c65 5f64 6573 63da  accessible_desc.
+00000920: 126d 656e 755f 6163 7469 6f6e 5f72 656e  .menu_action_ren
+00000930: 616d 65da 126d 656e 755f 6163 7469 6f6e  ame..menu_action
+00000940: 5f64 656c 6574 65da 1d6d 656e 755f 6163  _delete..menu_ac
+00000950: 7469 6f6e 5f64 656c 6574 655f 636f 6d70  tion_delete_comp
+00000960: 6c65 7465 6c79 da13 6d65 6e75 5f61 6374  letely..menu_act
+00000970: 696f 6e5f 7265 7374 6f72 65da 1864 6961  ion_restore..dia
+00000980: 6c6f 675f 6669 6c65 5f72 656e 616d 655f  log_file_rename_
+00000990: 7469 746c 65da 1e64 6961 6c6f 675f 6669  title..dialog_fi
+000009a0: 6c65 5f72 656e 616d 655f 6669 656c 645f  le_rename_field_
+000009b0: 6c61 6265 6cda 1c64 6961 6c6f 675f 6669  label..dialog_fi
+000009c0: 6c65 5f72 656e 616d 655f 6275 7474 6f6e  le_rename_button
+000009d0: 5f6f 6bda 2164 6961 6c6f 675f 6669 6c65  _ok.!dialog_file
+000009e0: 5f72 656e 616d 655f 7761 726e 696e 675f  _rename_warning_
+000009f0: 6578 6973 7473 da18 6469 616c 6f67 5f66  exists..dialog_f
+00000a00: 696c 655f 6465 6c65 7465 5f74 6974 6c65  ile_delete_title
+00000a10: da17 6469 616c 6f67 5f66 696c 655f 6465  ..dialog_file_de
+00000a20: 6c65 7465 5f74 6578 74da 2364 6961 6c6f  lete_text.#dialo
+00000a30: 675f 6669 6c65 5f64 656c 6574 655f 636f  g_file_delete_co
+00000a40: 6d70 6c65 7465 6c79 5f74 6974 6c65 da22  mpletely_title."
+00000a50: 6469 616c 6f67 5f66 696c 655f 6465 6c65  dialog_file_dele
+00000a60: 7465 5f63 6f6d 706c 6574 656c 795f 7465  te_completely_te
+00000a70: 7874 da18 6469 616c 6f67 5f66 696c 655f  xt..dialog_file_
+00000a80: 6465 6c65 7465 5f65 7272 6f72 da22 6469  delete_error."di
+00000a90: 616c 6f67 5f66 696c 655f 6465 6c65 7465  alog_file_delete
+00000aa0: 5f65 7272 6f72 5f6e 6f74 5f66 6f75 6e64  _error_not_found
+00000ab0: da19 6469 616c 6f67 5f66 696c 655f 7265  ..dialog_file_re
+00000ac0: 7374 6f72 655f 7469 746c 65da 1864 6961  store_title..dia
+00000ad0: 6c6f 675f 6669 6c65 5f72 6573 746f 7265  log_file_restore
+00000ae0: 5f74 6578 74da 1964 6961 6c6f 675f 6669  _text..dialog_fi
+00000af0: 6c65 5f72 6573 746f 7265 5f65 7272 6f72  le_restore_error
+00000b00: da22 6469 616c 6f67 5f66 696c 655f 7265  ."dialog_file_re
+00000b10: 7374 6f72 655f 7761 726e 696e 675f 6578  store_warning_ex
+00000b20: 6973 7473 da18 6469 616c 6f67 5f6d 6573  ists..dialog_mes
+00000b30: 7361 6765 5f62 6f78 5f74 6974 6c65 da1c  sage_box_title..
+00000b40: 6469 616c 6f67 5f6d 6573 7361 6765 5f62  dialog_message_b
+00000b50: 6f78 5f62 7574 746f 6e5f 6f6b da28 6163  ox_button_ok.(ac
+00000b60: 7469 6f6e 5f6e 6577 5f66 696c 655f 6669  tion_new_file_fi
+00000b70: 7273 745f 6c69 6e65 5f74 656d 706c 6174  rst_line_templat
+00000b80: 655f 7465 7874 da1f 6163 7469 6f6e 5f6f  e_text..action_o
+00000b90: 7065 6e5f 6669 6c65 5f64 6961 6c6f 675f  pen_file_dialog_
+00000ba0: 6361 7074 696f 6eda 2261 6374 696f 6e5f  caption."action_
+00000bb0: 7361 7665 5f61 735f 6669 6c65 5f64 6961  save_as_file_dia
+00000bc0: 6c6f 675f 6361 7074 696f 6eda 1c64 6961  log_caption..dia
+00000bd0: 6c6f 675f 7361 7665 5f65 6d70 7479 5f66  log_save_empty_f
+00000be0: 696c 655f 7469 746c 65da 1b64 6961 6c6f  ile_title..dialo
+00000bf0: 675f 7361 7665 5f65 6d70 7479 5f66 696c  g_save_empty_fil
+00000c00: 655f 7465 7874 da19 6469 616c 6f67 5f65  e_text..dialog_e
+00000c10: 6e63 7279 7074 5f66 696c 655f 7469 746c  ncrypt_file_titl
+00000c20: 65da 1864 6961 6c6f 675f 656e 6372 7970  e..dialog_encryp
+00000c30: 745f 6669 6c65 5f74 6578 74da 2e65 6e63  t_file_text..enc
+00000c40: 7279 7074 5f66 696c 655f 7761 726e 696e  rypt_file_warnin
+00000c50: 675f 6669 6c65 5f69 735f 616c 7265 6164  g_file_is_alread
+00000c60: 795f 656e 6372 7970 7465 64da 2a64 6961  y_encrypted.*dia
+00000c70: 6c6f 675f 656e 6372 7970 745f 6669 6c65  log_encrypt_file
+00000c80: 5f72 6577 7269 7465 5f65 7869 7374 696e  _rewrite_existin
+00000c90: 675f 7469 746c 65da 2964 6961 6c6f 675f  g_title.)dialog_
+00000ca0: 656e 6372 7970 745f 6669 6c65 5f72 6577  encrypt_file_rew
+00000cb0: 7269 7465 5f65 7869 7374 696e 675f 7465  rite_existing_te
+00000cc0: 7874 da19 6469 616c 6f67 5f64 6563 7279  xt..dialog_decry
+00000cd0: 7074 5f66 696c 655f 7469 746c 65da 1864  pt_file_title..d
+00000ce0: 6961 6c6f 675f 6465 6372 7970 745f 6669  ialog_decrypt_fi
+00000cf0: 6c65 5f74 6578 74da 2a64 6563 7279 7074  le_text.*decrypt
+00000d00: 5f66 696c 655f 7761 726e 696e 675f 6669  _file_warning_fi
+00000d10: 6c65 5f69 735f 6e6f 745f 656e 6372 7970  le_is_not_encryp
+00000d20: 7465 64da 2a64 6961 6c6f 675f 6465 6372  ted.*dialog_decr
+00000d30: 7970 745f 6669 6c65 5f72 6577 7269 7465  ypt_file_rewrite
+00000d40: 5f65 7869 7374 696e 675f 7469 746c 65da  _existing_title.
+00000d50: 2964 6961 6c6f 675f 6465 6372 7970 745f  )dialog_decrypt_
+00000d60: 6669 6c65 5f72 6577 7269 7465 5f65 7869  file_rewrite_exi
+00000d70: 7374 696e 675f 7465 7874 da21 6469 616c  sting_text.!dial
+00000d80: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
+00000d90: 6173 7377 6f72 645f 7469 746c 65da 2164  assword_title.!d
+00000da0: 6961 6c6f 675f 656e 6372 7970 745f 6e65  ialog_encrypt_ne
+00000db0: 775f 7061 7373 776f 7264 5f6c 6162 656c  w_password_label
+00000dc0: da32 6469 616c 6f67 5f65 6e63 7279 7074  .2dialog_encrypt
+00000dd0: 5f6e 6577 5f70 6173 7377 6f72 645f 696e  _new_password_in
+00000de0: 7075 745f 706c 6163 6568 6f6c 6465 725f  put_placeholder_
+00000df0: 7465 7874 da26 6469 616c 6f67 5f65 6e63  text.&dialog_enc
+00000e00: 7279 7074 5f6e 6577 5f70 6173 7377 6f72  rypt_new_passwor
+00000e10: 645f 6869 6e74 5f6c 6162 656c da32 6469  d_hint_label.2di
+00000e20: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+00000e30: 5f70 6173 7377 6f72 645f 6869 6e74 5f6c  _password_hint_l
+00000e40: 6162 656c 5f64 6573 6372 6970 7469 6f6e  abel_description
+00000e50: da37 6469 616c 6f67 5f65 6e63 7279 7074  .7dialog_encrypt
+00000e60: 5f6e 6577 5f70 6173 7377 6f72 645f 6869  _new_password_hi
+00000e70: 6e74 5f69 6e70 7574 5f70 6c61 6365 686f  nt_input_placeho
+00000e80: 6c64 6572 5f74 6578 74da 2564 6961 6c6f  lder_text.%dialo
+00000e90: 675f 656e 6372 7970 745f 6e65 775f 7061  g_encrypt_new_pa
+00000ea0: 7373 776f 7264 5f62 7574 746f 6e5f 6f6b  ssword_button_ok
+00000eb0: da29 6469 616c 6f67 5f65 6e63 7279 7074  .)dialog_encrypt
+00000ec0: 5f6e 6577 5f70 6173 7377 6f72 645f 6275  _new_password_bu
+00000ed0: 7474 6f6e 5f63 616e 6365 6cda 2f64 6961  tton_cancel./dia
+00000ee0: 6c6f 675f 656e 6372 7970 745f 6e65 775f  log_encrypt_new_
+00000ef0: 7061 7373 776f 7264 5f77 6172 6e69 6e67  password_warning
+00000f00: 5f65 6d70 7479 5f74 6974 6c65 da2e 6469  _empty_title..di
+00000f10: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+00000f20: 5f70 6173 7377 6f72 645f 7761 726e 696e  _password_warnin
+00000f30: 675f 656d 7074 795f 7465 7874 da32 6469  g_empty_text.2di
+00000f40: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+00000f50: 5f70 6173 7377 6f72 645f 7761 726e 696e  _password_warnin
+00000f60: 675f 746f 6f5f 6c6f 6e67 5f74 6974 6c65  g_too_long_title
+00000f70: da31 6469 616c 6f67 5f65 6e63 7279 7074  .1dialog_encrypt
+00000f80: 5f6e 6577 5f70 6173 7377 6f72 645f 7761  _new_password_wa
+00000f90: 726e 696e 675f 746f 6f5f 6c6f 6e67 5f74  rning_too_long_t
+00000fa0: 6578 74da 1d64 6961 6c6f 675f 656e 6372  ext..dialog_encr
+00000fb0: 7970 745f 7061 7373 776f 7264 5f74 6974  ypt_password_tit
+00000fc0: 6c65 da1d 6469 616c 6f67 5f65 6e63 7279  le..dialog_encry
+00000fd0: 7074 5f70 6173 7377 6f72 645f 6c61 6265  pt_password_labe
+00000fe0: 6cda 2e64 6961 6c6f 675f 656e 6372 7970  l..dialog_encryp
+00000ff0: 745f 7061 7373 776f 7264 5f69 6e70 7574  t_password_input
+00001000: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
+00001010: 74da 2264 6961 6c6f 675f 656e 6372 7970  t."dialog_encryp
+00001020: 745f 7061 7373 776f 7264 5f68 696e 745f  t_password_hint_
+00001030: 6c61 6265 6cda 2164 6961 6c6f 675f 656e  label.!dialog_en
+00001040: 6372 7970 745f 7061 7373 776f 7264 5f62  crypt_password_b
+00001050: 7574 746f 6e5f 6f6b da25 6469 616c 6f67  utton_ok.%dialog
+00001060: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
+00001070: 645f 6275 7474 6f6e 5f63 616e 6365 6cda  d_button_cancel.
+00001080: 2364 6961 6c6f 675f 656e 6372 7970 745f  #dialog_encrypt_
+00001090: 7061 7373 776f 7264 5f72 6573 6574 5f74  password_reset_t
+000010a0: 6974 6c65 da22 6469 616c 6f67 5f65 6e63  itle."dialog_enc
+000010b0: 7279 7074 5f70 6173 7377 6f72 645f 7265  rypt_password_re
+000010c0: 7365 745f 7465 7874 da2b 6469 616c 6f67  set_text.+dialog
+000010d0: 5f65 6e63 7279 7074 5f70 6173 7377 6f72  _encrypt_passwor
+000010e0: 645f 7265 7365 745f 6275 7474 6f6e 5f63  d_reset_button_c
+000010f0: 616e 6365 6cda 2864 6961 6c6f 675f 656e  ancel.(dialog_en
+00001100: 6372 7970 745f 7061 7373 776f 7264 5f72  crypt_password_r
+00001110: 6573 6574 5f62 7574 746f 6e5f 7965 73da  eset_button_yes.
+00001120: 1664 6961 6c6f 675f 6f70 656e 5f6c 696e  .dialog_open_lin
+00001130: 6b5f 7469 746c 65da 1564 6961 6c6f 675f  k_title..dialog_
+00001140: 6f70 656e 5f6c 696e 6b5f 7465 7874 da26  open_link_text.&
+00001150: 6c6f 6164 5f66 696c 655f 656e 6372 7970  load_file_encryp
+00001160: 7469 6f6e 5f70 6173 7377 6f72 645f 6d69  tion_password_mi
+00001170: 736d 6174 6368 da27 6c6f 6164 5f66 696c  smatch.'load_fil
+00001180: 655f 656e 6372 7970 7469 6f6e 5f70 6173  e_encryption_pas
+00001190: 7377 6f72 645f 696e 636f 7272 6563 74da  sword_incorrect.
+000011a0: 1c6c 6f61 645f 6669 6c65 5f6e 6f6e 655f  .load_file_none_
+000011b0: 636f 6e74 656e 745f 6572 726f 72da 1f73  content_error..s
+000011c0: 6176 655f 6163 7469 7665 5f66 696c 655f  ave_active_file_
+000011d0: 6572 726f 725f 6f63 6375 7272 6564 da1e  error_occurred..
+000011e0: 6578 7061 6e64 6162 6c65 5f62 6c6f 636b  expandable_block
+000011f0: 5f64 6566 6175 6c74 5f74 6974 6c65 da31  _default_title.1
+00001200: 6469 616c 6f67 5f63 6f6c 6f72 5f70 6963  dialog_color_pic
+00001210: 6b65 725f 636f 6c6f 725f 636f 7069 6564  ker_color_copied
+00001220: 5f74 6f5f 7468 655f 636c 6970 626f 6172  _to_the_clipboar
+00001230: 64da 1170 6f70 7570 5f61 626f 7574 5f74  d..popup_about_t
+00001240: 6974 6c65 da20 706f 7075 705f 6162 6f75  itle. popup_abou
+00001250: 745f 6170 705f 6e61 6d65 5f64 6573 6372  t_app_name_descr
+00001260: 6970 7469 6f6e da13 706f 7075 705f 6162  iption..popup_ab
+00001270: 6f75 745f 7665 7273 696f 6eda 1370 6f70  out_version..pop
+00001280: 7570 5f61 626f 7574 5f6c 6963 656e 7365  up_about_license
+00001290: da13 706f 7075 705f 6162 6f75 745f 7765  ..popup_about_we
+000012a0: 6273 6974 65da 1670 6f70 7570 5f61 626f  bsite..popup_abo
+000012b0: 7574 5f72 6570 6f73 6974 6f72 79da 1070  ut_repository..p
+000012c0: 6f70 7570 5f61 626f 7574 5f70 7970 69da  opup_about_pypi.
+000012d0: 1070 6f70 7570 5f61 626f 7574 5f64 6174  .popup_about_dat
+000012e0: 65da 2675 7064 6174 655f 6865 6c70 6572  e.&update_helper
+000012f0: 5f6e 6577 5f76 6572 7369 6f6e 5f69 735f  _new_version_is_
+00001300: 6176 6169 6c61 626c 65da 2675 7064 6174  available.&updat
+00001310: 655f 6865 6c70 6572 5f6c 6174 6573 745f  e_helper_latest_
+00001320: 7665 7273 696f 6e5f 696e 7374 616c 6c65  version_installe
+00001330: 64da 1e6e 6574 776f 726b 5f63 6f6e 6e65  d..network_conne
+00001340: 6374 696f 6e5f 6572 726f 725f 656d 7074  ction_error_empt
+00001350: 79da 2a6e 6574 776f 726b 5f63 6f6e 6e65  y.*network_conne
+00001360: 6374 696f 6e5f 6572 726f 725f 636f 6e6e  ction_error_conn
+00001370: 6563 7469 6f6e 5f6f 725f 646e 73da 2b6e  ection_or_dns.+n
+00001380: 6574 776f 726b 5f63 6f6e 6e65 6374 696f  etwork_connectio
+00001390: 6e5f 6572 726f 725f 636f 6e6e 6563 7469  n_error_connecti
+000013a0: 6f6e 5f72 6566 7573 6564 da2d 6e65 7477  on_refused.-netw
+000013b0: 6f72 6b5f 636f 6e6e 6563 7469 6f6e 5f65  ork_connection_e
+000013c0: 7272 6f72 5f63 6f6e 6e65 6374 696f 6e5f  rror_connection_
+000013d0: 7469 6d65 645f 6f75 74da 2d6e 6574 776f  timed_out.-netwo
+000013e0: 726b 5f63 6f6e 6e65 6374 696f 6e5f 6572  rk_connection_er
+000013f0: 726f 725f 636f 6e6e 6563 7469 6f6e 5f34  ror_connection_4
+00001400: 3034 5f65 7272 6f72 da31 6e65 7477 6f72  04_error.1networ
+00001410: 6b5f 636f 6e6e 6563 7469 6f6e 5f65 7272  k_connection_err
+00001420: 6f72 5f67 656e 6572 6963 5f77 6974 685f  or_generic_with_
+00001430: 7374 6174 7573 5f63 6f64 654e 2901 da07  status_codeN)...
+00001440: 6c65 7865 6d65 73a9 0072 6100 0000 7261  lexemes..ra...ra
+00001450: 0000 00fa 432f 5573 6572 732f 7661 6469  ....C/Users/vadi
+00001460: 6b75 732f 5079 6368 6172 6d50 726f 6a65  kus/PycharmProje
+00001470: 6374 732f 6e6f 746f 6c6f 672d 6465 762f  cts/notolog-dev/
+00001480: 6170 702f 6c65 7865 6d65 732f 656e 2f63  app/lexemes/en/c
+00001490: 6f6d 6d6f 6e2e 7079 da08 3c6d 6f64 756c  ommon.py..<modul
+000014a0: 653e 0300 0000 73a8 0000 0002 0102 0202  e>....s.........
+000014b0: 0202 0102 0102 0102 0202 0102 0102 0102  ................
+000014c0: 0202 0102 0102 0102 0102 0102 0202 0102  ................
+000014d0: 0102 0102 0202 0102 0202 0102 0102 0202  ................
+000014e0: 0102 0202 0102 0102 0102 0102 0202 0102  ................
+000014f0: 0102 0102 0102 0202 0102 0102 0102 0102  ................
+00001500: 0402 0102 0102 0102 0102 0102 0102 0202  ................
+00001510: 0102 0102 0102 0102 0102 0202 0102 0102  ................
+00001520: 0102 0202 0102 0202 0102 0102 0202 0202  ................
+00001530: 0202 0202 0102 0202 0102 0102 0102 0102  ................
+00001540: 0102 0202 0102 0202 0202 0202 0102 0202  ................
+00001550: 0102 90                                  ...
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/main_menu.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 2181 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 8508 0000  a.......(..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 8508 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
 00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640c 6401 640d 640e  d.d.d.d.d.d.d.d.
 00000050: 640f 6410 6411 6412 6413 6414 6415 6416  d.d.d.d.d.d.d.d.
 00000060: 6417 6418 6419 641a 641b 641c 641d 641e  d.d.d.d.d.d.d.d.
 00000070: 641e 641f 641f 6420 6421 6422 6422 6423  d.d.d.d d!d"d"d#
-00000080: 9c28 5a00 6424 5300 2925 da04 4669 6c65  .(Z.d$S.)%..File
+00000080: 9c28 5a00 6424 5300 2925 5a04 4669 6c65  .(Z.d$S.)%Z.File
 00000090: 5a04 4564 6974 5a05 546f 6f6c 73da 0448  Z.EditZ.Tools..H
 000000a0: 656c 707a 0c4e 6577 2064 6f63 756d 656e  elpz.New documen
 000000b0: 74da 044f 7065 6e7a 0d4f 7065 6e20 646f  t..Openz.Open do
 000000c0: 6375 6d65 6e74 da04 5361 7665 7a0d 5361  cument..Savez.Sa
 000000d0: 7665 2064 6f63 756d 656e 747a 0753 6176  ve documentz.Sav
 000000e0: 6520 6173 7a15 5361 7665 2061 7320 646f  e asz.Save as do
-000000f0: 6375 6d65 6e74 2063 6f70 79da 0445 7869  cument copy..Exi
+000000f0: 6375 6d65 6e74 2063 6f70 795a 0445 7869  cument copyZ.Exi
 00000100: 747a 0c45 7869 7420 7468 6520 6170 707a  tz.Exit the appz
 00000110: 0945 6469 7420 4669 6c65 da06 536f 7572  .Edit File..Sour
 00000120: 6365 7a0b 536f 7572 6365 2043 6f64 65da  cez.Source Code.
 00000130: 0442 6f6c 647a 1042 6f6c 6420 5465 7874  .Boldz.Bold Text
 00000140: 2046 6f72 6d61 74da 0649 7461 6c69 637a   Format..Italicz
 00000150: 1249 7461 6c69 6320 5465 7874 2046 6f72  .Italic Text For
 00000160: 6d61 74da 0955 6e64 6572 6c69 6e65 7a15  mat..Underlinez.
@@ -93,17 +93,17 @@
 000005c0: 5f61 7373 6973 7461 6e74 da2a 746f 6f6c  _assistant.*tool
 000005d0: 735f 6163 7469 6f6e 735f 6163 6365 7373  s_actions_access
 000005e0: 6962 6c65 5f6e 616d 655f 6169 5f61 7373  ible_name_ai_ass
 000005f0: 6973 7461 6e74 da1a 746f 6f6c 735f 6163  istant..tools_ac
 00000600: 7469 6f6e 735f 636f 6c6f 725f 7069 636b  tions_color_pick
 00000610: 6572 da2a 746f 6f6c 735f 6163 7469 6f6e  er.*tools_action
 00000620: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
-00000630: 655f 636f 6c6f 725f 7069 636b 6572 5a1c  e_color_pickerZ.
+00000630: 655f 636f 6c6f 725f 7069 636b 6572 da1c  e_color_picker..
 00000640: 6163 7469 6f6e 735f 6865 6c70 5f6c 6162  actions_help_lab
-00000650: 656c 5f6d 645f 7379 6e74 6178 5a26 6163  el_md_syntaxZ&ac
+00000650: 656c 5f6d 645f 7379 6e74 6178 da26 6163  el_md_syntax.&ac
 00000660: 7469 6f6e 735f 6865 6c70 5f61 6363 6573  tions_help_acces
 00000670: 7369 626c 655f 6e61 6d65 5f6d 645f 7379  sible_name_md_sy
 00000680: 6e74 6178 da24 6163 7469 6f6e 735f 6865  ntax.$actions_he
 00000690: 6c70 5f6c 6162 656c 5f63 6865 636b 5f66  lp_label_check_f
 000006a0: 6f72 5f75 7064 6174 6573 da2e 6163 7469  or_updates..acti
 000006b0: 6f6e 735f 6865 6c70 5f61 6363 6573 7369  ons_help_accessi
 000006c0: 626c 655f 6e61 6d65 5f63 6865 636b 5f66  ble_name_check_f
@@ -116,15 +116,15 @@
 00000730: 5f6c 6162 656c 5f61 626f 7574 da22 6163  _label_about."ac
 00000740: 7469 6f6e 735f 6865 6c70 5f61 6363 6573  tions_help_acces
 00000750: 7369 626c 655f 6e61 6d65 5f61 626f 7574  sible_name_about
 00000760: 4e29 01da 076c 6578 656d 6573 a900 7231  N)...lexemes..r1
 00000770: 0000 0072 3100 0000 fa46 2f55 7365 7273  ...r1....F/Users
 00000780: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
 00000790: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-000007a0: 2f6e 6f74 6f6c 6f67 2f6c 6578 656d 6573  /notolog/lexemes
+000007a0: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
 000007b0: 2f65 6e2f 6d61 696e 5f6d 656e 752e 7079  /en/main_menu.py
 000007c0: da08 3c6d 6f64 756c 653e 0300 0000 7350  ..<module>....sP
 000007d0: 0000 0002 0102 0102 0102 0202 0102 0102  ................
 000007e0: 0102 0102 0102 0102 0102 0102 0102 0202  ................
 000007f0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000800: 0102 0102 0102 0102 0102 0202 0102 0102  ................
 00000810: 0102 0202 0102 0102 0102 0102 0102 0102  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/settings_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 3351 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,217 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 170d 0000  a.......(..f....
+00000000: 610d 0d0a 0000 0000 42a9 3566 020e 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 002e 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
-00000080: 6429 642a 642b 642c 642d 9c2d 5a00 642e  d)d*d+d,d-.-Z.d.
-00000090: 5300 292f da08 5365 7474 696e 6773 da05  S.)/..Settings..
-000000a0: 436c 6f73 655a 0747 656e 6572 616c 5a06  CloseZ.GeneralZ.
-000000b0: 4564 6974 6f72 5a06 5669 6577 6572 7a09  EditorZ.Viewerz.
-000000c0: 4149 2043 6f6e 6669 677a 0a41 7070 2063  AI Configz.App c
-000000d0: 6f6e 6669 67da 084c 616e 6775 6167 657a  onfig..Languagez
-000000e0: 1143 686f 6f73 6520 6120 6c61 6e67 7561  .Choose a langua
-000000f0: 6765 7a18 4170 7027 7320 696e 7465 7266  gez.App's interf
-00000100: 6163 6520 6c61 6e67 7561 6765 da05 5468  ace language..Th
-00000110: 656d 657a 0e43 686f 6f73 6520 6120 7468  emez.Choose a th
-00000120: 656d 657a 1541 7070 2773 2069 6e74 6572  emez.App's inter
-00000130: 6661 6365 2074 6865 6d65 7a09 4d61 696e  face themez.Main
-00000140: 204d 656e 757a 0e53 686f 7720 4d61 696e   Menuz.Show Main
-00000150: 204d 656e 757a 2444 6973 706c 6179 2074   Menuz$Display t
-00000160: 6865 2061 7070 2773 206d 6169 6e20 6472  he app's main dr
-00000170: 6f70 646f 776e 206d 656e 757a 1346 6f6e  opdown menuz.Fon
-00000180: 7420 5369 7a65 3a20 7b73 697a 657d 7074  t Size: {size}pt
-00000190: 7a21 4164 6a75 7374 2074 6865 2061 7070  z!Adjust the app
-000001a0: 2773 2067 6c6f 6261 6c20 666f 6e74 2073  's global font s
-000001b0: 697a 657a 0a53 7461 7475 7320 4261 727a  izez.Status Barz
-000001c0: 1b53 686f 7720 476c 6f62 616c 2043 7572  .Show Global Cur
-000001d0: 736f 7220 506f 7369 7469 6f6e 7a34 4469  sor Positionz4Di
-000001e0: 7370 6c61 7920 7468 6520 676c 6f62 616c  splay the global
-000001f0: 2063 7572 736f 7220 706f 7369 7469 6f6e   cursor position
-00000200: 2069 6e20 7468 6520 7374 6174 7573 2062   in the status b
-00000210: 6172 7a14 4564 6974 6f72 2043 6f6e 6669  arz.Editor Confi
-00000220: 6775 7261 7469 6f6e 7a11 5368 6f77 204c  gurationz.Show L
-00000230: 696e 6520 4e75 6d62 6572 737a 2244 6973  ine Numbersz"Dis
-00000240: 706c 6179 206c 696e 6520 6e75 6d62 6572  play line number
-00000250: 7320 696e 2074 6865 2065 6469 746f 727a  s in the editorz
-00000260: 1456 6965 7765 7220 436f 6e66 6967 7572  .Viewer Configur
-00000270: 6174 696f 6e7a 1f43 6f6e 7665 7274 2054  ationz.Convert T
-00000280: 6578 7420 456d 6f6a 6973 2074 6f20 4772  ext Emojis to Gr
-00000290: 6170 6869 6373 7a30 436f 6e76 6572 7420  aphicsz0Convert 
-000002a0: 7465 7874 2065 6d6f 6a69 7320 746f 2067  text emojis to g
-000002b0: 7261 7068 6963 616c 2072 6570 7265 7365  raphical represe
-000002c0: 6e74 6174 696f 6e73 7a0f 4869 6768 6c69  ntationsz.Highli
-000002d0: 6768 7420 544f 444f 737a 2345 6d70 6861  ght TODOsz#Empha
-000002e0: 7369 7a65 2054 4f44 4f20 7461 6773 2077  size TODO tags w
-000002f0: 6974 6869 6e20 7468 6520 7465 7874 7a22  ithin the textz"
-00000300: 5265 7175 6972 6520 436f 6e66 6972 6d61  Require Confirma
-00000310: 7469 6f6e 2074 6f20 4f70 656e 204c 696e  tion to Open Lin
-00000320: 6b73 7a29 4173 6b20 666f 7220 636f 6e66  ksz)Ask for conf
-00000330: 6972 6d61 7469 6f6e 2062 6566 6f72 6520  irmation before 
-00000340: 6f70 656e 696e 6720 6c69 6e6b 737a 0a4f  opening linksz.O
-00000350: 7065 6e41 4920 4150 497a 0741 5049 2055  penAI APIz.API U
-00000360: 524c 7a0e 4f70 656e 4149 2041 5049 2055  RLz.OpenAI API U
-00000370: 524c 7a07 4150 4920 6b65 797a 0e4f 7065  RLz.API keyz.Ope
-00000380: 6e41 4920 4150 4920 6b65 797a 1053 7570  nAI API keyz.Sup
-00000390: 706f 7274 6564 206d 6f64 656c 737a 0c43  ported modelsz.C
-000003a0: 686f 6f73 6520 6d6f 6465 6c7a 1a53 7570  hoose modelz.Sup
-000003b0: 706f 7274 6564 206d 6f64 656c 7320 746f  ported models to
-000003c0: 2063 686f 6f73 657a 0f42 6173 6520 5061   choosez.Base Pa
-000003d0: 7261 6d65 7465 7273 7a0d 5379 7374 656d  rametersz.System
-000003e0: 2050 726f 6d70 747a 2d42 6173 6520 7379   Promptz-Base sy
-000003f0: 7374 656d 2070 726f 6d70 7420 7468 6174  stem prompt that
-00000400: 2070 7265 6365 6465 7320 6561 6368 2072   precedes each r
-00000410: 6571 7565 7374 7a42 4261 7365 2073 7973  equestzBBase sys
-00000420: 7465 6d20 7072 6f6d 7074 2074 6861 7420  tem prompt that 
-00000430: 7072 6563 6564 6573 2065 6163 6820 7265  precedes each re
-00000440: 7175 6573 742e 2054 6869 7320 6973 2070  quest. This is p
-00000450: 6c61 696e 2074 6578 742e 7a17 4d61 7869  lain text.z.Maxi
-00000460: 6d75 6d20 5265 7370 6f6e 7365 2054 6f6b  mum Response Tok
-00000470: 656e 737a 2f4d 6178 696d 756d 206e 756d  ensz/Maximum num
-00000480: 6265 7220 6f66 2074 6f6b 656e 7320 746f  ber of tokens to
-00000490: 2072 6563 6569 7665 2069 6e20 7265 7370   receive in resp
-000004a0: 6f6e 7365 292d da0c 7769 6e64 6f77 5f74  onse)-..window_t
-000004b0: 6974 6c65 da0c 6275 7474 6f6e 5f63 6c6f  itle..button_clo
-000004c0: 7365 da0b 7461 625f 6765 6e65 7261 6cda  se..tab_general.
-000004d0: 1174 6162 5f65 6469 746f 725f 636f 6e66  .tab_editor_conf
-000004e0: 6967 da11 7461 625f 7669 6577 6572 5f63  ig..tab_viewer_c
-000004f0: 6f6e 6669 67da 0d74 6162 5f61 695f 636f  onfig..tab_ai_co
-00000500: 6e66 6967 da18 6765 6e65 7261 6c5f 6170  nfig..general_ap
-00000510: 705f 636f 6e66 6967 5f6c 6162 656c da1a  p_config_label..
-00000520: 6765 6e65 7261 6c5f 6170 705f 6c61 6e67  general_app_lang
-00000530: 7561 6765 5f6c 6162 656c da2b 6765 6e65  uage_label.+gene
-00000540: 7261 6c5f 6170 705f 6c61 6e67 7561 6765  ral_app_language
-00000550: 5f63 6f6d 626f 5f70 6c61 6365 686f 6c64  _combo_placehold
-00000560: 6572 5f74 6578 745a 3167 656e 6572 616c  er_textZ1general
-00000570: 5f61 7070 5f6c 616e 6775 6167 655f 636f  _app_language_co
-00000580: 6d62 6f5f 6163 6365 7373 6962 6c65 5f64  mbo_accessible_d
-00000590: 6573 6372 6970 7469 6f6e da17 6765 6e65  escription..gene
-000005a0: 7261 6c5f 6170 705f 7468 656d 655f 6c61  ral_app_theme_la
-000005b0: 6265 6cda 2867 656e 6572 616c 5f61 7070  bel.(general_app
-000005c0: 5f74 6865 6d65 5f63 6f6d 626f 5f70 6c61  _theme_combo_pla
-000005d0: 6365 686f 6c64 6572 5f74 6578 74da 2e67  ceholder_text..g
-000005e0: 656e 6572 616c 5f61 7070 5f74 6865 6d65  eneral_app_theme
-000005f0: 5f63 6f6d 626f 5f61 6363 6573 7369 626c  _combo_accessibl
-00000600: 655f 6465 7363 7269 7074 696f 6eda 1b67  e_description..g
-00000610: 656e 6572 616c 5f61 7070 5f6d 6169 6e5f  eneral_app_main_
-00000620: 6d65 6e75 5f6c 6162 656c da1e 6765 6e65  menu_label..gene
-00000630: 7261 6c5f 6170 705f 6d61 696e 5f6d 656e  ral_app_main_men
-00000640: 755f 6368 6563 6b62 6f78 da35 6765 6e65  u_checkbox.5gene
-00000650: 7261 6c5f 6170 705f 6d61 696e 5f6d 656e  ral_app_main_men
-00000660: 755f 6368 6563 6b62 6f78 5f61 6363 6573  u_checkbox_acces
-00000670: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000680: 6eda 1b67 656e 6572 616c 5f61 7070 5f66  n..general_app_f
-00000690: 6f6e 745f 7369 7a65 5f6c 6162 656c da33  ont_size_label.3
-000006a0: 6765 6e65 7261 6c5f 6170 705f 666f 6e74  general_app_font
-000006b0: 5f73 697a 655f 736c 6964 6572 5f61 6363  _size_slider_acc
-000006c0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
-000006d0: 696f 6eda 1767 656e 6572 616c 5f73 7461  ion..general_sta
-000006e0: 7475 7362 6172 5f6c 6162 656c da36 6765  tusbar_label.6ge
-000006f0: 6e65 7261 6c5f 7374 6174 7573 6261 725f  neral_statusbar_
-00000700: 7368 6f77 5f67 6c6f 6261 6c5f 6375 7273  show_global_curs
-00000710: 6f72 5f70 6f73 6974 696f 6e5f 6368 6563  or_position_chec
-00000720: 6b62 6f78 da4d 6765 6e65 7261 6c5f 7374  kbox.Mgeneral_st
-00000730: 6174 7573 6261 725f 7368 6f77 5f67 6c6f  atusbar_show_glo
-00000740: 6261 6c5f 6375 7273 6f72 5f70 6f73 6974  bal_cursor_posit
-00000750: 696f 6e5f 6368 6563 6b62 6f78 5f61 6363  ion_checkbox_acc
-00000760: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
-00000770: 696f 6eda 1365 6469 746f 725f 636f 6e66  ion..editor_conf
-00000780: 6967 5f6c 6162 656c da28 6564 6974 6f72  ig_label.(editor
-00000790: 5f63 6f6e 6669 675f 7368 6f77 5f6c 696e  _config_show_lin
-000007a0: 655f 6e75 6d62 6572 735f 6368 6563 6b62  e_numbers_checkb
-000007b0: 6f78 da3f 6564 6974 6f72 5f63 6f6e 6669  ox.?editor_confi
-000007c0: 675f 7368 6f77 5f6c 696e 655f 6e75 6d62  g_show_line_numb
-000007d0: 6572 735f 6368 6563 6b62 6f78 5f61 6363  ers_checkbox_acc
-000007e0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
-000007f0: 696f 6eda 1376 6965 7765 725f 636f 6e66  ion..viewer_conf
-00000800: 6967 5f6c 6162 656c da25 7669 6577 6572  ig_label.%viewer
-00000810: 5f63 6f6e 6669 675f 7072 6f63 6573 735f  _config_process_
-00000820: 656d 6f6a 6973 5f63 6865 636b 626f 78da  emojis_checkbox.
-00000830: 3c76 6965 7765 725f 636f 6e66 6967 5f70  <viewer_config_p
-00000840: 726f 6365 7373 5f65 6d6f 6a69 735f 6368  rocess_emojis_ch
-00000850: 6563 6b62 6f78 5f61 6363 6573 7369 626c  eckbox_accessibl
-00000860: 655f 6465 7363 7269 7074 696f 6eda 2676  e_description.&v
-00000870: 6965 7765 725f 636f 6e66 6967 5f68 6967  iewer_config_hig
-00000880: 686c 6967 6874 5f74 6f64 6f73 5f63 6865  hlight_todos_che
-00000890: 636b 626f 78da 3d76 6965 7765 725f 636f  ckbox.=viewer_co
-000008a0: 6e66 6967 5f68 6967 686c 6967 6874 5f74  nfig_highlight_t
-000008b0: 6f64 6f73 5f63 6865 636b 626f 785f 6163  odos_checkbox_ac
-000008c0: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
-000008d0: 7469 6f6e da2d 7669 6577 6572 5f63 6f6e  tion.-viewer_con
-000008e0: 6669 675f 6f70 656e 5f6c 696e 6b5f 636f  fig_open_link_co
-000008f0: 6e66 6972 6d61 7469 6f6e 5f63 6865 636b  nfirmation_check
-00000900: 626f 78da 4476 6965 7765 725f 636f 6e66  box.Dviewer_conf
-00000910: 6967 5f6f 7065 6e5f 6c69 6e6b 5f63 6f6e  ig_open_link_con
-00000920: 6669 726d 6174 696f 6e5f 6368 6563 6b62  firmation_checkb
-00000930: 6f78 5f61 6363 6573 7369 626c 655f 6465  ox_accessible_de
-00000940: 7363 7269 7074 696f 6eda 1a61 695f 636f  scription..ai_co
-00000950: 6e66 6967 5f6f 7065 6e61 695f 6170 695f  nfig_openai_api_
-00000960: 6c61 6265 6cda 2f61 695f 636f 6e66 6967  label./ai_config
-00000970: 5f6f 7065 6e61 695f 6170 695f 7572 6c5f  _openai_api_url_
-00000980: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
-00000990: 725f 7465 7874 da35 6169 5f63 6f6e 6669  r_text.5ai_confi
-000009a0: 675f 6f70 656e 6169 5f61 7069 5f75 726c  g_openai_api_url
-000009b0: 5f69 6e70 7574 5f61 6363 6573 7369 626c  _input_accessibl
-000009c0: 655f 6465 7363 7269 7074 696f 6eda 2f61  e_description./a
-000009d0: 695f 636f 6e66 6967 5f6f 7065 6e61 695f  i_config_openai_
-000009e0: 6170 695f 6b65 795f 696e 7075 745f 706c  api_key_input_pl
-000009f0: 6163 6568 6f6c 6465 725f 7465 7874 da35  aceholder_text.5
-00000a00: 6169 5f63 6f6e 6669 675f 6f70 656e 6169  ai_config_openai
-00000a10: 5f61 7069 5f6b 6579 5f69 6e70 7574 5f61  _api_key_input_a
-00000a20: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
-00000a30: 7074 696f 6eda 2b61 695f 636f 6e66 6967  ption.+ai_config
-00000a40: 5f6f 7065 6e61 695f 6170 695f 7375 7070  _openai_api_supp
-00000a50: 6f72 7465 645f 6d6f 6465 6c73 5f6c 6162  orted_models_lab
-00000a60: 656c da2f 6169 5f63 6f6e 6669 675f 6169  el./ai_config_ai
-00000a70: 5f6d 6f64 656c 5f6e 616d 6573 5f63 6f6d  _model_names_com
-00000a80: 626f 5f70 6c61 6365 686f 6c64 6572 5f74  bo_placeholder_t
-00000a90: 6578 74da 3561 695f 636f 6e66 6967 5f61  ext.5ai_config_a
-00000aa0: 695f 6d6f 6465 6c5f 6e61 6d65 735f 636f  i_model_names_co
-00000ab0: 6d62 6f5f 6163 6365 7373 6962 6c65 5f64  mbo_accessible_d
-00000ac0: 6573 6372 6970 7469 6f6e da14 6169 5f63  escription..ai_c
-00000ad0: 6f6e 6669 675f 6261 7365 5f6c 6162 656c  onfig_base_label
-00000ae0: da22 6169 5f63 6f6e 6669 675f 6261 7365  ."ai_config_base
-00000af0: 5f73 7973 7465 6d5f 7072 6f6d 7074 5f6c  _system_prompt_l
-00000b00: 6162 656c da32 6169 5f63 6f6e 6669 675f  abel.2ai_config_
-00000b10: 6261 7365 5f73 7973 7465 6d5f 7072 6f6d  base_system_prom
-00000b20: 7074 5f65 6469 745f 706c 6163 6568 6f6c  pt_edit_placehol
-00000b30: 6465 725f 7465 7874 da38 6169 5f63 6f6e  der_text.8ai_con
-00000b40: 6669 675f 6261 7365 5f73 7973 7465 6d5f  fig_base_system_
-00000b50: 7072 6f6d 7074 5f65 6469 745f 6163 6365  prompt_edit_acce
-00000b60: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
-00000b70: 6f6e da28 6169 5f63 6f6e 6669 675f 6261  on.(ai_config_ba
-00000b80: 7365 5f72 6573 706f 6e73 655f 6d61 785f  se_response_max_
-00000b90: 746f 6b65 6e73 5f6c 6162 656c da3f 6169  tokens_label.?ai
-00000ba0: 5f63 6f6e 6669 675f 6261 7365 5f72 6573  _config_base_res
-00000bb0: 706f 6e73 655f 6d61 785f 746f 6b65 6e73  ponse_max_tokens
-00000bc0: 5f69 6e70 7574 5f61 6363 6573 7369 626c  _input_accessibl
-00000bd0: 655f 6465 7363 7269 7074 696f 6e4e 2901  e_descriptionN).
-00000be0: da07 6c65 7865 6d65 73a9 0072 3200 0000  ..lexemes..r2...
-00000bf0: 7232 0000 00fa 4c2f 5573 6572 732f 7661  r2....L/Users/va
-00000c00: 6469 6b75 732f 5079 6368 6172 6d50 726f  dikus/PycharmPro
-00000c10: 6a65 6374 732f 6e6f 746f 6c6f 672f 6e6f  jects/notolog/no
-00000c20: 746f 6c6f 672f 6c65 7865 6d65 732f 656e  tolog/lexemes/en
-00000c30: 2f73 6574 7469 6e67 735f 6469 616c 6f67  /settings_dialog
-00000c40: 2e70 79da 083c 6d6f 6475 6c65 3e04 0000  .py..<module>...
-00000c50: 0073 5a00 0000 0202 0202 0201 0201 0201  .sZ.............
-00000c60: 0202 0201 0201 0201 0201 0201 0201 0201  ................
-00000c70: 0201 0201 0201 0201 0202 0201 0202 0202  ................
-00000c80: 0201 0201 0202 0201 0201 0201 0201 0201  ................
-00000c90: 0202 0202 0201 0201 0201 0201 0201 0201  ................
-00000ca0: 0201 0202 0201 0201 0202 0201 0201 02c7  ................
+00000080: 6429 642a 642b 642c 642d 642e 642f 9c2f  d)d*d+d,d-d.d/./
+00000090: 5a00 6430 5300 2931 da08 5365 7474 696e  Z.d0S.)1..Settin
+000000a0: 6773 da05 436c 6f73 655a 0747 656e 6572  gs..CloseZ.Gener
+000000b0: 616c 5a06 4564 6974 6f72 5a06 5669 6577  alZ.EditorZ.View
+000000c0: 6572 7a09 4149 2043 6f6e 6669 677a 0a41  erz.AI Configz.A
+000000d0: 7070 2063 6f6e 6669 67da 084c 616e 6775  pp config..Langu
+000000e0: 6167 657a 1143 686f 6f73 6520 6120 6c61  agez.Choose a la
+000000f0: 6e67 7561 6765 7a18 4170 7027 7320 696e  nguagez.App's in
+00000100: 7465 7266 6163 6520 6c61 6e67 7561 6765  terface language
+00000110: da05 5468 656d 657a 0e43 686f 6f73 6520  ..Themez.Choose 
+00000120: 6120 7468 656d 657a 1541 7070 2773 2069  a themez.App's i
+00000130: 6e74 6572 6661 6365 2074 6865 6d65 7a09  nterface themez.
+00000140: 4d61 696e 204d 656e 757a 0e53 686f 7720  Main Menuz.Show 
+00000150: 4d61 696e 204d 656e 757a 2444 6973 706c  Main Menuz$Displ
+00000160: 6179 2074 6865 2061 7070 2773 206d 6169  ay the app's mai
+00000170: 6e20 6472 6f70 646f 776e 206d 656e 757a  n dropdown menuz
+00000180: 1346 6f6e 7420 5369 7a65 3a20 7b73 697a  .Font Size: {siz
+00000190: 657d 7074 7a21 4164 6a75 7374 2074 6865  e}ptz!Adjust the
+000001a0: 2061 7070 2773 2067 6c6f 6261 6c20 666f   app's global fo
+000001b0: 6e74 2073 697a 657a 0a53 7461 7475 7320  nt sizez.Status 
+000001c0: 4261 727a 1b53 686f 7720 476c 6f62 616c  Barz.Show Global
+000001d0: 2043 7572 736f 7220 506f 7369 7469 6f6e   Cursor Position
+000001e0: 7a34 4469 7370 6c61 7920 7468 6520 676c  z4Display the gl
+000001f0: 6f62 616c 2063 7572 736f 7220 706f 7369  obal cursor posi
+00000200: 7469 6f6e 2069 6e20 7468 6520 7374 6174  tion in the stat
+00000210: 7573 2062 6172 7a14 4564 6974 6f72 2043  us barz.Editor C
+00000220: 6f6e 6669 6775 7261 7469 6f6e 7a11 5368  onfigurationz.Sh
+00000230: 6f77 204c 696e 6520 4e75 6d62 6572 737a  ow Line Numbersz
+00000240: 2244 6973 706c 6179 206c 696e 6520 6e75  "Display line nu
+00000250: 6d62 6572 7320 696e 2074 6865 2065 6469  mbers in the edi
+00000260: 746f 727a 1456 6965 7765 7220 436f 6e66  torz.Viewer Conf
+00000270: 6967 7572 6174 696f 6e7a 1f43 6f6e 7665  igurationz.Conve
+00000280: 7274 2054 6578 7420 456d 6f6a 6973 2074  rt Text Emojis t
+00000290: 6f20 4772 6170 6869 6373 7a30 436f 6e76  o Graphicsz0Conv
+000002a0: 6572 7420 7465 7874 2065 6d6f 6a69 7320  ert text emojis 
+000002b0: 746f 2067 7261 7068 6963 616c 2072 6570  to graphical rep
+000002c0: 7265 7365 6e74 6174 696f 6e73 7a0f 4869  resentationsz.Hi
+000002d0: 6768 6c69 6768 7420 544f 444f 737a 2345  ghlight TODOsz#E
+000002e0: 6d70 6861 7369 7a65 2054 4f44 4f20 7461  mphasize TODO ta
+000002f0: 6773 2077 6974 6869 6e20 7468 6520 7465  gs within the te
+00000300: 7874 7a22 5265 7175 6972 6520 436f 6e66  xtz"Require Conf
+00000310: 6972 6d61 7469 6f6e 2074 6f20 4f70 656e  irmation to Open
+00000320: 204c 696e 6b73 7a29 4173 6b20 666f 7220   Linksz)Ask for 
+00000330: 636f 6e66 6972 6d61 7469 6f6e 2062 6566  confirmation bef
+00000340: 6f72 6520 6f70 656e 696e 6720 6c69 6e6b  ore opening link
+00000350: 737a 2141 7574 6f2d 7361 7665 2065 7874  sz!Auto-save ext
+00000360: 6572 6e61 6c20 696d 6167 6573 2074 6f20  ernal images to 
+00000370: 6469 736b 7a49 4175 746f 6d61 7469 6361  diskzIAutomatica
+00000380: 6c6c 7920 7361 7665 7320 636f 7069 6573  lly saves copies
+00000390: 206f 6620 6578 7465 726e 616c 2069 6d61   of external ima
+000003a0: 6765 7320 746f 2064 6973 6b20 666f 7220  ges to disk for 
+000003b0: 6f66 666c 696e 6520 6163 6365 7373 2e7a  offline access.z
+000003c0: 0a4f 7065 6e41 4920 4150 497a 0741 5049  .OpenAI APIz.API
+000003d0: 2055 524c 7a0e 4f70 656e 4149 2041 5049   URLz.OpenAI API
+000003e0: 2055 524c 7a07 4150 4920 6b65 797a 0e4f   URLz.API keyz.O
+000003f0: 7065 6e41 4920 4150 4920 6b65 797a 1053  penAI API keyz.S
+00000400: 7570 706f 7274 6564 206d 6f64 656c 737a  upported modelsz
+00000410: 0c43 686f 6f73 6520 6d6f 6465 6c7a 1a53  .Choose modelz.S
+00000420: 7570 706f 7274 6564 206d 6f64 656c 7320  upported models 
+00000430: 746f 2063 686f 6f73 657a 0f42 6173 6520  to choosez.Base 
+00000440: 5061 7261 6d65 7465 7273 7a0d 5379 7374  Parametersz.Syst
+00000450: 656d 2050 726f 6d70 747a 2d42 6173 6520  em Promptz-Base 
+00000460: 7379 7374 656d 2070 726f 6d70 7420 7468  system prompt th
+00000470: 6174 2070 7265 6365 6465 7320 6561 6368  at precedes each
+00000480: 2072 6571 7565 7374 7a42 4261 7365 2073   requestzBBase s
+00000490: 7973 7465 6d20 7072 6f6d 7074 2074 6861  ystem prompt tha
+000004a0: 7420 7072 6563 6564 6573 2065 6163 6820  t precedes each 
+000004b0: 7265 7175 6573 742e 2054 6869 7320 6973  request. This is
+000004c0: 2070 6c61 696e 2074 6578 742e 7a17 4d61   plain text.z.Ma
+000004d0: 7869 6d75 6d20 5265 7370 6f6e 7365 2054  ximum Response T
+000004e0: 6f6b 656e 737a 2f4d 6178 696d 756d 206e  okensz/Maximum n
+000004f0: 756d 6265 7220 6f66 2074 6f6b 656e 7320  umber of tokens 
+00000500: 746f 2072 6563 6569 7665 2069 6e20 7265  to receive in re
+00000510: 7370 6f6e 7365 292f da0c 7769 6e64 6f77  sponse)/..window
+00000520: 5f74 6974 6c65 da0c 6275 7474 6f6e 5f63  _title..button_c
+00000530: 6c6f 7365 da0b 7461 625f 6765 6e65 7261  lose..tab_genera
+00000540: 6cda 1174 6162 5f65 6469 746f 725f 636f  l..tab_editor_co
+00000550: 6e66 6967 da11 7461 625f 7669 6577 6572  nfig..tab_viewer
+00000560: 5f63 6f6e 6669 67da 0d74 6162 5f61 695f  _config..tab_ai_
+00000570: 636f 6e66 6967 da18 6765 6e65 7261 6c5f  config..general_
+00000580: 6170 705f 636f 6e66 6967 5f6c 6162 656c  app_config_label
+00000590: da1a 6765 6e65 7261 6c5f 6170 705f 6c61  ..general_app_la
+000005a0: 6e67 7561 6765 5f6c 6162 656c da2b 6765  nguage_label.+ge
+000005b0: 6e65 7261 6c5f 6170 705f 6c61 6e67 7561  neral_app_langua
+000005c0: 6765 5f63 6f6d 626f 5f70 6c61 6365 686f  ge_combo_placeho
+000005d0: 6c64 6572 5f74 6578 74da 3167 656e 6572  lder_text.1gener
+000005e0: 616c 5f61 7070 5f6c 616e 6775 6167 655f  al_app_language_
+000005f0: 636f 6d62 6f5f 6163 6365 7373 6962 6c65  combo_accessible
+00000600: 5f64 6573 6372 6970 7469 6f6e da17 6765  _description..ge
+00000610: 6e65 7261 6c5f 6170 705f 7468 656d 655f  neral_app_theme_
+00000620: 6c61 6265 6cda 2867 656e 6572 616c 5f61  label.(general_a
+00000630: 7070 5f74 6865 6d65 5f63 6f6d 626f 5f70  pp_theme_combo_p
+00000640: 6c61 6365 686f 6c64 6572 5f74 6578 74da  laceholder_text.
+00000650: 2e67 656e 6572 616c 5f61 7070 5f74 6865  .general_app_the
+00000660: 6d65 5f63 6f6d 626f 5f61 6363 6573 7369  me_combo_accessi
+00000670: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
+00000680: 1b67 656e 6572 616c 5f61 7070 5f6d 6169  .general_app_mai
+00000690: 6e5f 6d65 6e75 5f6c 6162 656c da1e 6765  n_menu_label..ge
+000006a0: 6e65 7261 6c5f 6170 705f 6d61 696e 5f6d  neral_app_main_m
+000006b0: 656e 755f 6368 6563 6b62 6f78 da35 6765  enu_checkbox.5ge
+000006c0: 6e65 7261 6c5f 6170 705f 6d61 696e 5f6d  neral_app_main_m
+000006d0: 656e 755f 6368 6563 6b62 6f78 5f61 6363  enu_checkbox_acc
+000006e0: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
+000006f0: 696f 6eda 1b67 656e 6572 616c 5f61 7070  ion..general_app
+00000700: 5f66 6f6e 745f 7369 7a65 5f6c 6162 656c  _font_size_label
+00000710: da33 6765 6e65 7261 6c5f 6170 705f 666f  .3general_app_fo
+00000720: 6e74 5f73 697a 655f 736c 6964 6572 5f61  nt_size_slider_a
+00000730: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000740: 7074 696f 6eda 1767 656e 6572 616c 5f73  ption..general_s
+00000750: 7461 7475 7362 6172 5f6c 6162 656c da36  tatusbar_label.6
+00000760: 6765 6e65 7261 6c5f 7374 6174 7573 6261  general_statusba
+00000770: 725f 7368 6f77 5f67 6c6f 6261 6c5f 6375  r_show_global_cu
+00000780: 7273 6f72 5f70 6f73 6974 696f 6e5f 6368  rsor_position_ch
+00000790: 6563 6b62 6f78 da4d 6765 6e65 7261 6c5f  eckbox.Mgeneral_
+000007a0: 7374 6174 7573 6261 725f 7368 6f77 5f67  statusbar_show_g
+000007b0: 6c6f 6261 6c5f 6375 7273 6f72 5f70 6f73  lobal_cursor_pos
+000007c0: 6974 696f 6e5f 6368 6563 6b62 6f78 5f61  ition_checkbox_a
+000007d0: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+000007e0: 7074 696f 6eda 1365 6469 746f 725f 636f  ption..editor_co
+000007f0: 6e66 6967 5f6c 6162 656c da28 6564 6974  nfig_label.(edit
+00000800: 6f72 5f63 6f6e 6669 675f 7368 6f77 5f6c  or_config_show_l
+00000810: 696e 655f 6e75 6d62 6572 735f 6368 6563  ine_numbers_chec
+00000820: 6b62 6f78 da3f 6564 6974 6f72 5f63 6f6e  kbox.?editor_con
+00000830: 6669 675f 7368 6f77 5f6c 696e 655f 6e75  fig_show_line_nu
+00000840: 6d62 6572 735f 6368 6563 6b62 6f78 5f61  mbers_checkbox_a
+00000850: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
+00000860: 7074 696f 6eda 1376 6965 7765 725f 636f  ption..viewer_co
+00000870: 6e66 6967 5f6c 6162 656c da25 7669 6577  nfig_label.%view
+00000880: 6572 5f63 6f6e 6669 675f 7072 6f63 6573  er_config_proces
+00000890: 735f 656d 6f6a 6973 5f63 6865 636b 626f  s_emojis_checkbo
+000008a0: 78da 3c76 6965 7765 725f 636f 6e66 6967  x.<viewer_config
+000008b0: 5f70 726f 6365 7373 5f65 6d6f 6a69 735f  _process_emojis_
+000008c0: 6368 6563 6b62 6f78 5f61 6363 6573 7369  checkbox_accessi
+000008d0: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
+000008e0: 2676 6965 7765 725f 636f 6e66 6967 5f68  &viewer_config_h
+000008f0: 6967 686c 6967 6874 5f74 6f64 6f73 5f63  ighlight_todos_c
+00000900: 6865 636b 626f 78da 3d76 6965 7765 725f  heckbox.=viewer_
+00000910: 636f 6e66 6967 5f68 6967 686c 6967 6874  config_highlight
+00000920: 5f74 6f64 6f73 5f63 6865 636b 626f 785f  _todos_checkbox_
+00000930: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
+00000940: 6970 7469 6f6e da2d 7669 6577 6572 5f63  iption.-viewer_c
+00000950: 6f6e 6669 675f 6f70 656e 5f6c 696e 6b5f  onfig_open_link_
+00000960: 636f 6e66 6972 6d61 7469 6f6e 5f63 6865  confirmation_che
+00000970: 636b 626f 78da 4476 6965 7765 725f 636f  ckbox.Dviewer_co
+00000980: 6e66 6967 5f6f 7065 6e5f 6c69 6e6b 5f63  nfig_open_link_c
+00000990: 6f6e 6669 726d 6174 696f 6e5f 6368 6563  onfirmation_chec
+000009a0: 6b62 6f78 5f61 6363 6573 7369 626c 655f  kbox_accessible_
+000009b0: 6465 7363 7269 7074 696f 6eda 2576 6965  description.%vie
+000009c0: 7765 725f 636f 6e66 6967 5f73 6176 655f  wer_config_save_
+000009d0: 7265 736f 7572 6365 735f 6368 6563 6b62  resources_checkb
+000009e0: 6f78 da3c 7669 6577 6572 5f63 6f6e 6669  ox.<viewer_confi
+000009f0: 675f 7361 7665 5f72 6573 6f75 7263 6573  g_save_resources
+00000a00: 5f63 6865 636b 626f 785f 6163 6365 7373  _checkbox_access
+00000a10: 6962 6c65 5f64 6573 6372 6970 7469 6f6e  ible_description
+00000a20: da1a 6169 5f63 6f6e 6669 675f 6f70 656e  ..ai_config_open
+00000a30: 6169 5f61 7069 5f6c 6162 656c da2f 6169  ai_api_label./ai
+00000a40: 5f63 6f6e 6669 675f 6f70 656e 6169 5f61  _config_openai_a
+00000a50: 7069 5f75 726c 5f69 6e70 7574 5f70 6c61  pi_url_input_pla
+00000a60: 6365 686f 6c64 6572 5f74 6578 74da 3561  ceholder_text.5a
+00000a70: 695f 636f 6e66 6967 5f6f 7065 6e61 695f  i_config_openai_
+00000a80: 6170 695f 7572 6c5f 696e 7075 745f 6163  api_url_input_ac
+00000a90: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
+00000aa0: 7469 6f6e da2f 6169 5f63 6f6e 6669 675f  tion./ai_config_
+00000ab0: 6f70 656e 6169 5f61 7069 5f6b 6579 5f69  openai_api_key_i
+00000ac0: 6e70 7574 5f70 6c61 6365 686f 6c64 6572  nput_placeholder
+00000ad0: 5f74 6578 74da 3561 695f 636f 6e66 6967  _text.5ai_config
+00000ae0: 5f6f 7065 6e61 695f 6170 695f 6b65 795f  _openai_api_key_
+00000af0: 696e 7075 745f 6163 6365 7373 6962 6c65  input_accessible
+00000b00: 5f64 6573 6372 6970 7469 6f6e da2b 6169  _description.+ai
+00000b10: 5f63 6f6e 6669 675f 6f70 656e 6169 5f61  _config_openai_a
+00000b20: 7069 5f73 7570 706f 7274 6564 5f6d 6f64  pi_supported_mod
+00000b30: 656c 735f 6c61 6265 6cda 2f61 695f 636f  els_label./ai_co
+00000b40: 6e66 6967 5f61 695f 6d6f 6465 6c5f 6e61  nfig_ai_model_na
+00000b50: 6d65 735f 636f 6d62 6f5f 706c 6163 6568  mes_combo_placeh
+00000b60: 6f6c 6465 725f 7465 7874 da35 6169 5f63  older_text.5ai_c
+00000b70: 6f6e 6669 675f 6169 5f6d 6f64 656c 5f6e  onfig_ai_model_n
+00000b80: 616d 6573 5f63 6f6d 626f 5f61 6363 6573  ames_combo_acces
+00000b90: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
+00000ba0: 6eda 1461 695f 636f 6e66 6967 5f62 6173  n..ai_config_bas
+00000bb0: 655f 6c61 6265 6cda 2261 695f 636f 6e66  e_label."ai_conf
+00000bc0: 6967 5f62 6173 655f 7379 7374 656d 5f70  ig_base_system_p
+00000bd0: 726f 6d70 745f 6c61 6265 6cda 3261 695f  rompt_label.2ai_
+00000be0: 636f 6e66 6967 5f62 6173 655f 7379 7374  config_base_syst
+00000bf0: 656d 5f70 726f 6d70 745f 6564 6974 5f70  em_prompt_edit_p
+00000c00: 6c61 6365 686f 6c64 6572 5f74 6578 74da  laceholder_text.
+00000c10: 3861 695f 636f 6e66 6967 5f62 6173 655f  8ai_config_base_
+00000c20: 7379 7374 656d 5f70 726f 6d70 745f 6564  system_prompt_ed
+00000c30: 6974 5f61 6363 6573 7369 626c 655f 6465  it_accessible_de
+00000c40: 7363 7269 7074 696f 6eda 2861 695f 636f  scription.(ai_co
+00000c50: 6e66 6967 5f62 6173 655f 7265 7370 6f6e  nfig_base_respon
+00000c60: 7365 5f6d 6178 5f74 6f6b 656e 735f 6c61  se_max_tokens_la
+00000c70: 6265 6cda 3f61 695f 636f 6e66 6967 5f62  bel.?ai_config_b
+00000c80: 6173 655f 7265 7370 6f6e 7365 5f6d 6178  ase_response_max
+00000c90: 5f74 6f6b 656e 735f 696e 7075 745f 6163  _tokens_input_ac
+00000ca0: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
+00000cb0: 7469 6f6e 4e29 01da 076c 6578 656d 6573  tionN)...lexemes
+00000cc0: a900 7235 0000 0072 3500 0000 fa4c 2f55  ..r5...r5....L/U
+00000cd0: 7365 7273 2f76 6164 696b 7573 2f50 7963  sers/vadikus/Pyc
+00000ce0: 6861 726d 5072 6f6a 6563 7473 2f6e 6f74  harmProjects/not
+00000cf0: 6f6c 6f67 2d64 6576 2f61 7070 2f6c 6578  olog-dev/app/lex
+00000d00: 656d 6573 2f65 6e2f 7365 7474 696e 6773  emes/en/settings
+00000d10: 5f64 6961 6c6f 672e 7079 da08 3c6d 6f64  _dialog.py..<mod
+00000d20: 756c 653e 0400 0000 735e 0000 0002 0202  ule>....s^......
+00000d30: 0202 0102 0102 0102 0202 0102 0102 0102  ................
+00000d40: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00000d50: 0202 0102 0202 0202 0102 0102 0202 0102  ................
+00000d60: 0102 0102 0102 0102 0202 0102 0202 0202  ................
+00000d70: 0102 0102 0102 0102 0102 0102 0102 0202  ................
+00000d80: 0102 0102 0202 0102 0102 c4              ...........
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/it/__pycache__/statusbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 1201 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,81 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 b104 0000  a.......(..f....
+00000000: 610d 0d0a 0000 0000 b254 2c66 d604 0000  a........T,f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
-00000050: 6411 9c11 5a00 6412 5300 2913 7a0a 4c69  d...Z.d.S.).z.Li
-00000060: 7474 6572 2062 696e 7a17 5368 6f77 206c  tter binz.Show l
-00000070: 6974 7465 7220 6269 6e20 636f 6e74 656e  itter bin conten
-00000080: 7473 0400 0000 f09f 92be 7304 0000 00f0  ts........s.....
-00000090: 9f94 9273 0400 0000 f09f 9493 7a09 5669  ...s........z.Vi
-000000a0: 6577 206d 6f64 657a 0945 6469 7420 6d6f  ew modez.Edit mo
-000000b0: 6465 7a0b 536f 7572 6365 206d 6f64 65da  dez.Source mode.
-000000c0: 084d 6172 6b64 6f77 6eda 0448 544d 4c7a  .Markdown..HTMLz
-000000d0: 137b 656e 6372 7970 7469 6f6e 7d20 7b69  .{encryption} {i
-000000e0: 636f 6e7d da05 506c 6169 6e5a 0945 6e63  con}..PlainZ.Enc
-000000f0: 7279 7074 6564 751e 0000 006c 696e 653a  ryptedu....line:
-00000100: 207b 6c69 6e65 7d20 e286 9220 636f 6c3a   {line} ... col:
-00000110: 207b 636f 6c75 6d6e 7d75 3200 0000 6c69   {column}u2...li
-00000120: 6e65 3a20 7b6c 696e 657d 20e2 8692 2063  ne: {line} ... c
-00000130: 6f6c 3a20 7b63 6f6c 756d 6e7d 20e2 8692  ol: {column} ...
-00000140: 2073 656c 3a20 7b73 656c 6563 7465 647d   sel: {selected}
-00000150: 7532 0000 006c 696e 653a 207b 6c69 6e65  u2...line: {line
-00000160: 7d20 e286 9220 636f 6c3a 207b 636f 6c75  } ... col: {colu
-00000170: 6d6e 7d20 e286 9220 706f 733a 207b 706f  mn} ... pos: {po
-00000180: 7369 7469 6f6e 7d75 4600 0000 6c69 6e65  sition}uF...line
-00000190: 3a20 7b6c 696e 657d 20e2 8692 2063 6f6c  : {line} ... col
-000001a0: 3a20 7b63 6f6c 756d 6e7d 20e2 8692 2070  : {column} ... p
-000001b0: 6f73 3a20 7b70 6f73 6974 696f 6e7d 20e2  os: {position} .
-000001c0: 8692 2073 656c 3a20 7b73 656c 6563 7465  .. sel: {selecte
-000001d0: 647d 2911 da1a 7374 6174 7573 6261 725f  d})...statusbar_
-000001e0: 6c69 7474 6572 5f62 696e 5f6c 6162 656c  litter_bin_label
-000001f0: da24 7374 6174 7573 6261 725f 6c69 7474  .$statusbar_litt
-00000200: 6572 5f62 696e 5f61 6363 6573 7369 626c  er_bin_accessibl
-00000210: 655f 6e61 6d65 da1d 7374 6174 7573 6261  e_name..statusba
-00000220: 725f 7361 7665 5f70 726f 6772 6573 735f  r_save_progress_
-00000230: 6c61 6265 6cda 2b73 7461 7475 7362 6172  label.+statusbar
-00000240: 5f65 6e63 7279 7074 696f 6e5f 7379 6d62  _encryption_symb
-00000250: 6f6c 5f65 6e63 7279 7074 6564 5f6c 6162  ol_encrypted_lab
-00000260: 656c da2d 7374 6174 7573 6261 725f 656e  el.-statusbar_en
-00000270: 6372 7970 7469 6f6e 5f73 796d 626f 6c5f  cryption_symbol_
-00000280: 756e 656e 6372 7970 7465 645f 6c61 6265  unencrypted_labe
-00000290: 6c5a 1e73 7461 7475 7362 6172 5f6d 6f64  lZ.statusbar_mod
-000002a0: 655f 6c61 6265 6c5f 6d6f 6465 5f76 6965  e_label_mode_vie
-000002b0: 775a 1e73 7461 7475 7362 6172 5f6d 6f64  wZ.statusbar_mod
-000002c0: 655f 6c61 6265 6c5f 6d6f 6465 5f65 6469  e_label_mode_edi
-000002d0: 745a 2073 7461 7475 7362 6172 5f6d 6f64  tZ statusbar_mod
-000002e0: 655f 6c61 6265 6c5f 6d6f 6465 5f73 6f75  e_label_mode_sou
-000002f0: 7263 655a 2673 7461 7475 7362 6172 5f73  rceZ&statusbar_s
-00000300: 6f75 7263 655f 6c61 6265 6c5f 736f 7572  ource_label_sour
-00000310: 6365 5f6d 6172 6b64 6f77 6e5a 2273 7461  ce_markdownZ"sta
-00000320: 7475 7362 6172 5f73 6f75 7263 655f 6c61  tusbar_source_la
-00000330: 6265 6c5f 736f 7572 6365 5f68 746d 6cda  bel_source_html.
-00000340: 1a73 7461 7475 7362 6172 5f65 6e63 7279  .statusbar_encry
-00000350: 7074 696f 6e5f 6c61 6265 6c5a 2b73 7461  ption_labelZ+sta
-00000360: 7475 7362 6172 5f65 6e63 7279 7074 696f  tusbar_encryptio
-00000370: 6e5f 6c61 6265 6c5f 656e 6372 7970 7469  n_label_encrypti
-00000380: 6f6e 5f70 6c61 696e 5a2f 7374 6174 7573  on_plainZ/status
-00000390: 6261 725f 656e 6372 7970 7469 6f6e 5f6c  bar_encryption_l
-000003a0: 6162 656c 5f65 6e63 7279 7074 696f 6e5f  abel_encryption_
-000003b0: 656e 6372 7970 7465 64da 1673 7461 7475  encrypted..statu
-000003c0: 7362 6172 5f63 7572 736f 725f 6c61 6265  sbar_cursor_labe
-000003d0: 6cda 1f73 7461 7475 7362 6172 5f63 7572  l..statusbar_cur
-000003e0: 736f 725f 6c61 6265 6c5f 7365 6c65 6374  sor_label_select
-000003f0: 6564 da22 7374 6174 7573 6261 725f 6375  ed."statusbar_cu
-00000400: 7273 6f72 5f6c 6162 656c 5f77 6974 685f  rsor_label_with_
-00000410: 676c 6f62 616c da2b 7374 6174 7573 6261  global.+statusba
-00000420: 725f 6375 7273 6f72 5f6c 6162 656c 5f73  r_cursor_label_s
-00000430: 656c 6563 7465 645f 7769 7468 5f67 6c6f  elected_with_glo
-00000440: 6261 6c4e 2901 da07 6c65 7865 6d65 73a9  balN)...lexemes.
-00000450: 0072 0f00 0000 720f 0000 00fa 462f 5573  .r....r.....F/Us
-00000460: 6572 732f 7661 6469 6b75 732f 5079 6368  ers/vadikus/Pych
-00000470: 6172 6d50 726f 6a65 6374 732f 6e6f 746f  armProjects/noto
-00000480: 6c6f 672f 6e6f 746f 6c6f 672f 6c65 7865  log/notolog/lexe
-00000490: 6d65 732f 656e 2f73 7461 7475 7362 6172  mes/en/statusbar
-000004a0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
-000004b0: 0073 2200 0000 0201 0202 0201 0201 0202  .s".............
-000004c0: 0201 0201 0202 0201 0202 0201 0201 0202  ................
-000004d0: 0201 0201 0201 02ea                      ........
+00000050: 6411 9c11 5a00 6412 5300 2913 5a07 4365  d...Z.d.S.).Z.Ce
+00000060: 7374 696e 6f7a 1f4d 6f73 7472 6120 696c  stinoz.Mostra il
+00000070: 2063 6f6e 7465 6e75 746f 2064 656c 2063   contenuto del c
+00000080: 6573 7469 6e6f 7304 0000 00f0 9f92 be73  estinos........s
+00000090: 0400 0000 f09f 9492 7304 0000 00f0 9f94  ........s.......
+000000a0: 9375 1400 0000 4d6f 6461 6c69 74c3 a020  .u....Modalit.. 
+000000b0: 5669 7375 616c 697a 7a61 7512 0000 004d  Visualizzau....M
+000000c0: 6f64 616c 6974 c3a0 204d 6f64 6966 6963  odalit.. Modific
+000000d0: 6175 1200 0000 4d6f 6461 6c69 74c3 a020  au....Modalit.. 
+000000e0: 536f 7267 656e 7465 da08 4d61 726b 646f  Sorgente..Markdo
+000000f0: 776e da04 4854 4d4c 7a13 7b65 6e63 7279  wn..HTMLz.{encry
+00000100: 7074 696f 6e7d 207b 6963 6f6e 7d5a 074e  ption} {icon}Z.N
+00000110: 6f72 6d61 6c65 5a08 4372 6970 7461 746f  ormaleZ.Criptato
+00000120: 751f 0000 006c 696e 6561 3a20 7b6c 696e  u....linea: {lin
+00000130: 657d 20e2 8692 2063 6f6c 3a20 7b63 6f6c  e} ... col: {col
+00000140: 756d 6e7d 7533 0000 006c 696e 6561 3a20  umn}u3...linea: 
+00000150: 7b6c 696e 657d 20e2 8692 2063 6f6c 3a20  {line} ... col: 
+00000160: 7b63 6f6c 756d 6e7d 20e2 8692 2073 656c  {column} ... sel
+00000170: 3a20 7b73 656c 6563 7465 647d 7533 0000  : {selected}u3..
+00000180: 006c 696e 6561 3a20 7b6c 696e 657d 20e2  .linea: {line} .
+00000190: 8692 2063 6f6c 3a20 7b63 6f6c 756d 6e7d  .. col: {column}
+000001a0: 20e2 8692 2070 6f73 3a20 7b70 6f73 6974   ... pos: {posit
+000001b0: 696f 6e7d 7547 0000 006c 696e 6561 3a20  ion}uG...linea: 
+000001c0: 7b6c 696e 657d 20e2 8692 2063 6f6c 3a20  {line} ... col: 
+000001d0: 7b63 6f6c 756d 6e7d 20e2 8692 2070 6f73  {column} ... pos
+000001e0: 3a20 7b70 6f73 6974 696f 6e7d 20e2 8692  : {position} ...
+000001f0: 2073 656c 3a20 7b73 656c 6563 7465 647d   sel: {selected}
+00000200: 2911 da1a 7374 6174 7573 6261 725f 6c69  )...statusbar_li
+00000210: 7474 6572 5f62 696e 5f6c 6162 656c da24  tter_bin_label.$
+00000220: 7374 6174 7573 6261 725f 6c69 7474 6572  statusbar_litter
+00000230: 5f62 696e 5f61 6363 6573 7369 626c 655f  _bin_accessible_
+00000240: 6e61 6d65 da1d 7374 6174 7573 6261 725f  name..statusbar_
+00000250: 7361 7665 5f70 726f 6772 6573 735f 6c61  save_progress_la
+00000260: 6265 6cda 2b73 7461 7475 7362 6172 5f65  bel.+statusbar_e
+00000270: 6e63 7279 7074 696f 6e5f 7379 6d62 6f6c  ncryption_symbol
+00000280: 5f65 6e63 7279 7074 6564 5f6c 6162 656c  _encrypted_label
+00000290: da2d 7374 6174 7573 6261 725f 656e 6372  .-statusbar_encr
+000002a0: 7970 7469 6f6e 5f73 796d 626f 6c5f 756e  yption_symbol_un
+000002b0: 656e 6372 7970 7465 645f 6c61 6265 6cda  encrypted_label.
+000002c0: 1e73 7461 7475 7362 6172 5f6d 6f64 655f  .statusbar_mode_
+000002d0: 6c61 6265 6c5f 6d6f 6465 5f76 6965 77da  label_mode_view.
+000002e0: 1e73 7461 7475 7362 6172 5f6d 6f64 655f  .statusbar_mode_
+000002f0: 6c61 6265 6c5f 6d6f 6465 5f65 6469 74da  label_mode_edit.
+00000300: 2073 7461 7475 7362 6172 5f6d 6f64 655f   statusbar_mode_
+00000310: 6c61 6265 6c5f 6d6f 6465 5f73 6f75 7263  label_mode_sourc
+00000320: 65da 2673 7461 7475 7362 6172 5f73 6f75  e.&statusbar_sou
+00000330: 7263 655f 6c61 6265 6c5f 736f 7572 6365  rce_label_source
+00000340: 5f6d 6172 6b64 6f77 6eda 2273 7461 7475  _markdown."statu
+00000350: 7362 6172 5f73 6f75 7263 655f 6c61 6265  sbar_source_labe
+00000360: 6c5f 736f 7572 6365 5f68 746d 6cda 1a73  l_source_html..s
+00000370: 7461 7475 7362 6172 5f65 6e63 7279 7074  tatusbar_encrypt
+00000380: 696f 6e5f 6c61 6265 6cda 2b73 7461 7475  ion_label.+statu
+00000390: 7362 6172 5f65 6e63 7279 7074 696f 6e5f  sbar_encryption_
+000003a0: 6c61 6265 6c5f 656e 6372 7970 7469 6f6e  label_encryption
+000003b0: 5f70 6c61 696e da2f 7374 6174 7573 6261  _plain./statusba
+000003c0: 725f 656e 6372 7970 7469 6f6e 5f6c 6162  r_encryption_lab
+000003d0: 656c 5f65 6e63 7279 7074 696f 6e5f 656e  el_encryption_en
+000003e0: 6372 7970 7465 64da 1673 7461 7475 7362  crypted..statusb
+000003f0: 6172 5f63 7572 736f 725f 6c61 6265 6cda  ar_cursor_label.
+00000400: 1f73 7461 7475 7362 6172 5f63 7572 736f  .statusbar_curso
+00000410: 725f 6c61 6265 6c5f 7365 6c65 6374 6564  r_label_selected
+00000420: da22 7374 6174 7573 6261 725f 6375 7273  ."statusbar_curs
+00000430: 6f72 5f6c 6162 656c 5f77 6974 685f 676c  or_label_with_gl
+00000440: 6f62 616c da2b 7374 6174 7573 6261 725f  obal.+statusbar_
+00000450: 6375 7273 6f72 5f6c 6162 656c 5f73 656c  cursor_label_sel
+00000460: 6563 7465 645f 7769 7468 5f67 6c6f 6261  ected_with_globa
+00000470: 6c4e 2901 da07 6c65 7865 6d65 73a9 0072  lN)...lexemes..r
+00000480: 1500 0000 7215 0000 00fa 4a2f 5573 6572  ....r.....J/User
+00000490: 732f 7661 6469 6b75 732f 5079 6368 6172  s/vadikus/Pychar
+000004a0: 6d50 726f 6a65 6374 732f 6e6f 746f 6c6f  mProjects/notolo
+000004b0: 672d 6465 762f 6e6f 746f 6c6f 672f 6c65  g-dev/notolog/le
+000004c0: 7865 6d65 732f 6974 2f73 7461 7475 7362  xemes/it/statusb
+000004d0: 6172 2e70 79da 083c 6d6f 6475 6c65 3e03  ar.py..<module>.
+000004e0: 0000 0073 2200 0000 0201 0202 0201 0201  ...s"...........
+000004f0: 0202 0201 0201 0202 0201 0202 0201 0201  ................
+00000500: 0202 0201 0201 0201 02ea                 ..........
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/en/__pycache__/toolbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:24 2024 UTC, .py size: 2573 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 28c4 2e66 0d0a 0000  a.......(..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 0d0a 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0032 0000 0040 0000 0073 6c00 0000 6400  .2...@...sl...d.
 00000030: 6400 6401 6402 6403 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 6423 6424 6425 6426 6427  d d!d"d#d$d%d&d'
@@ -59,19 +59,19 @@
 000003a0: 5f6e 6577 5f64 6f63 756d 656e 74da 1261  _new_document..a
 000003b0: 6374 696f 6e73 5f6c 6162 656c 5f6f 7065  ctions_label_ope
 000003c0: 6eda 1c61 6374 696f 6e73 5f61 6363 6573  n..actions_acces
 000003d0: 7369 626c 655f 6e61 6d65 5f6f 7065 6eda  sible_name_open.
 000003e0: 1261 6374 696f 6e73 5f6c 6162 656c 5f73  .actions_label_s
 000003f0: 6176 65da 1c61 6374 696f 6e73 5f61 6363  ave..actions_acc
 00000400: 6573 7369 626c 655f 6e61 6d65 5f73 6176  essible_name_sav
-00000410: 655a 1561 6374 696f 6e73 5f6c 6162 656c  eZ.actions_label
-00000420: 5f73 6176 655f 6173 5a1f 6163 7469 6f6e  _save_asZ.action
+00000410: 65da 1561 6374 696f 6e73 5f6c 6162 656c  e..actions_label
+00000420: 5f73 6176 655f 6173 da1f 6163 7469 6f6e  _save_as..action
 00000430: 735f 6163 6365 7373 6962 6c65 5f6e 616d  s_accessible_nam
-00000440: 655f 7361 7665 5f61 735a 1261 6374 696f  e_save_asZ.actio
-00000450: 6e73 5f6c 6162 656c 5f73 796e 635a 1c61  ns_label_syncZ.a
+00000440: 655f 7361 7665 5f61 73da 1261 6374 696f  e_save_as..actio
+00000450: 6e73 5f6c 6162 656c 5f73 796e 63da 1c61  ns_label_sync..a
 00000460: 6374 696f 6e73 5f61 6363 6573 7369 626c  ctions_accessibl
 00000470: 655f 6e61 6d65 5f73 796e 63da 1261 6374  e_name_sync..act
 00000480: 696f 6e73 5f6c 6162 656c 5f65 6469 74da  ions_label_edit.
 00000490: 1c61 6374 696f 6e73 5f61 6363 6573 7369  .actions_accessi
 000004a0: 626c 655f 6e61 6d65 5f65 6469 74da 1461  ble_name_edit..a
 000004b0: 6374 696f 6e73 5f6c 6162 656c 5f73 6f75  ctions_label_sou
 000004c0: 7263 65da 1e61 6374 696f 6e73 5f61 6363  rce..actions_acc
@@ -137,19 +137,19 @@
 00000880: 6275 7474 6f6e 735f 6c61 6265 6c5f 6e65  buttons_label_ne
 00000890: 7874 da23 7365 6172 6368 5f62 7574 746f  xt.#search_butto
 000008a0: 6e73 5f61 6363 6573 7369 626c 655f 6e61  ns_accessible_na
 000008b0: 6d65 5f6e 6578 74da 1573 6561 7263 685f  me_next..search_
 000008c0: 6361 7365 5f73 656e 7369 7469 7665 da19  case_sensitive..
 000008d0: 7365 6172 6368 5f6d 6174 6368 5f63 6173  search_match_cas
 000008e0: 655f 746f 6f6c 7469 704e 2901 da07 6c65  e_tooltipN)...le
-000008f0: 7865 6d65 73a9 0072 3b00 0000 723b 0000  xemes..r;...r;..
+000008f0: 7865 6d65 73a9 0072 3f00 0000 723f 0000  xemes..r?...r?..
 00000900: 00fa 442f 5573 6572 732f 7661 6469 6b75  ..D/Users/vadiku
 00000910: 732f 5079 6368 6172 6d50 726f 6a65 6374  s/PycharmProject
-00000920: 732f 6e6f 746f 6c6f 672f 6e6f 746f 6c6f  s/notolog/notolo
-00000930: 672f 6c65 7865 6d65 732f 656e 2f74 6f6f  g/lexemes/en/too
+00000920: 732f 6e6f 746f 6c6f 672d 6465 762f 6170  s/notolog-dev/ap
+00000930: 702f 6c65 7865 6d65 732f 656e 2f74 6f6f  p/lexemes/en/too
 00000940: 6c62 6172 2e70 79da 083c 6d6f 6475 6c65  lbar.py..<module
 00000950: 3e03 0000 0073 6200 0000 0201 0201 0201  >....sb.........
 00000960: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00000970: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00000980: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00000990: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 000009a0: 0201 0201 0202 0201 0201 0201 0201 0201  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/en/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/en/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/common.py` & `notolog-0.9.0b11/app/lexemes/en/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # English lexemes common.py
 lexemes = {
-    "app_title": "Name Editor",
+    "app_title": "Notolog Editor",
     "app_title_with_sub": "{app_title} - {sub_title}",
 
     "tree_filter_accessible_desc": "File filter field",
 
     "menu_action_rename": "Rename",
     "menu_action_delete": "Delete",
     "menu_action_delete_completely": "Delete completely",
@@ -93,14 +93,15 @@
     "popup_about_title": "Application Info",
     "popup_about_app_name_description": "Markdown Editor",
 
     "popup_about_version": "Version",
     "popup_about_license": "License",
     "popup_about_website": "Website",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Date",
 
     "update_helper_new_version_is_available": "A new version '{latest_version}' of the app is available",
     "update_helper_latest_version_installed": "The latest version of the app is installed",
 
     "network_connection_error_empty": "Cannot obtain response information",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/main_menu.py` & `notolog-0.9.0b11/app/lexemes/en/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/zh/settings_dialog.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,62 @@
-# English lexemes settings_dialog.py
+# Chinese lexemes settings_dialog.py
 lexemes = {
-    # Settings dialog
-    "window_title": "Settings",
+    # 设置
+    "window_title": "设置",
 
-    "button_close": "Close",
+    "button_close": "关闭",
 
-    "tab_general": "General",
-    "tab_editor_config": "Editor",
-    "tab_viewer_config": "Viewer",
-    "tab_ai_config": "AI Config",
-
-    "general_app_config_label": "App config",
-    "general_app_language_label": "Language",
-    "general_app_language_combo_placeholder_text": "Choose a language",
-    "general_app_language_combo_accessible_description": "App's interface language",
-    "general_app_theme_label": "Theme",
-    "general_app_theme_combo_placeholder_text": "Choose a theme",
-    "general_app_theme_combo_accessible_description": "App's interface theme",
-    "general_app_main_menu_label": "Main Menu",
-    "general_app_main_menu_checkbox": "Show Main Menu",
-    "general_app_main_menu_checkbox_accessible_description": "Display the app's main dropdown menu",
-    "general_app_font_size_label": "Font Size: {size}pt",
-    "general_app_font_size_slider_accessible_description": "Adjust the app's global font size",
+    "tab_general": "通用",
+    "tab_editor_config": "编辑器",
+    "tab_viewer_config": "查看器",
+    "tab_ai_config": "AI 配置",
+
+    "general_app_config_label": "应用配置",
+    "general_app_language_label": "语言",
+    "general_app_language_combo_placeholder_text": "选择语言",
+    "general_app_language_combo_accessible_description": "应用界面语言",
+    "general_app_theme_label": "主题",
+    "general_app_theme_combo_placeholder_text": "选择主题",
+    "general_app_theme_combo_accessible_description": "应用界面主题",
+    "general_app_main_menu_label": "主菜单",
+    "general_app_main_menu_checkbox": "显示主菜单",
+    "general_app_main_menu_checkbox_accessible_description": "显示应用的主下拉菜单",
+    "general_app_font_size_label": "字体大小：{size}pt",
+    "general_app_font_size_slider_accessible_description": "调整应用程序的全局字体大小",
 
-    "general_statusbar_label": "Status Bar",
-    "general_statusbar_show_global_cursor_position_checkbox": "Show Global Cursor Position",
+    "general_statusbar_label": "状态栏",
+    "general_statusbar_show_global_cursor_position_checkbox": "显示全局光标位置",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "Display the global cursor position in the status bar",
+        "在状态栏显示全局光标位置",
 
-    "editor_config_label": "Editor Configuration",
-    "editor_config_show_line_numbers_checkbox": "Show Line Numbers",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "Display line numbers in the editor",
-
-    "viewer_config_label": "Viewer Configuration",
-    "viewer_config_process_emojis_checkbox": "Convert Text Emojis to Graphics",
-    "viewer_config_process_emojis_checkbox_accessible_description": "Convert text emojis to graphical representations",
-    "viewer_config_highlight_todos_checkbox": "Highlight TODOs",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "Emphasize TODO tags within the text",
-    "viewer_config_open_link_confirmation_checkbox": "Require Confirmation to Open Links",
+    "editor_config_label": "编辑器配置",
+    "editor_config_show_line_numbers_checkbox": "显示行号",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "在编辑器中显示行号",
+
+    "viewer_config_label": "查看器配置",
+    "viewer_config_process_emojis_checkbox": "将文本表情转换为图形",
+    "viewer_config_process_emojis_checkbox_accessible_description": "将文本表情转换为图形表示",
+    "viewer_config_highlight_todos_checkbox": "突出显示待办事项",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "在文本中突出显示待办事项标签",
+    "viewer_config_open_link_confirmation_checkbox": "打开链接前需确认",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "Ask for confirmation before opening links",
+        "打开链接前询问确认",
+    "viewer_config_save_resources_checkbox": "自动保存外部图片到硬盘",
+    "viewer_config_save_resources_checkbox_accessible_description": "自动将外部图片的副本保存到硬盘以供离线访问。",
 
     "ai_config_openai_api_label": "OpenAI API",
-    "ai_config_openai_api_url_input_placeholder_text": "API URL",
-    "ai_config_openai_api_url_input_accessible_description": "OpenAI API URL",
-    "ai_config_openai_api_key_input_placeholder_text": "API key",
-    "ai_config_openai_api_key_input_accessible_description": "OpenAI API key",
-    "ai_config_openai_api_supported_models_label": "Supported models",
-    "ai_config_ai_model_names_combo_placeholder_text": "Choose model",
-    "ai_config_ai_model_names_combo_accessible_description": "Supported models to choose",
-
-    "ai_config_base_label": "Base Parameters",
-    "ai_config_base_system_prompt_label": "System Prompt",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Base system prompt that precedes each request",
+    "ai_config_openai_api_url_input_placeholder_text": "API 地址",
+    "ai_config_openai_api_url_input_accessible_description": "OpenAI API 地址",
+    "ai_config_openai_api_key_input_placeholder_text": "API 密钥",
+    "ai_config_openai_api_key_input_accessible_description": "OpenAI API 密钥",
+    "ai_config_openai_api_supported_models_label": "支持的模型",
+    "ai_config_ai_model_names_combo_placeholder_text": "选择模型",
+    "ai_config_ai_model_names_combo_accessible_description": "选择支持的模型",
+
+    "ai_config_base_label": "基础参数",
+    "ai_config_base_system_prompt_label": "系统提示",
+    "ai_config_base_system_prompt_edit_placeholder_text": "基础系统提示，位于每个请求之前",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "Base system prompt that precedes each request. This is plain text.",
-    "ai_config_base_response_max_tokens_label": "Maximum Response Tokens",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum number of tokens to receive in response",
+        "基础系统提示，位于每个请求之前。纯文本。",
+    "ai_config_base_response_max_tokens_label": "响应的最大令牌数",
+    "ai_config_base_response_max_tokens_input_accessible_description": "响应中接收的最大令牌数",
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `notolog-0.9.0b10/app/lexemes/en/statusbar.py` & `notolog-0.9.0b11/app/lexemes/en/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/en/toolbar.py` & `notolog-0.9.0b11/app/lexemes/en/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/es/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/es/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/common.py` & `notolog-0.9.0b11/app/lexemes/es/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Información de la Aplicación",
     "popup_about_app_name_description": "Editor Markdown",
 
     "popup_about_version": "Versión",
     "popup_about_license": "Licencia",
     "popup_about_website": "Sitio Web",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Fecha",
 
     "update_helper_new_version_is_available": "Una nueva versión '{latest_version}' de la aplicación está disponible",
     "update_helper_latest_version_installed": "La última versión de la aplicación está instalada",
 
     "network_connection_error_empty": "No se puede obtener información de la respuesta",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/es/main_menu.py` & `notolog-0.9.0b11/app/lexemes/es/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/es/settings_dialog.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     "viewer_config_process_emojis_checkbox_accessible_description":
         "Convertir emojis de texto en representaciones gráficas",
     "viewer_config_highlight_todos_checkbox": "Resaltar TODOs",
     "viewer_config_highlight_todos_checkbox_accessible_description": "Resaltar etiquetas TODO en el texto",
     "viewer_config_open_link_confirmation_checkbox": "Requerir confirmación para abrir enlaces",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "Solicitar confirmación antes de abrir enlaces",
+    "viewer_config_save_resources_checkbox": "Guardar automáticamente imágenes externas en el disco",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Guarda automáticamente copias de imágenes externas en el disco para acceso sin conexión.",
 
     "ai_config_openai_api_label": "API de OpenAI",
     "ai_config_openai_api_url_input_placeholder_text": "URL de la API",
     "ai_config_openai_api_url_input_accessible_description": "URL de la API de OpenAI",
     "ai_config_openai_api_key_input_placeholder_text": "Clave de la API",
     "ai_config_openai_api_key_input_accessible_description": "Clave de la API de OpenAI",
     "ai_config_openai_api_supported_models_label": "Modelos soportados",
```

### Comparing `notolog-0.9.0b10/app/lexemes/es/statusbar.py` & `notolog-0.9.0b11/app/lexemes/es/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/es/toolbar.py` & `notolog-0.9.0b11/app/lexemes/es/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/fr/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/fr/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/common.py` & `notolog-0.9.0b11/app/lexemes/fr/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Infos de l'Application",
     "popup_about_app_name_description": "Éditeur Markdown",
 
     "popup_about_version": "Version",
     "popup_about_license": "Licence",
     "popup_about_website": "Site Web",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Date",
 
     "update_helper_new_version_is_available": "Une nouvelle version '{latest_version}' de l'application est disponible",
     "update_helper_latest_version_installed": "La dernière version de l'application est installée",
 
     "network_connection_error_empty": "Impossible d'obtenir des informations de réponse",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/fr/main_menu.py` & `notolog-0.9.0b11/app/lexemes/fr/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/la/settings_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-# French lexemes settings_dialog.py
+# Latin lexemes settings_dialog.py
 lexemes = {
-    # Paramètres
-    "window_title": "Paramètres",
+    # Configurationes
+    "window_title": "Configurationes",
 
-    "button_close": "Fermer",
+    "button_close": "Claudere",
 
-    "tab_general": "Général",
-    "tab_editor_config": "Éditeur",
-    "tab_viewer_config": "Visualiseur",
-    "tab_ai_config": "Config IA",
-
-    "general_app_config_label": "Configuration de l'application",
-    "general_app_language_label": "Langue",
-    "general_app_language_combo_placeholder_text": "Choisir une langue",
-    "general_app_language_combo_accessible_description": "Langue de l'interface de l'application",
-    "general_app_theme_label": "Thème",
-    "general_app_theme_combo_placeholder_text": "Choisir un thème",
-    "general_app_theme_combo_accessible_description": "Thème de l'interface de l'application",
-    "general_app_main_menu_label": "Menu Principal",
-    "general_app_main_menu_checkbox": "Afficher le menu principal",
-    "general_app_main_menu_checkbox_accessible_description": "Afficher le menu déroulant principal de l'application",
-    "general_app_font_size_label": "Taille de police : {size}pt",
-    "general_app_font_size_slider_accessible_description": "Ajuster la taille de la police globale de l'application",
+    "tab_general": "Generale",
+    "tab_editor_config": "Editor",
+    "tab_viewer_config": "Visor",
+    "tab_ai_config": "Configuratio AI",
+
+    "general_app_config_label": "Configuratio App",
+    "general_app_language_label": "Lingua",
+    "general_app_language_combo_placeholder_text": "Elige linguam",
+    "general_app_language_combo_accessible_description": "Lingua interfaciei app",
+    "general_app_theme_label": "Thema",
+    "general_app_theme_combo_placeholder_text": "Elige thema",
+    "general_app_theme_combo_accessible_description": "Thema interfaciei app",
+    "general_app_main_menu_label": "Praecipuum Menu",
+    "general_app_main_menu_checkbox": "Praecipuum Menu Ostende",
+    "general_app_main_menu_checkbox_accessible_description": "Praecipuum dropdown menu applicationis ostendere",
+    "general_app_font_size_label": "Magnitudo Fontis: {size}pt",
+    "general_app_font_size_slider_accessible_description": "Regula magnitudinem fontis globalis applicationis",
 
-    "general_statusbar_label": "Barre de statut",
-    "general_statusbar_show_global_cursor_position_checkbox": "Afficher la position globale du curseur",
+    "general_statusbar_label": "Status Barra",
+    "general_statusbar_show_global_cursor_position_checkbox": "Ostende Globalem Cursoris Positionem",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "Afficher la position globale du curseur dans la barre de statut",
+        "Ostende globalem cursoris positionem in status barra",
 
-    "editor_config_label": "Configuration de l'éditeur",
-    "editor_config_show_line_numbers_checkbox": "Afficher les numéros de ligne",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "Afficher les numéros de ligne dans l'éditeur",
+    "editor_config_label": "Editoris Configuratio",
+    "editor_config_show_line_numbers_checkbox": "Ostende Numeros Linearum",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "Ostende numeros linearum in editor",
 
-    "viewer_config_label": "Configuration du visualiseur",
-    "viewer_config_process_emojis_checkbox": "Convertir les emojis de texte en graphiques",
+    "viewer_config_label": "Visoris Configuratio",
+    "viewer_config_process_emojis_checkbox": "Converte Textum Emojis ad Graphica",
     "viewer_config_process_emojis_checkbox_accessible_description":
-        "Convertir les emojis de texte en représentations graphiques",
-    "viewer_config_highlight_todos_checkbox": "Mettre en évidence les TODO",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "Souligner les balises TODO dans le texte",
-    "viewer_config_open_link_confirmation_checkbox": "Demander confirmation avant d'ouvrir les liens",
+        "Converte emojis textuales in representationes graphicas",
+    "viewer_config_highlight_todos_checkbox": "Illustra TODOs",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "In textu TODOs signa illustra",
+    "viewer_config_open_link_confirmation_checkbox": "Postulat Confirmationem ad Aperiendum Nexus",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "Demander une confirmation avant d'ouvrir des liens",
+        "Quaere confirmationem ante apertionem nexus",
+    "viewer_config_save_resources_checkbox": "Serva imagines externas in disco automatice",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Automatice servat exemplaria imaginum externarum in disco ad usum sine nexu.",
 
     "ai_config_openai_api_label": "API OpenAI",
-    "ai_config_openai_api_url_input_placeholder_text": "URL de l'API",
-    "ai_config_openai_api_url_input_accessible_description": "URL de l'API OpenAI",
-    "ai_config_openai_api_key_input_placeholder_text": "Clé API",
-    "ai_config_openai_api_key_input_accessible_description": "Clé de l'API OpenAI",
-    "ai_config_openai_api_supported_models_label": "Modèles pris en charge",
-    "ai_config_ai_model_names_combo_placeholder_text": "Choisir un modèle",
-    "ai_config_ai_model_names_combo_accessible_description": "Modèles pris en charge à choisir",
-
-    "ai_config_base_label": "Paramètres de base",
-    "ai_config_base_system_prompt_label": "Invite de système",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Invite de système de base qui précède chaque demande",
+    "ai_config_openai_api_url_input_placeholder_text": "URL API",
+    "ai_config_openai_api_url_input_accessible_description": "URL API OpenAI",
+    "ai_config_openai_api_key_input_placeholder_text": "Clavis API",
+    "ai_config_openai_api_key_input_accessible_description": "Clavis API OpenAI",
+    "ai_config_openai_api_supported_models_label": "Modela sustenta",
+    "ai_config_ai_model_names_combo_placeholder_text": "Modelum elige",
+    "ai_config_ai_model_names_combo_accessible_description": "Modela sustenta ad eligendum",
+
+    "ai_config_base_label": "Parametri Principes",
+    "ai_config_base_system_prompt_label": "Systēma Monitum",
+    "ai_config_base_system_prompt_edit_placeholder_text": "Monitum systēmatis basis quod præcedit singulas postulationes",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "Invite de système de base qui précède chaque demande. Texte brut.",
-    "ai_config_base_response_max_tokens_label": "Nombre maximal de jetons de réponse",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Nombre maximal de jetons à recevoir en réponse",
+        "Monitum systēmatis basis quod præcedit singulas postulationes. Textus simpliciter.",
+    "ai_config_base_response_max_tokens_label": "Maxima Responsionis Signa",
+    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum signorum quæ in responsione accipiuntur",
 }
```

### Comparing `notolog-0.9.0b10/app/lexemes/fr/statusbar.py` & `notolog-0.9.0b11/app/lexemes/fr/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/fr/toolbar.py` & `notolog-0.9.0b11/app/lexemes/fr/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/ge/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/ge/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/common.py` & `notolog-0.9.0b11/app/lexemes/ge/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     "popup_about_title": "აპლიკაციის ინფორმაცია",
     "popup_about_app_name_description": "Markdown რედაქტორი",
 
     "popup_about_version": "ვერსია",
     "popup_about_license": "ლიცენზია",
     "popup_about_website": "ვებგვერდი",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "თარიღი",
 
     "update_helper_new_version_is_available": "აპლიკაციის ახალი ვერსია '{latest_version}' მისაწვდომია",
     "update_helper_latest_version_installed": "აპლიკაციის უახლესი ვერსია დაყენებულია",
 
     "network_connection_error_empty": "პასუხის ინფორმაციის მიღება ვერ ხერხდება",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/ge/main_menu.py` & `notolog-0.9.0b11/app/lexemes/ge/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/ge/settings_dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     "viewer_config_process_emojis_checkbox": "ტექსტური ემოჯის გრაფიკულად გარდაქმნა",
     "viewer_config_process_emojis_checkbox_accessible_description": "ტექსტური ემოჯების გრაფიკული წარმოჩენა",
     "viewer_config_highlight_todos_checkbox": "TODO-ების გამოყოფა",
     "viewer_config_highlight_todos_checkbox_accessible_description": "TODO ტეგების გამოყოფა ტექსტში",
     "viewer_config_open_link_confirmation_checkbox": "ბმულების გახსნის დასტური",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "ბმულების გახსნისას დასტურის მოთხოვნა",
+    "viewer_config_save_resources_checkbox": "გარე სურათების ავტომატური შენახვა დისკზე",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "გარე სურათების ასლების ავტომატურად შენახვა დისკზე ოფლაინ წვდომისთვის.",
 
     "ai_config_openai_api_label": "OpenAI API",
     "ai_config_openai_api_url_input_placeholder_text": "API URL",
     "ai_config_openai_api_url_input_accessible_description": "OpenAI API URL",
     "ai_config_openai_api_key_input_placeholder_text": "API გასაღები",
     "ai_config_openai_api_key_input_accessible_description": "OpenAI API გასაღები",
     "ai_config_openai_api_supported_models_label": "მხარდაჭერილი მოდელები",
```

### Comparing `notolog-0.9.0b10/app/lexemes/ge/statusbar.py` & `notolog-0.9.0b11/app/lexemes/ge/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ge/toolbar.py` & `notolog-0.9.0b11/app/lexemes/ge/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/it/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/it/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/common.py` & `notolog-0.9.0b11/app/lexemes/it/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Informazioni sull'Applicazione",
     "popup_about_app_name_description": "Editor Markdown",
 
     "popup_about_version": "Versione",
     "popup_about_license": "Licenza",
     "popup_about_website": "Sito Web",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Data",
 
     "update_helper_new_version_is_available": "Nuova versione '{latest_version}' dell'app disponibile",
     "update_helper_latest_version_installed": "L'ultima versione dell'app è installata",
 
     "network_connection_error_empty": "Impossibile ottenere informazioni sulla risposta",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/it/main_menu.py` & `notolog-0.9.0b11/app/lexemes/it/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/ja/settings_dialog.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,62 @@
-# Italian lexemes settings_dialog.py
+# Japanese lexemes settings_dialog.py
 lexemes = {
-    # Impostazioni
-    "window_title": "Impostazioni",
+    # 設定
+    "window_title": "設定",
 
-    "button_close": "Chiudi",
+    "button_close": "閉じる",
 
-    "tab_general": "Generale",
-    "tab_editor_config": "Editore",
-    "tab_viewer_config": "Visualizzatore",
-    "tab_ai_config": "Configurazione IA",
-
-    "general_app_config_label": "Configurazione dell'app",
-    "general_app_language_label": "Lingua",
-    "general_app_language_combo_placeholder_text": "Scegli una lingua",
-    "general_app_language_combo_accessible_description": "Lingua dell'interfaccia dell'app",
-    "general_app_theme_label": "Tema",
-    "general_app_theme_combo_placeholder_text": "Scegli un tema",
-    "general_app_theme_combo_accessible_description": "Tema dell'interfaccia dell'app",
-    "general_app_main_menu_label": "Menu Principale",
-    "general_app_main_menu_checkbox": "Mostra il menu principale",
-    "general_app_main_menu_checkbox_accessible_description": "Visualizza il menu a discesa principale dell'app",
-    "general_app_font_size_label": "Dimensione del carattere: {size}pt",
-    "general_app_font_size_slider_accessible_description": "Regola la dimensione del carattere globale dell'app",
+    "tab_general": "一般",
+    "tab_editor_config": "エディター",
+    "tab_viewer_config": "ビューア",
+    "tab_ai_config": "AI 設定",
+
+    "general_app_config_label": "アプリ設定",
+    "general_app_language_label": "言語",
+    "general_app_language_combo_placeholder_text": "言語を選択",
+    "general_app_language_combo_accessible_description": "アプリのインターフェース言語",
+    "general_app_theme_label": "テーマ",
+    "general_app_theme_combo_placeholder_text": "テーマを選択",
+    "general_app_theme_combo_accessible_description": "アプリのインターフェーステーマ",
+    "general_app_main_menu_label": "メインメニュー",
+    "general_app_main_menu_checkbox": "メインメニューを表示",
+    "general_app_main_menu_checkbox_accessible_description": "アプリのメインドロップダウンメニューを表示",
+    "general_app_font_size_label": "フォントサイズ：{size}pt",
+    "general_app_font_size_slider_accessible_description": "アプリの全体的なフォントサイズを調整する",
 
-    "general_statusbar_label": "Barra di Stato",
-    "general_statusbar_show_global_cursor_position_checkbox": "Mostra la Posizione Globale del Cursore",
+    "general_statusbar_label": "ステータスバー",
+    "general_statusbar_show_global_cursor_position_checkbox": "グローバルカーソル位置を表示",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "Visualizza la posizione globale del cursore nella barra di stato",
+        "ステータスバーにグローバルカーソル位置を表示する",
 
-    "editor_config_label": "Configurazione Editor",
-    "editor_config_show_line_numbers_checkbox": "Mostra Numeri di Riga",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "Visualizza i numeri di riga nell'editor",
-
-    "viewer_config_label": "Configurazione Visualizzatore",
-    "viewer_config_process_emojis_checkbox": "Converti Emoji di Testo in Grafica",
-    "viewer_config_process_emojis_checkbox_accessible_description":
-        "Converti le emoji di testo in rappresentazioni grafiche",
-    "viewer_config_highlight_todos_checkbox": "Evidenzia TODO",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "Evidenzia le etichette TODO nel testo",
-    "viewer_config_open_link_confirmation_checkbox": "Richiedi Conferma per Aprire i Link",
-    "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "Richiedi conferma prima di aprire i link",
-
-    "ai_config_openai_api_label": "API OpenAI",
-    "ai_config_openai_api_url_input_placeholder_text": "URL API",
-    "ai_config_openai_api_url_input_accessible_description": "URL dell'API OpenAI",
-    "ai_config_openai_api_key_input_placeholder_text": "Chiave API",
-    "ai_config_openai_api_key_input_accessible_description": "Chiave API di OpenAI",
-    "ai_config_openai_api_supported_models_label": "Modelli supportati",
-    "ai_config_ai_model_names_combo_placeholder_text": "Scegli modello",
-    "ai_config_ai_model_names_combo_accessible_description": "Modelli supportati da scegliere",
-
-    "ai_config_base_label": "Parametri Base",
-    "ai_config_base_system_prompt_label": "Prompt del Sistema",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Prompt di sistema base che precede ogni richiesta",
+    "editor_config_label": "エディタ設定",
+    "editor_config_show_line_numbers_checkbox": "行番号を表示",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "エディタ内で行番号を表示する",
+
+    "viewer_config_label": "ビューワ設定",
+    "viewer_config_process_emojis_checkbox": "テキスト絵文字をグラフィックに変換",
+    "viewer_config_process_emojis_checkbox_accessible_description": "テキスト絵文字をグラフィカルな表現に変換する",
+    "viewer_config_highlight_todos_checkbox": "TODOをハイライト",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "テキスト内のTODOタグを強調表示する",
+    "viewer_config_open_link_confirmation_checkbox": "リンク開く前に確認が必要",
+    "viewer_config_open_link_confirmation_checkbox_accessible_description": "リンクを開く前に確認を求める",
+    "viewer_config_save_resources_checkbox": "外部画像をディスクに自動保存",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "オフラインアクセスのために外部画像のコピーをディスクに自動保存します。",
+
+    "ai_config_openai_api_label": "OpenAI API",
+    "ai_config_openai_api_url_input_placeholder_text": "API URL",
+    "ai_config_openai_api_url_input_accessible_description": "OpenAI APIのURL",
+    "ai_config_openai_api_key_input_placeholder_text": "API キー",
+    "ai_config_openai_api_key_input_accessible_description": "OpenAI APIのキー",
+    "ai_config_openai_api_supported_models_label": "サポートされているモデル",
+    "ai_config_ai_model_names_combo_placeholder_text": "モデルを選択",
+    "ai_config_ai_model_names_combo_accessible_description": "選択可能なサポートされているモデル",
+
+    "ai_config_base_label": "基本パラメータ",
+    "ai_config_base_system_prompt_label": "システムプロンプト",
+    "ai_config_base_system_prompt_edit_placeholder_text": "各リクエストに先立つ基本システムプロンプト",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "Prompt di sistema base che precede ogni richiesta. Testo semplice.",
-    "ai_config_base_response_max_tokens_label": "Massimo di Token di Risposta",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Numero massimo di token da ricevere in risposta",
+        "各リクエストに先立つ基本システムプロンプト。プレーンテキスト。",
+    "ai_config_base_response_max_tokens_label": "応答の最大トークン数",
+    "ai_config_base_response_max_tokens_input_accessible_description": "応答で受け取る最大トークン数",
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `notolog-0.9.0b10/app/lexemes/it/statusbar.py` & `notolog-0.9.0b11/app/lexemes/it/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/it/toolbar.py` & `notolog-0.9.0b11/app/lexemes/it/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/ai_assistant.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 931 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 a303 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 a303 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000d 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 9c0c 5a00 640d 5300  d.d.d.d...Z.d.S.
 00000050: 290e 7518 0000 0041 4920 e381 b8e3 81ae  ).u....AI ......
 00000060: e383 aae3 82af e382 a8e3 82b9 e383 8875  ...............u
 00000070: 0f00 0000 e383 aae3 82af e382 a8e3 82b9  ................
@@ -52,13 +52,13 @@
 00000330: 5f61 6e73 7765 72da 1964 6961 6c6f 675f  _answer..dialog_
 00000340: 7573 6167 655f 746f 6b65 6e73 5f74 6f74  usage_tokens_tot
 00000350: 616c da1a 6469 616c 6f67 5f62 7574 746f  al..dialog_butto
 00000360: 6e5f 7365 6e64 5f72 6571 7565 7374 4e29  n_send_requestN)
 00000370: 01da 076c 6578 656d 6573 a900 720d 0000  ...lexemes..r...
 00000380: 0072 0d00 0000 fa49 2f55 7365 7273 2f76  .r.....I/Users/v
 00000390: 6164 696b 7573 2f50 7963 6861 726d 5072  adikus/PycharmPr
-000003a0: 6f6a 6563 7473 2f6e 6f74 6f6c 6f67 2f6e  ojects/notolog/n
-000003b0: 6f74 6f6c 6f67 2f6c 6578 656d 6573 2f6a  otolog/lexemes/j
+000003a0: 6f6a 6563 7473 2f6e 6f74 6f6c 6f67 2d64  ojects/notolog-d
+000003b0: 6576 2f61 7070 2f6c 6578 656d 6573 2f6a  ev/app/lexemes/j
 000003c0: 612f 6169 5f61 7373 6973 7461 6e74 2e70  a/ai_assistant.p
 000003d0: 79da 083c 6d6f 6475 6c65 3e04 0000 0073  y..<module>....s
 000003e0: 1800 0000 0201 0201 0201 0201 0201 0202  ................
 000003f0: 0201 0201 0201 0201 0201 02f2            ............
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/color_picker_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 8464 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 1021 0000  a.......'..f.!..
+00000000: 610d 0d0a 0000 0000 020f 3066 1021 0000  a.........0f.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 008f 0000 0040 0000 0073 2601 0000 6400  .....@...s&...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
@@ -500,16 +500,16 @@
 00001f30: 725f 7069 636b 6572 5f63 6f6c 6f72 5f77  r_picker_color_w
 00001f40: 6869 7465 736d 6f6b 655a 1e63 6f6c 6f72  hitesmokeZ.color
 00001f50: 5f70 6963 6b65 725f 636f 6c6f 725f 7965  _picker_color_ye
 00001f60: 6c6c 6f77 6772 6565 6e4e 2901 da07 6c65  llowgreenN)...le
 00001f70: 7865 6d65 73a9 0072 0300 0000 7203 0000  xemes..r....r...
 00001f80: 00fa 502f 5573 6572 732f 7661 6469 6b75  ..P/Users/vadiku
 00001f90: 732f 5079 6368 6172 6d50 726f 6a65 6374  s/PycharmProject
-00001fa0: 732f 6e6f 746f 6c6f 672f 6e6f 746f 6c6f  s/notolog/notolo
-00001fb0: 672f 6c65 7865 6d65 732f 6a61 2f63 6f6c  g/lexemes/ja/col
+00001fa0: 732f 6e6f 746f 6c6f 672d 6465 762f 6170  s/notolog-dev/ap
+00001fb0: 702f 6c65 7865 6d65 732f 6a61 2f63 6f6c  p/lexemes/ja/col
 00001fc0: 6f72 5f70 6963 6b65 725f 6469 616c 6f67  or_picker_dialog
 00001fd0: 2e70 79da 083c 6d6f 6475 6c65 3e03 0000  .py..<module>...
 00001fe0: 0073 1e01 0000 0202 0201 0201 0201 0201  .s..............
 00001ff0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00002000: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00002010: 0201 0201 0201 0201 0201 0201 0201 0201  ................
 00002020: 0201 0201 0201 0201 0201 0201 0201 0201  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/common.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/common.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 7209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,426 +1,428 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 291c 0000  a.......'..f)...
+00000000: 610d 0d0a 0000 0000 42a9 3566 491c 0000  a.......B.5fI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0054 0000 0040 0000 0073 b000 0000 6400  .T...@...s....d.
+00000020: 0055 0000 0040 0000 0073 b200 0000 6400  .U...@...s....d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6403 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 641e 641f 6423 6424 6425  d d!d"d.d.d#d$d%
 00000080: 6426 6427 6428 6429 642a 642b 642c 642b  d&d'd(d)d*d+d,d+
 00000090: 642d 642e 6424 642e 6426 6429 642a 642f  d-d.d$d.d&d)d*d/
 000000a0: 6430 642a 6431 6432 6433 6434 6435 6436  d0d*d1d2d3d4d5d6
 000000b0: 6437 6438 6439 643a 643b 643c 643d 643e  d7d8d9d:d;d<d=d>
 000000c0: 643f 6440 6441 6442 6443 6444 6445 6446  d?d@dAdBdCdDdEdF
-000000d0: 6447 6448 6449 9c53 5a00 644a 5300 294b  dGdHdI.SZ.dJS.)K
-000000e0: 7514 0000 004e 6f74 6f6c 6f67 20e3 82a8  u....Notolog ...
-000000f0: e383 87e3 82a3 e382 bf7a 197b 6170 705f  .........z.{app_
-00000100: 7469 746c 657d 202d 207b 7375 625f 7469  title} - {sub_ti
-00000110: 746c 657d 7527 0000 00e3 8395 e382 a1e3  tle}u'..........
-00000120: 82a4 e383 abe3 8395 e382 a3e3 83ab e382  ................
-00000130: bfe3 8395 e382 a3e3 83bc e383 abe3 8389  ................
-00000140: 750f 0000 00e5 908d e589 8de3 8292 e5a4  u...............
-00000150: 89e6 9bb4 7506 0000 00e5 898a e999 a475  ....u..........u
-00000160: 0f00 0000 e5ae 8ce5 85a8 e381 abe5 898a  ................
-00000170: e999 a475 0600 0000 e5be a9e5 8583 7518  ...u..........u.
-00000180: 0000 00e3 8395 e382 a1e3 82a4 e383 abe5  ................
-00000190: 908d e381 aee5 a489 e69b b475 2100 0000  ...........u!...
-000001a0: e696 b0e3 8197 e381 84e3 8395 e382 a1e3  ................
-000001b0: 82a4 e383 abe5 908d e382 92e5 85a5 e58a  ................
-000001c0: 9b75 3600 0000 e590 8ce5 908d e381 aee3  .u6.............
-000001d0: 8395 e382 a1e3 82a4 e383 abe3 818c e381  ................
-000001e0: 99e3 81a7 e381 abe5 ad98 e59c a8e3 8197  ................
-000001f0: e381 a6e3 8184 e381 bee3 8199 7515 0000  ............u...
-00000200: 00e3 8395 e382 a1e3 82a4 e383 abe3 81ae  ................
-00000210: e589 8ae9 99a4 7533 0000 00e3 8395 e382  ......u3........
-00000220: a1e3 82a4 e383 ab20 227b 6669 6c65 5f6e  ....... "{file_n
-00000230: 616d 657d 2220 e382 92e5 898a e999 a4e3  ame}" ..........
-00000240: 8197 e381 bee3 8199 e381 8bef bc9f 751e  ..............u.
-00000250: 0000 00e3 8395 e382 a1e3 82a4 e383 abe3  ................
-00000260: 8292 e5ae 8ce5 85a8 e381 abe5 898a e999  ................
-00000270: a475 3e00 0000 e383 95e3 82a1 e382 a4e3  .u>.............
-00000280: 83ab e380 8c7b 6669 6c65 5f6e 616d 657d  .....{file_name}
-00000290: e380 8de3 8292 e5ae 8ce5 85a8 e381 abe5  ................
-000002a0: 898a e999 a4e3 8197 e381 bee3 8199 e381  ................
-000002b0: 8bef bc9f 754e 0000 00e3 8395 e382 a1e3  ....uN..........
-000002c0: 82a4 e383 abe3 8292 e589 8ae9 99a4 e381  ................
-000002d0: a7e3 818d e381 bee3 819b e382 93e3 81a7  ................
-000002e0: e381 97e3 819f e380 82e3 82a8 e383 a9e3  ................
-000002f0: 83bc e381 8ce7 99ba e794 9fe3 8197 e381  ................
-00000300: bee3 8197 e381 9f75 2400 0000 e383 95e3  .......u$.......
-00000310: 82a1 e382 a4e3 83ab e381 8ce8 a68b e381  ................
-00000320: a4e3 818b e382 8ae3 81be e381 9be3 8293  ................
-00000330: 7515 0000 00e3 8395 e382 a1e3 82a4 e383  u...............
-00000340: abe3 8292 e5be a9e5 8583 7533 0000 00e3  ..........u3....
-00000350: 8395 e382 a1e3 82a4 e383 ab20 227b 6669  ........... "{fi
-00000360: 6c65 5f6e 616d 657d 2220 e382 92e5 bea9  le_name}" ......
-00000370: e585 83e3 8197 e381 bee3 8199 e381 8bef  ................
-00000380: bc9f 754e 0000 00e3 8395 e382 a1e3 82a4  ..uN............
-00000390: e383 abe3 8292 e5be a9e5 8583 e381 a7e3  ................
-000003a0: 818d e381 bee3 819b e382 93e3 81a7 e381  ................
-000003b0: 97e3 819f e380 82e3 82a8 e383 a9e3 83bc  ................
-000003c0: e381 8ce7 99ba e794 9fe3 8197 e381 bee3  ................
-000003d0: 8197 e381 9f75 4500 0000 7b66 696c 655f  .....uE...{file_
-000003e0: 6e61 6d65 7d20 e381 a8e3 8184 e381 86e5  name} ..........
-000003f0: 908d e589 8de3 81ae e383 95e3 82a1 e382  ................
-00000400: a4e3 83ab e381 8ce3 8199 e381 a7e3 81ab  ................
-00000410: e5ad 98e5 9ca8 e381 97e3 81be e381 9975  ...............u
-00000420: 0f00 0000 e383 a1e3 8383 e382 bbe3 83bc  ................
-00000430: e382 b875 0900 0000 e996 89e3 8198 e382  ...u............
-00000440: 8b75 1b00 0000 e696 b0e3 8197 e381 84e3  .u..............
-00000450: 8389 e382 ade3 83a5 e383 a1e3 83b3 e383  ................
-00000460: 8875 1500 0000 e383 95e3 82a1 e382 a4e3  .u..............
-00000470: 83ab e382 92e9 968b e381 8f75 1500 0000  ...........u....
-00000480: e383 95e3 82a1 e382 a4e3 83ab e382 92e4  ................
-00000490: bf9d e5ad 9875 1b00 0000 e7a9 bae3 81ae  .....u..........
-000004a0: e383 95e3 82a1 e382 a4e3 83ab e382 92e4  ................
-000004b0: bf9d e5ad 9875 3300 0000 e586 85e5 aeb9  .....u3.........
-000004c0: e381 8ce7 a9ba e381 aee3 8395 e382 a1e3  ................
-000004d0: 82a4 e383 abe3 8292 e4bf 9de5 ad98 e381  ................
-000004e0: 97e3 81be e381 99e3 818b efbc 9f75 1800  .............u..
-000004f0: 0000 e383 95e3 82a1 e382 a4e3 83ab e381  ................
-00000500: aee6 9a97 e58f b7e5 8c96 7536 0000 00e3  ..........u6....
-00000510: 8395 e382 a1e3 82a4 e383 ab20 227b 6669  ........... "{fi
-00000520: 6c65 5f6e 616d 657d 2220 e382 92e6 9a97  le_name}" ......
-00000530: e58f b7e5 8c96 e381 97e3 81be e381 99e3  ................
-00000540: 818b efbc 9f75 3600 0000 e383 95e3 82a1  .....u6.........
-00000550: e382 a4e3 83ab e381 afe3 8199 e381 a7e3  ................
-00000560: 81ab e69a 97e5 8fb7 e58c 96e3 8195 e382  ................
-00000570: 8ce3 81a6 e381 84e3 81be e381 99ef bc81  ................
-00000580: 7521 0000 00e6 97a2 e5ad 98e3 81ae e383  u!..............
-00000590: 95e3 82a1 e382 a4e3 83ab e382 92e4 b88a  ................
-000005a0: e69b b8e3 818d 753f 0000 00e6 97a2 e5ad  ......u?........
-000005b0: 98e3 81ae e383 95e3 82a1 e382 a4e3 83ab  ................
-000005c0: 2022 7b66 696c 655f 7061 7468 7d22 20e3   "{file_path}" .
-000005d0: 8292 e4b8 8ae6 9bb8 e381 8de3 8197 e381  ................
-000005e0: bee3 8199 e381 8bef bc9f 7515 0000 00e3  ..........u.....
-000005f0: 8395 e382 a1e3 82a4 e383 abe3 81ae e5be  ................
-00000600: a9e5 8fb7 7533 0000 00e3 8395 e382 a1e3  ....u3..........
-00000610: 82a4 e383 ab20 227b 6669 6c65 5f6e 616d  ..... "{file_nam
-00000620: 657d 2220 e382 92e5 bea9 e58f b7e3 8197  e}" ............
-00000630: e381 bee3 8199 e381 8bef bc9f 7530 0000  ............u0..
-00000640: 00e3 8395 e382 a1e3 82a4 e383 abe3 81af  ................
-00000650: e69a 97e5 8fb7 e58c 96e3 8195 e382 8ce3  ................
-00000660: 81a6 e381 84e3 81be e381 9be3 8293 efbc  ................
-00000670: 8175 1800 0000 e696 b0e3 8197 e381 84e3  .u..............
-00000680: 8391 e382 b9e3 83af e383 bce3 8389 7512  ..............u.
-00000690: 0000 00e3 8391 e382 b9e3 83af e383 bce3  ................
-000006a0: 8389 efbc 9a75 2100 0000 e696 b0e3 8197  .....u!.........
-000006b0: e381 84e3 8391 e382 b9e3 83af e383 bce3  ................
-000006c0: 8389 e382 92e5 85a5 e58a 9b75 0c00 0000  ...........u....
-000006d0: e383 92e3 83b3 e383 88ef bc9a 75e3 0000  ............u...
-000006e0: 00e3 8392 e383 b3e3 8388 e381 afe6 9a97  ................
-000006f0: e58f b7e5 8c96 e381 95e3 828c e381 9ae3  ................
-00000700: 81ab e383 95e3 82a1 e382 a4e3 83ab e381  ................
-00000710: 8be3 8289 e8aa ade3 81bf e58f 96e3 828b  ................
-00000720: e381 93e3 81a8 e381 8ce3 81a7 e381 8de3  ................
-00000730: 81be e381 99ef bc81 0ae8 aa95 e794 9fe6  ................
-00000740: 97a5 e381 aae3 81a9 e7b0 a1e5 8d98 e381  ................
-00000750: abe6 8ea8 e6b8 ace3 81a7 e381 8de3 828b  ................
-00000760: e383 92e3 83b3 e383 88e3 81af e4bd bfe7  ................
-00000770: 94a8 e381 97e3 81aa e381 84e3 81a7 e381  ................
-00000780: 8fe3 81a0 e381 95e3 8184 e380 820a e996  ................
-00000790: a2e9 80a3 e680 a7e3 81ae e4bd 8ee3 8184  ................
-000007a0: e58f 82e7 85a7 e382 92e4 bdbf e794 a8e3  ................
-000007b0: 8197 e381 a6e3 818f e381 a0e3 8195 e381  ................
-000007c0: 84e3 8082 7527 0000 00e3 8392 e383 b3e3  ....u'..........
-000007d0: 8388 e382 92e5 85a5 e58a 9bef bc88 e382  ................
-000007e0: aae3 8397 e382 b7e3 83a7 e383 b3ef bc89  ................
-000007f0: 5a02 4f4b 750f 0000 00e3 82ad e383 a3e3  Z.OKu...........
-00000800: 83b3 e382 bbe3 83ab 7506 0000 00e8 ada6  ........u.......
-00000810: e591 8a75 2d00 0000 e383 91e3 82b9 e383  ...u-...........
-00000820: afe3 83bc e383 89e6 ac84 e381 afe7 a9ba  ................
-00000830: e381 abe3 81a7 e381 8de3 81be e381 9be3  ................
-00000840: 8293 efbc 8175 3f00 0000 e383 92e3 83b3  .....u?.........
-00000850: e383 88e6 ac84 e381 8ce9 95b7 e381 99e3  ................
-00000860: 818e e381 bee3 8199 e380 82e6 9c80 e5a4  ................
-00000870: a77b 7379 6d62 6f6c 737d e696 87e5 ad97  .{symbols}......
-00000880: e381 a7e3 8199 efbc 8175 1800 0000 e383  .........u......
-00000890: 91e3 82b9 e383 afe3 83bc e383 89e3 8292  ................
-000008a0: e585 a5e5 8a9b 7527 0000 00e6 9a97 e58f  ......u'........
-000008b0: b7e5 8c96 e383 91e3 82b9 e383 afe3 83bc  ................
-000008c0: e383 89e3 81ae e383 aae3 82bb e383 83e3  ................
-000008d0: 8388 753f 0000 00e7 8fbe e59c a8e3 81ae  ..u?............
-000008e0: e69a 97e5 8fb7 e58c 96e3 8391 e382 b9e3  ................
-000008f0: 83af e383 bce3 8389 e382 92e3 83aa e382  ................
-00000900: bbe3 8383 e383 88e3 8197 e381 bee3 8199  ................
-00000910: e381 8bef bc9f 7506 0000 00e3 81af e381  ......u.........
-00000920: 8475 0900 0000 e383 aae3 83b3 e382 af75  .u.............u
-00000930: 3600 0000 e383 aae3 83b3 e382 af20 227b  6............ "{
-00000940: 7572 6c7d 2220 e382 92e3 8396 e383 a9e3  url}" ..........
-00000950: 82a6 e382 b6e3 81a7 e996 8be3 818d e381  ................
-00000960: bee3 8199 e381 8bef bc9f 7530 0000 00e6  ..........u0....
-00000970: 9a97 e58f b7e5 8c96 e383 91e3 82b9 e383  ................
-00000980: afe3 83bc e383 89e3 818c e4b8 80e8 87b4  ................
-00000990: e381 97e3 81be e381 9be3 8293 efbc 8175  ...............u
-000009a0: 3600 0000 e69a 97e5 8fb7 e58c 96e3 8391  6...............
-000009b0: e382 b9e3 83af e383 bce3 8389 e381 8ce6  ................
-000009c0: ada3 e381 97e3 818f e381 82e3 828a e381  ................
-000009d0: bee3 819b e382 93ef bc81 7527 0000 00e3  ..........u'....
-000009e0: 8395 e382 a1e3 82a4 e383 abe3 8292 e8aa  ................
-000009f0: ade3 81bf e8be bce3 8281 e381 bee3 819b  ................
-00000a00: e382 93e3 8082 754e 0000 00e3 8395 e382  ......uN........
-00000a10: a1e3 82a4 e383 abe3 8292 e4bf 9de5 ad98  ................
-00000a20: e381 a7e3 818d e381 bee3 819b e382 93e3  ................
-00000a30: 81a7 e381 97e3 819f e380 82e3 82a8 e383  ................
-00000a40: a9e3 83bc e381 8ce7 99ba e794 9fe3 8197  ................
-00000a50: e381 bee3 8197 e381 9f75 0f00 0000 e8a9  .........u......
-00000a60: b3e7 b4b0 e683 85e5 a0b1 2e2e 2e75 5a00  .............uZ.
-00000a70: 0000 e383 95e3 82a9 e383 bce3 839e e383  ................
-00000a80: 83e3 8388 e381 95e3 828c e381 9fe3 8386  ................
-00000a90: e382 ade3 82b9 e383 88e3 818c e382 afe3  ................
-00000aa0: 83aa e383 83e3 8397 e383 9ce3 83bc e383  ................
-00000ab0: 89e3 81ab e382 b3e3 8394 e383 bce3 8195  ................
-00000ac0: e382 8ce3 81be e381 97e3 819f 750f 0000  ............u...
-00000ad0: 00e3 82a2 e383 97e3 83aa e683 85e5 a0b1  ................
-00000ae0: 7515 0000 004d 6172 6b64 6f77 6e20 e382  u....Markdown ..
-00000af0: a8e3 8387 e382 a3e3 82bf 750f 0000 00e3  ..........u.....
-00000b00: 8390 e383 bce3 82b8 e383 a7e3 83b3 750f  ..............u.
-00000b10: 0000 00e3 83a9 e382 a4e3 82bb e383 b3e3  ................
-00000b20: 82b9 7512 0000 00e3 82a6 e382 a7e3 8396  ..u.............
-00000b30: e382 b5e3 82a4 e383 885a 0647 6974 4875  .........Z.GitHu
-00000b40: 6275 0600 0000 e697 a5e4 bb98 754d 0000  bu..........uM..
-00000b50: 00e3 82a2 e383 97e3 83aa e381 aee6 96b0  ................
-00000b60: e381 97e3 8184 e383 90e3 83bc e382 b8e3  ................
-00000b70: 83a7 e383 b320 277b 6c61 7465 7374 5f76  ..... '{latest_v
-00000b80: 6572 7369 6f6e 7d27 20e3 818c e588 a9e7  ersion}' .......
-00000b90: 94a8 e58f afe8 83bd e381 a7e3 8199 7548  ..............uH
-00000ba0: 0000 00e3 82a2 e383 97e3 83aa e381 aee6  ................
-00000bb0: 9c80 e696 b0e3 8390 e383 bce3 82b8 e383  ................
-00000bc0: a7e3 83b3 e381 8ce3 82a4 e383 b3e3 82b9  ................
-00000bd0: e383 88e3 83bc e383 abe3 8195 e382 8ce3  ................
-00000be0: 81a6 e381 84e3 81be e381 9975 2400 0000  ...........u$...
-00000bf0: e5bf 9ce7 ad94 e683 85e5 a0b1 e382 92e5  ................
-00000c00: 8f96 e5be 97e3 81a7 e381 8de3 81be e381  ................
-00000c10: 9be3 8293 7575 0000 00e3 839b e382 b9e3  ....uu..........
-00000c20: 8388 e381 8ce8 a68b e381 a4e3 818b e382  ................
-00000c30: 8ae3 81be e381 9be3 8293 e380 82e3 82a4  ................
-00000c40: e383 b3e3 82bf e383 bce3 838d e383 83e3  ................
-00000c50: 8388 e68e a5e7 b69a e381 bee3 819f e381  ................
-00000c60: af44 4e53 e381 abe5 958f e9a1 8ce3 818c  .DNS............
-00000c70: e381 82e3 828b e381 8be3 8282 e381 97e3  ................
-00000c80: 828c e381 bee3 819b e382 93e3 8082 758a  ..............u.
-00000c90: 0000 00e6 8ea5 e7b6 9ae3 818c e68b 92e5  ................
-00000ca0: 90a6 e381 95e3 828c e381 bee3 8197 e381  ................
-00000cb0: 9fe3 8082 e382 b5e3 83bc e383 90e3 83bc  ................
-00000cc0: e381 8ce3 8380 e382 a6e3 83b3 e381 97e3  ................
-00000cd0: 81a6 e381 84e3 828b e381 8be3 8081 e383  ................
-00000ce0: 8de3 8383 e383 88e3 83af e383 bce3 82af  ................
-00000cf0: e381 abe5 958f e9a1 8ce3 818c e381 82e3  ................
-00000d00: 828b e58f afe8 83bd e680 a7e3 818c e381  ................
-00000d10: 82e3 828a e381 bee3 8199 e380 8275 6600  .............uf.
-00000d20: 0000 e68e a5e7 b69a e381 8ce3 82bf e382  ................
-00000d30: a4e3 83a0 e382 a2e3 82a6 e383 88e3 8197  ................
-00000d40: e381 bee3 8197 e381 9fe3 8082 e383 8de3  ................
-00000d50: 8383 e383 88e3 83af e383 bce3 82af e381  ................
-00000d60: abe5 958f e9a1 8ce3 818c e381 82e3 828b  ................
-00000d70: e381 8be3 8282 e381 97e3 828c e381 bee3  ................
-00000d80: 819b e382 93e3 8082 755d 0000 00e6 8ea5  ........u]......
-00000d90: e7b6 9a34 3034 e382 a8e3 83a9 e383 bce3  ...404..........
-00000da0: 8082 e8a6 81e6 b182 e381 95e3 828c e381  ................
-00000db0: 9fe3 839a e383 bce3 82b8 e381 bee3 819f  ................
-00000dc0: e381 afe3 83aa e382 bde3 83bc e382 b9e3  ................
-00000dd0: 818c e8a6 8be3 81a4 e381 8be3 828a e381  ................
-00000de0: bee3 819b e382 93e3 8082 754c 0000 00e3  ..........uL....
-00000df0: 82b9 e383 86e3 83bc e382 bfe3 82b9 e382  ................
-00000e00: b3e3 83bc e383 897b 7374 6174 7573 5f63  .......{status_c
-00000e10: 6f64 657d e381 a7e3 83aa e382 afe3 82a8  ode}............
-00000e20: e382 b9e3 8388 e381 8ce5 a4b1 e695 97e3  ................
-00000e30: 8197 e381 bee3 8197 e381 9f29 53da 0961  ...........)S..a
-00000e40: 7070 5f74 6974 6c65 da12 6170 705f 7469  pp_title..app_ti
-00000e50: 746c 655f 7769 7468 5f73 7562 da1b 7472  tle_with_sub..tr
-00000e60: 6565 5f66 696c 7465 725f 6163 6365 7373  ee_filter_access
-00000e70: 6962 6c65 5f64 6573 63da 126d 656e 755f  ible_desc..menu_
-00000e80: 6163 7469 6f6e 5f72 656e 616d 65da 126d  action_rename..m
-00000e90: 656e 755f 6163 7469 6f6e 5f64 656c 6574  enu_action_delet
-00000ea0: 65da 1d6d 656e 755f 6163 7469 6f6e 5f64  e..menu_action_d
-00000eb0: 656c 6574 655f 636f 6d70 6c65 7465 6c79  elete_completely
-00000ec0: da13 6d65 6e75 5f61 6374 696f 6e5f 7265  ..menu_action_re
-00000ed0: 7374 6f72 65da 1864 6961 6c6f 675f 6669  store..dialog_fi
-00000ee0: 6c65 5f72 656e 616d 655f 7469 746c 65da  le_rename_title.
-00000ef0: 1e64 6961 6c6f 675f 6669 6c65 5f72 656e  .dialog_file_ren
-00000f00: 616d 655f 6669 656c 645f 6c61 6265 6cda  ame_field_label.
-00000f10: 1c64 6961 6c6f 675f 6669 6c65 5f72 656e  .dialog_file_ren
-00000f20: 616d 655f 6275 7474 6f6e 5f6f 6bda 2164  ame_button_ok.!d
-00000f30: 6961 6c6f 675f 6669 6c65 5f72 656e 616d  ialog_file_renam
-00000f40: 655f 7761 726e 696e 675f 6578 6973 7473  e_warning_exists
-00000f50: da18 6469 616c 6f67 5f66 696c 655f 6465  ..dialog_file_de
-00000f60: 6c65 7465 5f74 6974 6c65 da17 6469 616c  lete_title..dial
-00000f70: 6f67 5f66 696c 655f 6465 6c65 7465 5f74  og_file_delete_t
-00000f80: 6578 74da 2364 6961 6c6f 675f 6669 6c65  ext.#dialog_file
-00000f90: 5f64 656c 6574 655f 636f 6d70 6c65 7465  _delete_complete
-00000fa0: 6c79 5f74 6974 6c65 da22 6469 616c 6f67  ly_title."dialog
-00000fb0: 5f66 696c 655f 6465 6c65 7465 5f63 6f6d  _file_delete_com
-00000fc0: 706c 6574 656c 795f 7465 7874 da18 6469  pletely_text..di
-00000fd0: 616c 6f67 5f66 696c 655f 6465 6c65 7465  alog_file_delete
-00000fe0: 5f65 7272 6f72 da22 6469 616c 6f67 5f66  _error."dialog_f
-00000ff0: 696c 655f 6465 6c65 7465 5f65 7272 6f72  ile_delete_error
-00001000: 5f6e 6f74 5f66 6f75 6e64 da19 6469 616c  _not_found..dial
-00001010: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
-00001020: 7469 746c 65da 1864 6961 6c6f 675f 6669  title..dialog_fi
-00001030: 6c65 5f72 6573 746f 7265 5f74 6578 745a  le_restore_textZ
-00001040: 1964 6961 6c6f 675f 6669 6c65 5f72 6573  .dialog_file_res
-00001050: 746f 7265 5f65 7272 6f72 da22 6469 616c  tore_error."dial
-00001060: 6f67 5f66 696c 655f 7265 7374 6f72 655f  og_file_restore_
-00001070: 7761 726e 696e 675f 6578 6973 7473 da18  warning_exists..
-00001080: 6469 616c 6f67 5f6d 6573 7361 6765 5f62  dialog_message_b
-00001090: 6f78 5f74 6974 6c65 da1c 6469 616c 6f67  ox_title..dialog
-000010a0: 5f6d 6573 7361 6765 5f62 6f78 5f62 7574  _message_box_but
-000010b0: 746f 6e5f 6f6b da28 6163 7469 6f6e 5f6e  ton_ok.(action_n
-000010c0: 6577 5f66 696c 655f 6669 7273 745f 6c69  ew_file_first_li
-000010d0: 6e65 5f74 656d 706c 6174 655f 7465 7874  ne_template_text
-000010e0: da1f 6163 7469 6f6e 5f6f 7065 6e5f 6669  ..action_open_fi
-000010f0: 6c65 5f64 6961 6c6f 675f 6361 7074 696f  le_dialog_captio
-00001100: 6eda 2261 6374 696f 6e5f 7361 7665 5f61  n."action_save_a
-00001110: 735f 6669 6c65 5f64 6961 6c6f 675f 6361  s_file_dialog_ca
-00001120: 7074 696f 6eda 1c64 6961 6c6f 675f 7361  ption..dialog_sa
-00001130: 7665 5f65 6d70 7479 5f66 696c 655f 7469  ve_empty_file_ti
-00001140: 746c 65da 1b64 6961 6c6f 675f 7361 7665  tle..dialog_save
-00001150: 5f65 6d70 7479 5f66 696c 655f 7465 7874  _empty_file_text
-00001160: da19 6469 616c 6f67 5f65 6e63 7279 7074  ..dialog_encrypt
-00001170: 5f66 696c 655f 7469 746c 65da 1864 6961  _file_title..dia
-00001180: 6c6f 675f 656e 6372 7970 745f 6669 6c65  log_encrypt_file
-00001190: 5f74 6578 74da 2e65 6e63 7279 7074 5f66  _text..encrypt_f
-000011a0: 696c 655f 7761 726e 696e 675f 6669 6c65  ile_warning_file
-000011b0: 5f69 735f 616c 7265 6164 795f 656e 6372  _is_already_encr
-000011c0: 7970 7465 64da 2a64 6961 6c6f 675f 656e  ypted.*dialog_en
-000011d0: 6372 7970 745f 6669 6c65 5f72 6577 7269  crypt_file_rewri
-000011e0: 7465 5f65 7869 7374 696e 675f 7469 746c  te_existing_titl
-000011f0: 65da 2964 6961 6c6f 675f 656e 6372 7970  e.)dialog_encryp
-00001200: 745f 6669 6c65 5f72 6577 7269 7465 5f65  t_file_rewrite_e
-00001210: 7869 7374 696e 675f 7465 7874 da19 6469  xisting_text..di
-00001220: 616c 6f67 5f64 6563 7279 7074 5f66 696c  alog_decrypt_fil
-00001230: 655f 7469 746c 65da 1864 6961 6c6f 675f  e_title..dialog_
-00001240: 6465 6372 7970 745f 6669 6c65 5f74 6578  decrypt_file_tex
-00001250: 74da 2a64 6563 7279 7074 5f66 696c 655f  t.*decrypt_file_
-00001260: 7761 726e 696e 675f 6669 6c65 5f69 735f  warning_file_is_
-00001270: 6e6f 745f 656e 6372 7970 7465 64da 2a64  not_encrypted.*d
-00001280: 6961 6c6f 675f 6465 6372 7970 745f 6669  ialog_decrypt_fi
-00001290: 6c65 5f72 6577 7269 7465 5f65 7869 7374  le_rewrite_exist
-000012a0: 696e 675f 7469 746c 65da 2964 6961 6c6f  ing_title.)dialo
-000012b0: 675f 6465 6372 7970 745f 6669 6c65 5f72  g_decrypt_file_r
-000012c0: 6577 7269 7465 5f65 7869 7374 696e 675f  ewrite_existing_
-000012d0: 7465 7874 da21 6469 616c 6f67 5f65 6e63  text.!dialog_enc
-000012e0: 7279 7074 5f6e 6577 5f70 6173 7377 6f72  rypt_new_passwor
-000012f0: 645f 7469 746c 65da 2164 6961 6c6f 675f  d_title.!dialog_
-00001300: 656e 6372 7970 745f 6e65 775f 7061 7373  encrypt_new_pass
-00001310: 776f 7264 5f6c 6162 656c da32 6469 616c  word_label.2dial
-00001320: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
-00001330: 6173 7377 6f72 645f 696e 7075 745f 706c  assword_input_pl
-00001340: 6163 6568 6f6c 6465 725f 7465 7874 da26  aceholder_text.&
-00001350: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
-00001360: 6577 5f70 6173 7377 6f72 645f 6869 6e74  ew_password_hint
-00001370: 5f6c 6162 656c da32 6469 616c 6f67 5f65  _label.2dialog_e
-00001380: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-00001390: 6f72 645f 6869 6e74 5f6c 6162 656c 5f64  ord_hint_label_d
-000013a0: 6573 6372 6970 7469 6f6e da37 6469 616c  escription.7dial
-000013b0: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
-000013c0: 6173 7377 6f72 645f 6869 6e74 5f69 6e70  assword_hint_inp
-000013d0: 7574 5f70 6c61 6365 686f 6c64 6572 5f74  ut_placeholder_t
-000013e0: 6578 74da 2564 6961 6c6f 675f 656e 6372  ext.%dialog_encr
-000013f0: 7970 745f 6e65 775f 7061 7373 776f 7264  ypt_new_password
-00001400: 5f62 7574 746f 6e5f 6f6b da29 6469 616c  _button_ok.)dial
-00001410: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
-00001420: 6173 7377 6f72 645f 6275 7474 6f6e 5f63  assword_button_c
-00001430: 616e 6365 6cda 2f64 6961 6c6f 675f 656e  ancel./dialog_en
-00001440: 6372 7970 745f 6e65 775f 7061 7373 776f  crypt_new_passwo
-00001450: 7264 5f77 6172 6e69 6e67 5f65 6d70 7479  rd_warning_empty
-00001460: 5f74 6974 6c65 da2e 6469 616c 6f67 5f65  _title..dialog_e
-00001470: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-00001480: 6f72 645f 7761 726e 696e 675f 656d 7074  ord_warning_empt
-00001490: 795f 7465 7874 da32 6469 616c 6f67 5f65  y_text.2dialog_e
-000014a0: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
-000014b0: 6f72 645f 7761 726e 696e 675f 746f 6f5f  ord_warning_too_
-000014c0: 6c6f 6e67 5f74 6974 6c65 da31 6469 616c  long_title.1dial
-000014d0: 6f67 5f65 6e63 7279 7074 5f6e 6577 5f70  og_encrypt_new_p
-000014e0: 6173 7377 6f72 645f 7761 726e 696e 675f  assword_warning_
-000014f0: 746f 6f5f 6c6f 6e67 5f74 6578 74da 1d64  too_long_text..d
-00001500: 6961 6c6f 675f 656e 6372 7970 745f 7061  ialog_encrypt_pa
-00001510: 7373 776f 7264 5f74 6974 6c65 da1d 6469  ssword_title..di
-00001520: 616c 6f67 5f65 6e63 7279 7074 5f70 6173  alog_encrypt_pas
-00001530: 7377 6f72 645f 6c61 6265 6cda 2e64 6961  sword_label..dia
-00001540: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
-00001550: 776f 7264 5f69 6e70 7574 5f70 6c61 6365  word_input_place
-00001560: 686f 6c64 6572 5f74 6578 74da 2264 6961  holder_text."dia
-00001570: 6c6f 675f 656e 6372 7970 745f 7061 7373  log_encrypt_pass
-00001580: 776f 7264 5f68 696e 745f 6c61 6265 6cda  word_hint_label.
-00001590: 2164 6961 6c6f 675f 656e 6372 7970 745f  !dialog_encrypt_
-000015a0: 7061 7373 776f 7264 5f62 7574 746f 6e5f  password_button_
-000015b0: 6f6b da25 6469 616c 6f67 5f65 6e63 7279  ok.%dialog_encry
-000015c0: 7074 5f70 6173 7377 6f72 645f 6275 7474  pt_password_butt
-000015d0: 6f6e 5f63 616e 6365 6cda 2364 6961 6c6f  on_cancel.#dialo
-000015e0: 675f 656e 6372 7970 745f 7061 7373 776f  g_encrypt_passwo
-000015f0: 7264 5f72 6573 6574 5f74 6974 6c65 da22  rd_reset_title."
-00001600: 6469 616c 6f67 5f65 6e63 7279 7074 5f70  dialog_encrypt_p
-00001610: 6173 7377 6f72 645f 7265 7365 745f 7465  assword_reset_te
-00001620: 7874 da2b 6469 616c 6f67 5f65 6e63 7279  xt.+dialog_encry
-00001630: 7074 5f70 6173 7377 6f72 645f 7265 7365  pt_password_rese
-00001640: 745f 6275 7474 6f6e 5f63 616e 6365 6cda  t_button_cancel.
-00001650: 2864 6961 6c6f 675f 656e 6372 7970 745f  (dialog_encrypt_
-00001660: 7061 7373 776f 7264 5f72 6573 6574 5f62  password_reset_b
-00001670: 7574 746f 6e5f 7965 73da 1664 6961 6c6f  utton_yes..dialo
-00001680: 675f 6f70 656e 5f6c 696e 6b5f 7469 746c  g_open_link_titl
-00001690: 65da 1564 6961 6c6f 675f 6f70 656e 5f6c  e..dialog_open_l
-000016a0: 696e 6b5f 7465 7874 da26 6c6f 6164 5f66  ink_text.&load_f
-000016b0: 696c 655f 656e 6372 7970 7469 6f6e 5f70  ile_encryption_p
-000016c0: 6173 7377 6f72 645f 6d69 736d 6174 6368  assword_mismatch
-000016d0: da27 6c6f 6164 5f66 696c 655f 656e 6372  .'load_file_encr
-000016e0: 7970 7469 6f6e 5f70 6173 7377 6f72 645f  yption_password_
-000016f0: 696e 636f 7272 6563 74da 1c6c 6f61 645f  incorrect..load_
-00001700: 6669 6c65 5f6e 6f6e 655f 636f 6e74 656e  file_none_conten
-00001710: 745f 6572 726f 72da 1f73 6176 655f 6163  t_error..save_ac
-00001720: 7469 7665 5f66 696c 655f 6572 726f 725f  tive_file_error_
-00001730: 6f63 6375 7272 6564 da1e 6578 7061 6e64  occurred..expand
-00001740: 6162 6c65 5f62 6c6f 636b 5f64 6566 6175  able_block_defau
-00001750: 6c74 5f74 6974 6c65 da31 6469 616c 6f67  lt_title.1dialog
-00001760: 5f63 6f6c 6f72 5f70 6963 6b65 725f 636f  _color_picker_co
-00001770: 6c6f 725f 636f 7069 6564 5f74 6f5f 7468  lor_copied_to_th
-00001780: 655f 636c 6970 626f 6172 64da 1170 6f70  e_clipboard..pop
-00001790: 7570 5f61 626f 7574 5f74 6974 6c65 da20  up_about_title. 
-000017a0: 706f 7075 705f 6162 6f75 745f 6170 705f  popup_about_app_
-000017b0: 6e61 6d65 5f64 6573 6372 6970 7469 6f6e  name_description
-000017c0: da13 706f 7075 705f 6162 6f75 745f 7665  ..popup_about_ve
-000017d0: 7273 696f 6eda 1370 6f70 7570 5f61 626f  rsion..popup_abo
-000017e0: 7574 5f6c 6963 656e 7365 da13 706f 7075  ut_license..popu
-000017f0: 705f 6162 6f75 745f 7765 6273 6974 65da  p_about_website.
-00001800: 1670 6f70 7570 5f61 626f 7574 5f72 6570  .popup_about_rep
-00001810: 6f73 6974 6f72 79da 1070 6f70 7570 5f61  ository..popup_a
-00001820: 626f 7574 5f64 6174 65da 2675 7064 6174  bout_date.&updat
-00001830: 655f 6865 6c70 6572 5f6e 6577 5f76 6572  e_helper_new_ver
-00001840: 7369 6f6e 5f69 735f 6176 6169 6c61 626c  sion_is_availabl
-00001850: 65da 2675 7064 6174 655f 6865 6c70 6572  e.&update_helper
-00001860: 5f6c 6174 6573 745f 7665 7273 696f 6e5f  _latest_version_
-00001870: 696e 7374 616c 6c65 64da 1e6e 6574 776f  installed..netwo
-00001880: 726b 5f63 6f6e 6e65 6374 696f 6e5f 6572  rk_connection_er
-00001890: 726f 725f 656d 7074 79da 2a6e 6574 776f  ror_empty.*netwo
-000018a0: 726b 5f63 6f6e 6e65 6374 696f 6e5f 6572  rk_connection_er
-000018b0: 726f 725f 636f 6e6e 6563 7469 6f6e 5f6f  ror_connection_o
-000018c0: 725f 646e 73da 2b6e 6574 776f 726b 5f63  r_dns.+network_c
-000018d0: 6f6e 6e65 6374 696f 6e5f 6572 726f 725f  onnection_error_
-000018e0: 636f 6e6e 6563 7469 6f6e 5f72 6566 7573  connection_refus
-000018f0: 6564 da2d 6e65 7477 6f72 6b5f 636f 6e6e  ed.-network_conn
-00001900: 6563 7469 6f6e 5f65 7272 6f72 5f63 6f6e  ection_error_con
-00001910: 6e65 6374 696f 6e5f 7469 6d65 645f 6f75  nection_timed_ou
-00001920: 74da 2d6e 6574 776f 726b 5f63 6f6e 6e65  t.-network_conne
-00001930: 6374 696f 6e5f 6572 726f 725f 636f 6e6e  ction_error_conn
-00001940: 6563 7469 6f6e 5f34 3034 5f65 7272 6f72  ection_404_error
-00001950: da31 6e65 7477 6f72 6b5f 636f 6e6e 6563  .1network_connec
-00001960: 7469 6f6e 5f65 7272 6f72 5f67 656e 6572  tion_error_gener
-00001970: 6963 5f77 6974 685f 7374 6174 7573 5f63  ic_with_status_c
-00001980: 6f64 654e 2901 da07 6c65 7865 6d65 73a9  odeN)...lexemes.
-00001990: 0072 5400 0000 7254 0000 00fa 432f 5573  .rT...rT....C/Us
-000019a0: 6572 732f 7661 6469 6b75 732f 5079 6368  ers/vadikus/Pych
-000019b0: 6172 6d50 726f 6a65 6374 732f 6e6f 746f  armProjects/noto
-000019c0: 6c6f 672f 6e6f 746f 6c6f 672f 6c65 7865  log/notolog/lexe
-000019d0: 6d65 732f 6a61 2f63 6f6d 6d6f 6e2e 7079  mes/ja/common.py
-000019e0: da08 3c6d 6f64 756c 653e 0300 0000 73a6  ..<module>....s.
-000019f0: 0000 0002 0102 0202 0202 0102 0102 0102  ................
-00001a00: 0202 0102 0102 0102 0202 0102 0102 0102  ................
-00001a10: 0102 0102 0202 0102 0102 0102 0202 0102  ................
-00001a20: 0202 0102 0102 0202 0102 0202 0102 0102  ................
-00001a30: 0102 0102 0202 0102 0102 0102 0102 0202  ................
-00001a40: 0102 0102 0102 0102 0302 0102 0102 0102  ................
-00001a50: 0102 0102 0102 0202 0102 0102 0102 0102  ................
-00001a60: 0102 0202 0102 0102 0102 0202 0102 0202  ................
-00001a70: 0102 0102 0202 0202 0202 0202 0102 0202  ................
-00001a80: 0102 0102 0102 0102 0202 0102 0202 0202  ................
-00001a90: 0202 0102 0202 0102 92                   .........
+000000d0: 6447 6448 6449 644a 9c54 5a00 644b 5300  dGdHdIdJ.TZ.dKS.
+000000e0: 294c 7514 0000 004e 6f74 6f6c 6f67 20e3  )Lu....Notolog .
+000000f0: 82a8 e383 87e3 82a3 e382 bf7a 197b 6170  ...........z.{ap
+00000100: 705f 7469 746c 657d 202d 207b 7375 625f  p_title} - {sub_
+00000110: 7469 746c 657d 7527 0000 00e3 8395 e382  title}u'........
+00000120: a1e3 82a4 e383 abe3 8395 e382 a3e3 83ab  ................
+00000130: e382 bfe3 8395 e382 a3e3 83bc e383 abe3  ................
+00000140: 8389 750f 0000 00e5 908d e589 8de3 8292  ..u.............
+00000150: e5a4 89e6 9bb4 7506 0000 00e5 898a e999  ......u.........
+00000160: a475 0f00 0000 e5ae 8ce5 85a8 e381 abe5  .u..............
+00000170: 898a e999 a475 0600 0000 e5be a9e5 8583  .....u..........
+00000180: 7518 0000 00e3 8395 e382 a1e3 82a4 e383  u...............
+00000190: abe5 908d e381 aee5 a489 e69b b475 2100  .............u!.
+000001a0: 0000 e696 b0e3 8197 e381 84e3 8395 e382  ................
+000001b0: a1e3 82a4 e383 abe5 908d e382 92e5 85a5  ................
+000001c0: e58a 9b75 3600 0000 e590 8ce5 908d e381  ...u6...........
+000001d0: aee3 8395 e382 a1e3 82a4 e383 abe3 818c  ................
+000001e0: e381 99e3 81a7 e381 abe5 ad98 e59c a8e3  ................
+000001f0: 8197 e381 a6e3 8184 e381 bee3 8199 7515  ..............u.
+00000200: 0000 00e3 8395 e382 a1e3 82a4 e383 abe3  ................
+00000210: 81ae e589 8ae9 99a4 7533 0000 00e3 8395  ........u3......
+00000220: e382 a1e3 82a4 e383 ab20 227b 6669 6c65  ......... "{file
+00000230: 5f6e 616d 657d 2220 e382 92e5 898a e999  _name}" ........
+00000240: a4e3 8197 e381 bee3 8199 e381 8bef bc9f  ................
+00000250: 751e 0000 00e3 8395 e382 a1e3 82a4 e383  u...............
+00000260: abe3 8292 e5ae 8ce5 85a8 e381 abe5 898a  ................
+00000270: e999 a475 3e00 0000 e383 95e3 82a1 e382  ...u>...........
+00000280: a4e3 83ab e380 8c7b 6669 6c65 5f6e 616d  .......{file_nam
+00000290: 657d e380 8de3 8292 e5ae 8ce5 85a8 e381  e}..............
+000002a0: abe5 898a e999 a4e3 8197 e381 bee3 8199  ................
+000002b0: e381 8bef bc9f 754e 0000 00e3 8395 e382  ......uN........
+000002c0: a1e3 82a4 e383 abe3 8292 e589 8ae9 99a4  ................
+000002d0: e381 a7e3 818d e381 bee3 819b e382 93e3  ................
+000002e0: 81a7 e381 97e3 819f e380 82e3 82a8 e383  ................
+000002f0: a9e3 83bc e381 8ce7 99ba e794 9fe3 8197  ................
+00000300: e381 bee3 8197 e381 9f75 2400 0000 e383  .........u$.....
+00000310: 95e3 82a1 e382 a4e3 83ab e381 8ce8 a68b  ................
+00000320: e381 a4e3 818b e382 8ae3 81be e381 9be3  ................
+00000330: 8293 7515 0000 00e3 8395 e382 a1e3 82a4  ..u.............
+00000340: e383 abe3 8292 e5be a9e5 8583 7533 0000  ............u3..
+00000350: 00e3 8395 e382 a1e3 82a4 e383 ab20 227b  ............. "{
+00000360: 6669 6c65 5f6e 616d 657d 2220 e382 92e5  file_name}" ....
+00000370: bea9 e585 83e3 8197 e381 bee3 8199 e381  ................
+00000380: 8bef bc9f 754e 0000 00e3 8395 e382 a1e3  ....uN..........
+00000390: 82a4 e383 abe3 8292 e5be a9e5 8583 e381  ................
+000003a0: a7e3 818d e381 bee3 819b e382 93e3 81a7  ................
+000003b0: e381 97e3 819f e380 82e3 82a8 e383 a9e3  ................
+000003c0: 83bc e381 8ce7 99ba e794 9fe3 8197 e381  ................
+000003d0: bee3 8197 e381 9f75 4500 0000 7b66 696c  .......uE...{fil
+000003e0: 655f 6e61 6d65 7d20 e381 a8e3 8184 e381  e_name} ........
+000003f0: 86e5 908d e589 8de3 81ae e383 95e3 82a1  ................
+00000400: e382 a4e3 83ab e381 8ce3 8199 e381 a7e3  ................
+00000410: 81ab e5ad 98e5 9ca8 e381 97e3 81be e381  ................
+00000420: 9975 0f00 0000 e383 a1e3 8383 e382 bbe3  .u..............
+00000430: 83bc e382 b875 0900 0000 e996 89e3 8198  .....u..........
+00000440: e382 8b75 1b00 0000 e696 b0e3 8197 e381  ...u............
+00000450: 84e3 8389 e382 ade3 83a5 e383 a1e3 83b3  ................
+00000460: e383 8875 1500 0000 e383 95e3 82a1 e382  ...u............
+00000470: a4e3 83ab e382 92e9 968b e381 8f75 1500  .............u..
+00000480: 0000 e383 95e3 82a1 e382 a4e3 83ab e382  ................
+00000490: 92e4 bf9d e5ad 9875 1b00 0000 e7a9 bae3  .......u........
+000004a0: 81ae e383 95e3 82a1 e382 a4e3 83ab e382  ................
+000004b0: 92e4 bf9d e5ad 9875 3300 0000 e586 85e5  .......u3.......
+000004c0: aeb9 e381 8ce7 a9ba e381 aee3 8395 e382  ................
+000004d0: a1e3 82a4 e383 abe3 8292 e4bf 9de5 ad98  ................
+000004e0: e381 97e3 81be e381 99e3 818b efbc 9f75  ...............u
+000004f0: 1800 0000 e383 95e3 82a1 e382 a4e3 83ab  ................
+00000500: e381 aee6 9a97 e58f b7e5 8c96 7536 0000  ............u6..
+00000510: 00e3 8395 e382 a1e3 82a4 e383 ab20 227b  ............. "{
+00000520: 6669 6c65 5f6e 616d 657d 2220 e382 92e6  file_name}" ....
+00000530: 9a97 e58f b7e5 8c96 e381 97e3 81be e381  ................
+00000540: 99e3 818b efbc 9f75 3600 0000 e383 95e3  .......u6.......
+00000550: 82a1 e382 a4e3 83ab e381 afe3 8199 e381  ................
+00000560: a7e3 81ab e69a 97e5 8fb7 e58c 96e3 8195  ................
+00000570: e382 8ce3 81a6 e381 84e3 81be e381 99ef  ................
+00000580: bc81 7521 0000 00e6 97a2 e5ad 98e3 81ae  ..u!............
+00000590: e383 95e3 82a1 e382 a4e3 83ab e382 92e4  ................
+000005a0: b88a e69b b8e3 818d 753f 0000 00e6 97a2  ........u?......
+000005b0: e5ad 98e3 81ae e383 95e3 82a1 e382 a4e3  ................
+000005c0: 83ab 2022 7b66 696c 655f 7061 7468 7d22  .. "{file_path}"
+000005d0: 20e3 8292 e4b8 8ae6 9bb8 e381 8de3 8197   ...............
+000005e0: e381 bee3 8199 e381 8bef bc9f 7515 0000  ............u...
+000005f0: 00e3 8395 e382 a1e3 82a4 e383 abe3 81ae  ................
+00000600: e5be a9e5 8fb7 7533 0000 00e3 8395 e382  ......u3........
+00000610: a1e3 82a4 e383 ab20 227b 6669 6c65 5f6e  ....... "{file_n
+00000620: 616d 657d 2220 e382 92e5 bea9 e58f b7e3  ame}" ..........
+00000630: 8197 e381 bee3 8199 e381 8bef bc9f 7530  ..............u0
+00000640: 0000 00e3 8395 e382 a1e3 82a4 e383 abe3  ................
+00000650: 81af e69a 97e5 8fb7 e58c 96e3 8195 e382  ................
+00000660: 8ce3 81a6 e381 84e3 81be e381 9be3 8293  ................
+00000670: efbc 8175 1800 0000 e696 b0e3 8197 e381  ...u............
+00000680: 84e3 8391 e382 b9e3 83af e383 bce3 8389  ................
+00000690: 7512 0000 00e3 8391 e382 b9e3 83af e383  u...............
+000006a0: bce3 8389 efbc 9a75 2100 0000 e696 b0e3  .......u!.......
+000006b0: 8197 e381 84e3 8391 e382 b9e3 83af e383  ................
+000006c0: bce3 8389 e382 92e5 85a5 e58a 9b75 0c00  .............u..
+000006d0: 0000 e383 92e3 83b3 e383 88ef bc9a 75e3  ..............u.
+000006e0: 0000 00e3 8392 e383 b3e3 8388 e381 afe6  ................
+000006f0: 9a97 e58f b7e5 8c96 e381 95e3 828c e381  ................
+00000700: 9ae3 81ab e383 95e3 82a1 e382 a4e3 83ab  ................
+00000710: e381 8be3 8289 e8aa ade3 81bf e58f 96e3  ................
+00000720: 828b e381 93e3 81a8 e381 8ce3 81a7 e381  ................
+00000730: 8de3 81be e381 99ef bc81 0ae8 aa95 e794  ................
+00000740: 9fe6 97a5 e381 aae3 81a9 e7b0 a1e5 8d98  ................
+00000750: e381 abe6 8ea8 e6b8 ace3 81a7 e381 8de3  ................
+00000760: 828b e383 92e3 83b3 e383 88e3 81af e4bd  ................
+00000770: bfe7 94a8 e381 97e3 81aa e381 84e3 81a7  ................
+00000780: e381 8fe3 81a0 e381 95e3 8184 e380 820a  ................
+00000790: e996 a2e9 80a3 e680 a7e3 81ae e4bd 8ee3  ................
+000007a0: 8184 e58f 82e7 85a7 e382 92e4 bdbf e794  ................
+000007b0: a8e3 8197 e381 a6e3 818f e381 a0e3 8195  ................
+000007c0: e381 84e3 8082 7527 0000 00e3 8392 e383  ......u'........
+000007d0: b3e3 8388 e382 92e5 85a5 e58a 9bef bc88  ................
+000007e0: e382 aae3 8397 e382 b7e3 83a7 e383 b3ef  ................
+000007f0: bc89 5a02 4f4b 750f 0000 00e3 82ad e383  ..Z.OKu.........
+00000800: a3e3 83b3 e382 bbe3 83ab 7506 0000 00e8  ..........u.....
+00000810: ada6 e591 8a75 2d00 0000 e383 91e3 82b9  .....u-.........
+00000820: e383 afe3 83bc e383 89e6 ac84 e381 afe7  ................
+00000830: a9ba e381 abe3 81a7 e381 8de3 81be e381  ................
+00000840: 9be3 8293 efbc 8175 3f00 0000 e383 92e3  .......u?.......
+00000850: 83b3 e383 88e6 ac84 e381 8ce9 95b7 e381  ................
+00000860: 99e3 818e e381 bee3 8199 e380 82e6 9c80  ................
+00000870: e5a4 a77b 7379 6d62 6f6c 737d e696 87e5  ...{symbols}....
+00000880: ad97 e381 a7e3 8199 efbc 8175 1800 0000  ...........u....
+00000890: e383 91e3 82b9 e383 afe3 83bc e383 89e3  ................
+000008a0: 8292 e585 a5e5 8a9b 7527 0000 00e6 9a97  ........u'......
+000008b0: e58f b7e5 8c96 e383 91e3 82b9 e383 afe3  ................
+000008c0: 83bc e383 89e3 81ae e383 aae3 82bb e383  ................
+000008d0: 83e3 8388 753f 0000 00e7 8fbe e59c a8e3  ....u?..........
+000008e0: 81ae e69a 97e5 8fb7 e58c 96e3 8391 e382  ................
+000008f0: b9e3 83af e383 bce3 8389 e382 92e3 83aa  ................
+00000900: e382 bbe3 8383 e383 88e3 8197 e381 bee3  ................
+00000910: 8199 e381 8bef bc9f 7506 0000 00e3 81af  ........u.......
+00000920: e381 8475 0900 0000 e383 aae3 83b3 e382  ...u............
+00000930: af75 3600 0000 e383 aae3 83b3 e382 af20  .u6............ 
+00000940: 227b 7572 6c7d 2220 e382 92e3 8396 e383  "{url}" ........
+00000950: a9e3 82a6 e382 b6e3 81a7 e996 8be3 818d  ................
+00000960: e381 bee3 8199 e381 8bef bc9f 7530 0000  ............u0..
+00000970: 00e6 9a97 e58f b7e5 8c96 e383 91e3 82b9  ................
+00000980: e383 afe3 83bc e383 89e3 818c e4b8 80e8  ................
+00000990: 87b4 e381 97e3 81be e381 9be3 8293 efbc  ................
+000009a0: 8175 3600 0000 e69a 97e5 8fb7 e58c 96e3  .u6.............
+000009b0: 8391 e382 b9e3 83af e383 bce3 8389 e381  ................
+000009c0: 8ce6 ada3 e381 97e3 818f e381 82e3 828a  ................
+000009d0: e381 bee3 819b e382 93ef bc81 7527 0000  ............u'..
+000009e0: 00e3 8395 e382 a1e3 82a4 e383 abe3 8292  ................
+000009f0: e8aa ade3 81bf e8be bce3 8281 e381 bee3  ................
+00000a00: 819b e382 93e3 8082 754e 0000 00e3 8395  ........uN......
+00000a10: e382 a1e3 82a4 e383 abe3 8292 e4bf 9de5  ................
+00000a20: ad98 e381 a7e3 818d e381 bee3 819b e382  ................
+00000a30: 93e3 81a7 e381 97e3 819f e380 82e3 82a8  ................
+00000a40: e383 a9e3 83bc e381 8ce7 99ba e794 9fe3  ................
+00000a50: 8197 e381 bee3 8197 e381 9f75 0f00 0000  ...........u....
+00000a60: e8a9 b3e7 b4b0 e683 85e5 a0b1 2e2e 2e75  ...............u
+00000a70: 5a00 0000 e383 95e3 82a9 e383 bce3 839e  Z...............
+00000a80: e383 83e3 8388 e381 95e3 828c e381 9fe3  ................
+00000a90: 8386 e382 ade3 82b9 e383 88e3 818c e382  ................
+00000aa0: afe3 83aa e383 83e3 8397 e383 9ce3 83bc  ................
+00000ab0: e383 89e3 81ab e382 b3e3 8394 e383 bce3  ................
+00000ac0: 8195 e382 8ce3 81be e381 97e3 819f 750f  ..............u.
+00000ad0: 0000 00e3 82a2 e383 97e3 83aa e683 85e5  ................
+00000ae0: a0b1 7515 0000 004d 6172 6b64 6f77 6e20  ..u....Markdown 
+00000af0: e382 a8e3 8387 e382 a3e3 82bf 750f 0000  ............u...
+00000b00: 00e3 8390 e383 bce3 82b8 e383 a7e3 83b3  ................
+00000b10: 750f 0000 00e3 83a9 e382 a4e3 82bb e383  u...............
+00000b20: b3e3 82b9 7512 0000 00e3 82a6 e382 a7e3  ....u...........
+00000b30: 8396 e382 b5e3 82a4 e383 885a 0647 6974  ...........Z.Git
+00000b40: 4875 625a 0450 7950 6975 0600 0000 e697  HubZ.PyPiu......
+00000b50: a5e4 bb98 754d 0000 00e3 82a2 e383 97e3  ....uM..........
+00000b60: 83aa e381 aee6 96b0 e381 97e3 8184 e383  ................
+00000b70: 90e3 83bc e382 b8e3 83a7 e383 b320 277b  ............. '{
+00000b80: 6c61 7465 7374 5f76 6572 7369 6f6e 7d27  latest_version}'
+00000b90: 20e3 818c e588 a9e7 94a8 e58f afe8 83bd   ...............
+00000ba0: e381 a7e3 8199 7548 0000 00e3 82a2 e383  ......uH........
+00000bb0: 97e3 83aa e381 aee6 9c80 e696 b0e3 8390  ................
+00000bc0: e383 bce3 82b8 e383 a7e3 83b3 e381 8ce3  ................
+00000bd0: 82a4 e383 b3e3 82b9 e383 88e3 83bc e383  ................
+00000be0: abe3 8195 e382 8ce3 81a6 e381 84e3 81be  ................
+00000bf0: e381 9975 2400 0000 e5bf 9ce7 ad94 e683  ...u$...........
+00000c00: 85e5 a0b1 e382 92e5 8f96 e5be 97e3 81a7  ................
+00000c10: e381 8de3 81be e381 9be3 8293 7575 0000  ............uu..
+00000c20: 00e3 839b e382 b9e3 8388 e381 8ce8 a68b  ................
+00000c30: e381 a4e3 818b e382 8ae3 81be e381 9be3  ................
+00000c40: 8293 e380 82e3 82a4 e383 b3e3 82bf e383  ................
+00000c50: bce3 838d e383 83e3 8388 e68e a5e7 b69a  ................
+00000c60: e381 bee3 819f e381 af44 4e53 e381 abe5  .........DNS....
+00000c70: 958f e9a1 8ce3 818c e381 82e3 828b e381  ................
+00000c80: 8be3 8282 e381 97e3 828c e381 bee3 819b  ................
+00000c90: e382 93e3 8082 758a 0000 00e6 8ea5 e7b6  ......u.........
+00000ca0: 9ae3 818c e68b 92e5 90a6 e381 95e3 828c  ................
+00000cb0: e381 bee3 8197 e381 9fe3 8082 e382 b5e3  ................
+00000cc0: 83bc e383 90e3 83bc e381 8ce3 8380 e382  ................
+00000cd0: a6e3 83b3 e381 97e3 81a6 e381 84e3 828b  ................
+00000ce0: e381 8be3 8081 e383 8de3 8383 e383 88e3  ................
+00000cf0: 83af e383 bce3 82af e381 abe5 958f e9a1  ................
+00000d00: 8ce3 818c e381 82e3 828b e58f afe8 83bd  ................
+00000d10: e680 a7e3 818c e381 82e3 828a e381 bee3  ................
+00000d20: 8199 e380 8275 6600 0000 e68e a5e7 b69a  .....uf.........
+00000d30: e381 8ce3 82bf e382 a4e3 83a0 e382 a2e3  ................
+00000d40: 82a6 e383 88e3 8197 e381 bee3 8197 e381  ................
+00000d50: 9fe3 8082 e383 8de3 8383 e383 88e3 83af  ................
+00000d60: e383 bce3 82af e381 abe5 958f e9a1 8ce3  ................
+00000d70: 818c e381 82e3 828b e381 8be3 8282 e381  ................
+00000d80: 97e3 828c e381 bee3 819b e382 93e3 8082  ................
+00000d90: 755d 0000 00e6 8ea5 e7b6 9a34 3034 e382  u].........404..
+00000da0: a8e3 83a9 e383 bce3 8082 e8a6 81e6 b182  ................
+00000db0: e381 95e3 828c e381 9fe3 839a e383 bce3  ................
+00000dc0: 82b8 e381 bee3 819f e381 afe3 83aa e382  ................
+00000dd0: bde3 83bc e382 b9e3 818c e8a6 8be3 81a4  ................
+00000de0: e381 8be3 828a e381 bee3 819b e382 93e3  ................
+00000df0: 8082 754c 0000 00e3 82b9 e383 86e3 83bc  ..uL............
+00000e00: e382 bfe3 82b9 e382 b3e3 83bc e383 897b  ...............{
+00000e10: 7374 6174 7573 5f63 6f64 657d e381 a7e3  status_code}....
+00000e20: 83aa e382 afe3 82a8 e382 b9e3 8388 e381  ................
+00000e30: 8ce5 a4b1 e695 97e3 8197 e381 bee3 8197  ................
+00000e40: e381 9f29 54da 0961 7070 5f74 6974 6c65  ...)T..app_title
+00000e50: da12 6170 705f 7469 746c 655f 7769 7468  ..app_title_with
+00000e60: 5f73 7562 da1b 7472 6565 5f66 696c 7465  _sub..tree_filte
+00000e70: 725f 6163 6365 7373 6962 6c65 5f64 6573  r_accessible_des
+00000e80: 63da 126d 656e 755f 6163 7469 6f6e 5f72  c..menu_action_r
+00000e90: 656e 616d 65da 126d 656e 755f 6163 7469  ename..menu_acti
+00000ea0: 6f6e 5f64 656c 6574 65da 1d6d 656e 755f  on_delete..menu_
+00000eb0: 6163 7469 6f6e 5f64 656c 6574 655f 636f  action_delete_co
+00000ec0: 6d70 6c65 7465 6c79 da13 6d65 6e75 5f61  mpletely..menu_a
+00000ed0: 6374 696f 6e5f 7265 7374 6f72 65da 1864  ction_restore..d
+00000ee0: 6961 6c6f 675f 6669 6c65 5f72 656e 616d  ialog_file_renam
+00000ef0: 655f 7469 746c 65da 1e64 6961 6c6f 675f  e_title..dialog_
+00000f00: 6669 6c65 5f72 656e 616d 655f 6669 656c  file_rename_fiel
+00000f10: 645f 6c61 6265 6cda 1c64 6961 6c6f 675f  d_label..dialog_
+00000f20: 6669 6c65 5f72 656e 616d 655f 6275 7474  file_rename_butt
+00000f30: 6f6e 5f6f 6bda 2164 6961 6c6f 675f 6669  on_ok.!dialog_fi
+00000f40: 6c65 5f72 656e 616d 655f 7761 726e 696e  le_rename_warnin
+00000f50: 675f 6578 6973 7473 da18 6469 616c 6f67  g_exists..dialog
+00000f60: 5f66 696c 655f 6465 6c65 7465 5f74 6974  _file_delete_tit
+00000f70: 6c65 da17 6469 616c 6f67 5f66 696c 655f  le..dialog_file_
+00000f80: 6465 6c65 7465 5f74 6578 74da 2364 6961  delete_text.#dia
+00000f90: 6c6f 675f 6669 6c65 5f64 656c 6574 655f  log_file_delete_
+00000fa0: 636f 6d70 6c65 7465 6c79 5f74 6974 6c65  completely_title
+00000fb0: da22 6469 616c 6f67 5f66 696c 655f 6465  ."dialog_file_de
+00000fc0: 6c65 7465 5f63 6f6d 706c 6574 656c 795f  lete_completely_
+00000fd0: 7465 7874 da18 6469 616c 6f67 5f66 696c  text..dialog_fil
+00000fe0: 655f 6465 6c65 7465 5f65 7272 6f72 da22  e_delete_error."
+00000ff0: 6469 616c 6f67 5f66 696c 655f 6465 6c65  dialog_file_dele
+00001000: 7465 5f65 7272 6f72 5f6e 6f74 5f66 6f75  te_error_not_fou
+00001010: 6e64 da19 6469 616c 6f67 5f66 696c 655f  nd..dialog_file_
+00001020: 7265 7374 6f72 655f 7469 746c 65da 1864  restore_title..d
+00001030: 6961 6c6f 675f 6669 6c65 5f72 6573 746f  ialog_file_resto
+00001040: 7265 5f74 6578 745a 1964 6961 6c6f 675f  re_textZ.dialog_
+00001050: 6669 6c65 5f72 6573 746f 7265 5f65 7272  file_restore_err
+00001060: 6f72 da22 6469 616c 6f67 5f66 696c 655f  or."dialog_file_
+00001070: 7265 7374 6f72 655f 7761 726e 696e 675f  restore_warning_
+00001080: 6578 6973 7473 da18 6469 616c 6f67 5f6d  exists..dialog_m
+00001090: 6573 7361 6765 5f62 6f78 5f74 6974 6c65  essage_box_title
+000010a0: da1c 6469 616c 6f67 5f6d 6573 7361 6765  ..dialog_message
+000010b0: 5f62 6f78 5f62 7574 746f 6e5f 6f6b da28  _box_button_ok.(
+000010c0: 6163 7469 6f6e 5f6e 6577 5f66 696c 655f  action_new_file_
+000010d0: 6669 7273 745f 6c69 6e65 5f74 656d 706c  first_line_templ
+000010e0: 6174 655f 7465 7874 da1f 6163 7469 6f6e  ate_text..action
+000010f0: 5f6f 7065 6e5f 6669 6c65 5f64 6961 6c6f  _open_file_dialo
+00001100: 675f 6361 7074 696f 6eda 2261 6374 696f  g_caption."actio
+00001110: 6e5f 7361 7665 5f61 735f 6669 6c65 5f64  n_save_as_file_d
+00001120: 6961 6c6f 675f 6361 7074 696f 6eda 1c64  ialog_caption..d
+00001130: 6961 6c6f 675f 7361 7665 5f65 6d70 7479  ialog_save_empty
+00001140: 5f66 696c 655f 7469 746c 65da 1b64 6961  _file_title..dia
+00001150: 6c6f 675f 7361 7665 5f65 6d70 7479 5f66  log_save_empty_f
+00001160: 696c 655f 7465 7874 da19 6469 616c 6f67  ile_text..dialog
+00001170: 5f65 6e63 7279 7074 5f66 696c 655f 7469  _encrypt_file_ti
+00001180: 746c 65da 1864 6961 6c6f 675f 656e 6372  tle..dialog_encr
+00001190: 7970 745f 6669 6c65 5f74 6578 74da 2e65  ypt_file_text..e
+000011a0: 6e63 7279 7074 5f66 696c 655f 7761 726e  ncrypt_file_warn
+000011b0: 696e 675f 6669 6c65 5f69 735f 616c 7265  ing_file_is_alre
+000011c0: 6164 795f 656e 6372 7970 7465 64da 2a64  ady_encrypted.*d
+000011d0: 6961 6c6f 675f 656e 6372 7970 745f 6669  ialog_encrypt_fi
+000011e0: 6c65 5f72 6577 7269 7465 5f65 7869 7374  le_rewrite_exist
+000011f0: 696e 675f 7469 746c 65da 2964 6961 6c6f  ing_title.)dialo
+00001200: 675f 656e 6372 7970 745f 6669 6c65 5f72  g_encrypt_file_r
+00001210: 6577 7269 7465 5f65 7869 7374 696e 675f  ewrite_existing_
+00001220: 7465 7874 da19 6469 616c 6f67 5f64 6563  text..dialog_dec
+00001230: 7279 7074 5f66 696c 655f 7469 746c 65da  rypt_file_title.
+00001240: 1864 6961 6c6f 675f 6465 6372 7970 745f  .dialog_decrypt_
+00001250: 6669 6c65 5f74 6578 74da 2a64 6563 7279  file_text.*decry
+00001260: 7074 5f66 696c 655f 7761 726e 696e 675f  pt_file_warning_
+00001270: 6669 6c65 5f69 735f 6e6f 745f 656e 6372  file_is_not_encr
+00001280: 7970 7465 64da 2a64 6961 6c6f 675f 6465  ypted.*dialog_de
+00001290: 6372 7970 745f 6669 6c65 5f72 6577 7269  crypt_file_rewri
+000012a0: 7465 5f65 7869 7374 696e 675f 7469 746c  te_existing_titl
+000012b0: 65da 2964 6961 6c6f 675f 6465 6372 7970  e.)dialog_decryp
+000012c0: 745f 6669 6c65 5f72 6577 7269 7465 5f65  t_file_rewrite_e
+000012d0: 7869 7374 696e 675f 7465 7874 da21 6469  xisting_text.!di
+000012e0: 616c 6f67 5f65 6e63 7279 7074 5f6e 6577  alog_encrypt_new
+000012f0: 5f70 6173 7377 6f72 645f 7469 746c 65da  _password_title.
+00001300: 2164 6961 6c6f 675f 656e 6372 7970 745f  !dialog_encrypt_
+00001310: 6e65 775f 7061 7373 776f 7264 5f6c 6162  new_password_lab
+00001320: 656c da32 6469 616c 6f67 5f65 6e63 7279  el.2dialog_encry
+00001330: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
+00001340: 696e 7075 745f 706c 6163 6568 6f6c 6465  input_placeholde
+00001350: 725f 7465 7874 da26 6469 616c 6f67 5f65  r_text.&dialog_e
+00001360: 6e63 7279 7074 5f6e 6577 5f70 6173 7377  ncrypt_new_passw
+00001370: 6f72 645f 6869 6e74 5f6c 6162 656c da32  ord_hint_label.2
+00001380: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
+00001390: 6577 5f70 6173 7377 6f72 645f 6869 6e74  ew_password_hint
+000013a0: 5f6c 6162 656c 5f64 6573 6372 6970 7469  _label_descripti
+000013b0: 6f6e da37 6469 616c 6f67 5f65 6e63 7279  on.7dialog_encry
+000013c0: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
+000013d0: 6869 6e74 5f69 6e70 7574 5f70 6c61 6365  hint_input_place
+000013e0: 686f 6c64 6572 5f74 6578 74da 2564 6961  holder_text.%dia
+000013f0: 6c6f 675f 656e 6372 7970 745f 6e65 775f  log_encrypt_new_
+00001400: 7061 7373 776f 7264 5f62 7574 746f 6e5f  password_button_
+00001410: 6f6b da29 6469 616c 6f67 5f65 6e63 7279  ok.)dialog_encry
+00001420: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
+00001430: 6275 7474 6f6e 5f63 616e 6365 6cda 2f64  button_cancel./d
+00001440: 6961 6c6f 675f 656e 6372 7970 745f 6e65  ialog_encrypt_ne
+00001450: 775f 7061 7373 776f 7264 5f77 6172 6e69  w_password_warni
+00001460: 6e67 5f65 6d70 7479 5f74 6974 6c65 da2e  ng_empty_title..
+00001470: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
+00001480: 6577 5f70 6173 7377 6f72 645f 7761 726e  ew_password_warn
+00001490: 696e 675f 656d 7074 795f 7465 7874 da32  ing_empty_text.2
+000014a0: 6469 616c 6f67 5f65 6e63 7279 7074 5f6e  dialog_encrypt_n
+000014b0: 6577 5f70 6173 7377 6f72 645f 7761 726e  ew_password_warn
+000014c0: 696e 675f 746f 6f5f 6c6f 6e67 5f74 6974  ing_too_long_tit
+000014d0: 6c65 da31 6469 616c 6f67 5f65 6e63 7279  le.1dialog_encry
+000014e0: 7074 5f6e 6577 5f70 6173 7377 6f72 645f  pt_new_password_
+000014f0: 7761 726e 696e 675f 746f 6f5f 6c6f 6e67  warning_too_long
+00001500: 5f74 6578 74da 1d64 6961 6c6f 675f 656e  _text..dialog_en
+00001510: 6372 7970 745f 7061 7373 776f 7264 5f74  crypt_password_t
+00001520: 6974 6c65 da1d 6469 616c 6f67 5f65 6e63  itle..dialog_enc
+00001530: 7279 7074 5f70 6173 7377 6f72 645f 6c61  rypt_password_la
+00001540: 6265 6cda 2e64 6961 6c6f 675f 656e 6372  bel..dialog_encr
+00001550: 7970 745f 7061 7373 776f 7264 5f69 6e70  ypt_password_inp
+00001560: 7574 5f70 6c61 6365 686f 6c64 6572 5f74  ut_placeholder_t
+00001570: 6578 74da 2264 6961 6c6f 675f 656e 6372  ext."dialog_encr
+00001580: 7970 745f 7061 7373 776f 7264 5f68 696e  ypt_password_hin
+00001590: 745f 6c61 6265 6cda 2164 6961 6c6f 675f  t_label.!dialog_
+000015a0: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
+000015b0: 5f62 7574 746f 6e5f 6f6b da25 6469 616c  _button_ok.%dial
+000015c0: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
+000015d0: 6f72 645f 6275 7474 6f6e 5f63 616e 6365  ord_button_cance
+000015e0: 6cda 2364 6961 6c6f 675f 656e 6372 7970  l.#dialog_encryp
+000015f0: 745f 7061 7373 776f 7264 5f72 6573 6574  t_password_reset
+00001600: 5f74 6974 6c65 da22 6469 616c 6f67 5f65  _title."dialog_e
+00001610: 6e63 7279 7074 5f70 6173 7377 6f72 645f  ncrypt_password_
+00001620: 7265 7365 745f 7465 7874 da2b 6469 616c  reset_text.+dial
+00001630: 6f67 5f65 6e63 7279 7074 5f70 6173 7377  og_encrypt_passw
+00001640: 6f72 645f 7265 7365 745f 6275 7474 6f6e  ord_reset_button
+00001650: 5f63 616e 6365 6cda 2864 6961 6c6f 675f  _cancel.(dialog_
+00001660: 656e 6372 7970 745f 7061 7373 776f 7264  encrypt_password
+00001670: 5f72 6573 6574 5f62 7574 746f 6e5f 7965  _reset_button_ye
+00001680: 73da 1664 6961 6c6f 675f 6f70 656e 5f6c  s..dialog_open_l
+00001690: 696e 6b5f 7469 746c 65da 1564 6961 6c6f  ink_title..dialo
+000016a0: 675f 6f70 656e 5f6c 696e 6b5f 7465 7874  g_open_link_text
+000016b0: da26 6c6f 6164 5f66 696c 655f 656e 6372  .&load_file_encr
+000016c0: 7970 7469 6f6e 5f70 6173 7377 6f72 645f  yption_password_
+000016d0: 6d69 736d 6174 6368 da27 6c6f 6164 5f66  mismatch.'load_f
+000016e0: 696c 655f 656e 6372 7970 7469 6f6e 5f70  ile_encryption_p
+000016f0: 6173 7377 6f72 645f 696e 636f 7272 6563  assword_incorrec
+00001700: 74da 1c6c 6f61 645f 6669 6c65 5f6e 6f6e  t..load_file_non
+00001710: 655f 636f 6e74 656e 745f 6572 726f 72da  e_content_error.
+00001720: 1f73 6176 655f 6163 7469 7665 5f66 696c  .save_active_fil
+00001730: 655f 6572 726f 725f 6f63 6375 7272 6564  e_error_occurred
+00001740: da1e 6578 7061 6e64 6162 6c65 5f62 6c6f  ..expandable_blo
+00001750: 636b 5f64 6566 6175 6c74 5f74 6974 6c65  ck_default_title
+00001760: da31 6469 616c 6f67 5f63 6f6c 6f72 5f70  .1dialog_color_p
+00001770: 6963 6b65 725f 636f 6c6f 725f 636f 7069  icker_color_copi
+00001780: 6564 5f74 6f5f 7468 655f 636c 6970 626f  ed_to_the_clipbo
+00001790: 6172 64da 1170 6f70 7570 5f61 626f 7574  ard..popup_about
+000017a0: 5f74 6974 6c65 da20 706f 7075 705f 6162  _title. popup_ab
+000017b0: 6f75 745f 6170 705f 6e61 6d65 5f64 6573  out_app_name_des
+000017c0: 6372 6970 7469 6f6e da13 706f 7075 705f  cription..popup_
+000017d0: 6162 6f75 745f 7665 7273 696f 6eda 1370  about_version..p
+000017e0: 6f70 7570 5f61 626f 7574 5f6c 6963 656e  opup_about_licen
+000017f0: 7365 da13 706f 7075 705f 6162 6f75 745f  se..popup_about_
+00001800: 7765 6273 6974 65da 1670 6f70 7570 5f61  website..popup_a
+00001810: 626f 7574 5f72 6570 6f73 6974 6f72 79da  bout_repository.
+00001820: 1070 6f70 7570 5f61 626f 7574 5f70 7970  .popup_about_pyp
+00001830: 69da 1070 6f70 7570 5f61 626f 7574 5f64  i..popup_about_d
+00001840: 6174 65da 2675 7064 6174 655f 6865 6c70  ate.&update_help
+00001850: 6572 5f6e 6577 5f76 6572 7369 6f6e 5f69  er_new_version_i
+00001860: 735f 6176 6169 6c61 626c 65da 2675 7064  s_available.&upd
+00001870: 6174 655f 6865 6c70 6572 5f6c 6174 6573  ate_helper_lates
+00001880: 745f 7665 7273 696f 6e5f 696e 7374 616c  t_version_instal
+00001890: 6c65 64da 1e6e 6574 776f 726b 5f63 6f6e  led..network_con
+000018a0: 6e65 6374 696f 6e5f 6572 726f 725f 656d  nection_error_em
+000018b0: 7074 79da 2a6e 6574 776f 726b 5f63 6f6e  pty.*network_con
+000018c0: 6e65 6374 696f 6e5f 6572 726f 725f 636f  nection_error_co
+000018d0: 6e6e 6563 7469 6f6e 5f6f 725f 646e 73da  nnection_or_dns.
+000018e0: 2b6e 6574 776f 726b 5f63 6f6e 6e65 6374  +network_connect
+000018f0: 696f 6e5f 6572 726f 725f 636f 6e6e 6563  ion_error_connec
+00001900: 7469 6f6e 5f72 6566 7573 6564 da2d 6e65  tion_refused.-ne
+00001910: 7477 6f72 6b5f 636f 6e6e 6563 7469 6f6e  twork_connection
+00001920: 5f65 7272 6f72 5f63 6f6e 6e65 6374 696f  _error_connectio
+00001930: 6e5f 7469 6d65 645f 6f75 74da 2d6e 6574  n_timed_out.-net
+00001940: 776f 726b 5f63 6f6e 6e65 6374 696f 6e5f  work_connection_
+00001950: 6572 726f 725f 636f 6e6e 6563 7469 6f6e  error_connection
+00001960: 5f34 3034 5f65 7272 6f72 da31 6e65 7477  _404_error.1netw
+00001970: 6f72 6b5f 636f 6e6e 6563 7469 6f6e 5f65  ork_connection_e
+00001980: 7272 6f72 5f67 656e 6572 6963 5f77 6974  rror_generic_wit
+00001990: 685f 7374 6174 7573 5f63 6f64 654e 2901  h_status_codeN).
+000019a0: da07 6c65 7865 6d65 73a9 0072 5500 0000  ..lexemes..rU...
+000019b0: 7255 0000 00fa 432f 5573 6572 732f 7661  rU....C/Users/va
+000019c0: 6469 6b75 732f 5079 6368 6172 6d50 726f  dikus/PycharmPro
+000019d0: 6a65 6374 732f 6e6f 746f 6c6f 672d 6465  jects/notolog-de
+000019e0: 762f 6170 702f 6c65 7865 6d65 732f 6a61  v/app/lexemes/ja
+000019f0: 2f63 6f6d 6d6f 6e2e 7079 da08 3c6d 6f64  /common.py..<mod
+00001a00: 756c 653e 0300 0000 73a8 0000 0002 0102  ule>....s.......
+00001a10: 0202 0202 0102 0102 0102 0202 0102 0102  ................
+00001a20: 0102 0202 0102 0102 0102 0102 0102 0202  ................
+00001a30: 0102 0102 0102 0202 0102 0202 0102 0102  ................
+00001a40: 0202 0102 0202 0102 0102 0102 0102 0202  ................
+00001a50: 0102 0102 0102 0102 0202 0102 0102 0102  ................
+00001a60: 0102 0302 0102 0102 0102 0102 0102 0102  ................
+00001a70: 0202 0102 0102 0102 0102 0102 0202 0102  ................
+00001a80: 0102 0102 0202 0102 0202 0102 0102 0202  ................
+00001a90: 0202 0202 0202 0102 0202 0102 0102 0102  ................
+00001aa0: 0102 0102 0202 0102 0202 0202 0202 0102  ................
+00001ab0: 0202 0102 91                             .....
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/main_menu.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 2443 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 8b09 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 8b09 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0029 0000 0040 0000 0073 5a00 0000 6400  .)...@...sZ...d.
 00000030: 6401 6402 6403 6404 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640b 6401 640c 640d  d.d.d.d.d.d.d.d.
 00000050: 640e 640f 6410 6411 6412 6413 6414 6415  d.d.d.d.d.d.d.d.
 00000060: 6416 6417 6418 6419 641a 641b 641c 641d  d.d.d.d.d.d.d.d.
 00000070: 641d 641e 641e 641f 6420 6421 6421 6422  d.d.d.d.d d!d!d"
@@ -136,15 +136,15 @@
 00000870: 6f6e 735f 6865 6c70 5f6c 6162 656c 5f61  ons_help_label_a
 00000880: 626f 7574 da22 6163 7469 6f6e 735f 6865  bout."actions_he
 00000890: 6c70 5f61 6363 6573 7369 626c 655f 6e61  lp_accessible_na
 000008a0: 6d65 5f61 626f 7574 4e29 01da 076c 6578  me_aboutN)...lex
 000008b0: 656d 6573 a900 7228 0000 0072 2800 0000  emes..r(...r(...
 000008c0: fa46 2f55 7365 7273 2f76 6164 696b 7573  .F/Users/vadikus
 000008d0: 2f50 7963 6861 726d 5072 6f6a 6563 7473  /PycharmProjects
-000008e0: 2f6e 6f74 6f6c 6f67 2f6e 6f74 6f6c 6f67  /notolog/notolog
+000008e0: 2f6e 6f74 6f6c 6f67 2d64 6576 2f61 7070  /notolog-dev/app
 000008f0: 2f6c 6578 656d 6573 2f6a 612f 6d61 696e  /lexemes/ja/main
 00000900: 5f6d 656e 752e 7079 da08 3c6d 6f64 756c  _menu.py..<modul
 00000910: 653e 0300 0000 7350 0000 0002 0102 0102  e>....sP........
 00000920: 0102 0202 0102 0102 0102 0102 0102 0102  ................
 00000930: 0102 0102 0102 0202 0102 0102 0102 0102  ................
 00000940: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000950: 0102 0202 0102 0102 0102 0202 0102 0102  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/settings_dialog.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 3747 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,237 +1,253 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 a30e 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 42a9 3566 ae0f 0000  a.......B.5f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 002e 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
+00000020: 0030 0000 0040 0000 0073 6800 0000 6400  .0...@...sh...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 6412 6413 6414 6415 6416 6417 6418  d.d.d.d.d.d.d.d.
 00000060: 6419 641a 641b 641c 641d 641e 641f 6420  d.d.d.d.d.d.d.d 
 00000070: 6421 6422 6423 6424 6425 6426 6427 6428  d!d"d#d$d%d&d'd(
-00000080: 6429 642a 642b 642c 642d 9c2d 5a00 642e  d)d*d+d,d-.-Z.d.
-00000090: 5300 292f 7506 0000 00e8 a8ad e5ae 9a75  S.)/u..........u
-000000a0: 0900 0000 e996 89e3 8198 e382 8b75 0600  .............u..
-000000b0: 0000 e4b8 80e8 88ac 750f 0000 00e3 82a8  ........u.......
-000000c0: e383 87e3 82a3 e382 bfe3 83bc 750c 0000  ............u...
-000000d0: 00e3 8393 e383 a5e3 83bc e382 a275 0900  .............u..
-000000e0: 0000 4149 20e8 a8ad e5ae 9a75 0f00 0000  ..AI ......u....
-000000f0: e382 a2e3 8397 e383 aae8 a8ad e5ae 9a75  ...............u
-00000100: 0600 0000 e8a8 80e8 aa9e 750f 0000 00e8  ..........u.....
-00000110: a880 e8aa 9ee3 8292 e981 b8e6 8a9e 752a  ..............u*
-00000120: 0000 00e3 82a2 e383 97e3 83aa e381 aee3  ................
-00000130: 82a4 e383 b3e3 82bf e383 bce3 8395 e382  ................
-00000140: a7e3 83bc e382 b9e8 a880 e8aa 9e75 0900  .............u..
-00000150: 0000 e383 86e3 83bc e383 9e75 1200 0000  ...........u....
-00000160: e383 86e3 83bc e383 9ee3 8292 e981 b8e6  ................
-00000170: 8a9e 752d 0000 00e3 82a2 e383 97e3 83aa  ..u-............
-00000180: e381 aee3 82a4 e383 b3e3 82bf e383 bce3  ................
-00000190: 8395 e382 a7e3 83bc e382 b9e3 8386 e383  ................
-000001a0: bce3 839e 7515 0000 00e3 83a1 e382 a4e3  ....u...........
-000001b0: 83b3 e383 a1e3 838b e383 a5e3 83bc 751e  ..............u.
-000001c0: 0000 00e3 83a1 e382 a4e3 83b3 e383 a1e3  ................
-000001d0: 838b e383 a5e3 83bc e382 92e8 a1a8 e7a4  ................
-000001e0: ba75 3f00 0000 e382 a2e3 8397 e383 aae3  .u?.............
-000001f0: 81ae e383 a1e3 82a4 e383 b3e3 8389 e383  ................
-00000200: ade3 8383 e383 97e3 8380 e382 a6e3 83b3  ................
-00000210: e383 a1e3 838b e383 a5e3 83bc e382 92e8  ................
-00000220: a1a8 e7a4 ba75 2000 0000 e383 95e3 82a9  .....u .........
-00000230: e383 b3e3 8388 e382 b5e3 82a4 e382 baef  ................
-00000240: bc9a 7b73 697a 657d 7074 753c 0000 00e3  ..{size}ptu<....
-00000250: 82a2 e383 97e3 83aa e381 aee5 85a8 e4bd  ................
-00000260: 93e7 9a84 e381 aae3 8395 e382 a9e3 83b3  ................
-00000270: e383 88e3 82b5 e382 a4e3 82ba e382 92e8  ................
-00000280: aabf e695 b4e3 8199 e382 8b75 1500 0000  ...........u....
-00000290: e382 b9e3 8386 e383 bce3 82bf e382 b9e3  ................
-000002a0: 8390 e383 bc75 2a00 0000 e382 b0e3 83ad  .....u*.........
-000002b0: e383 bce3 8390 e383 abe3 82ab e383 bce3  ................
-000002c0: 82bd e383 abe4 bd8d e7bd aee3 8292 e8a1  ................
-000002d0: a8e7 a4ba 7548 0000 00e3 82b9 e383 86e3  ....uH..........
-000002e0: 83bc e382 bfe3 82b9 e383 90e3 83bc e381  ................
-000002f0: abe3 82b0 e383 ade3 83bc e383 90e3 83ab  ................
-00000300: e382 abe3 83bc e382 bde3 83ab e4bd 8de7  ................
-00000310: bdae e382 92e8 a1a8 e7a4 bae3 8199 e382  ................
-00000320: 8b75 1200 0000 e382 a8e3 8387 e382 a3e3  .u..............
-00000330: 82bf e8a8 ade5 ae9a 7512 0000 00e8 a18c  ........u.......
-00000340: e795 aae5 8fb7 e382 92e8 a1a8 e7a4 ba75  ...............u
-00000350: 2a00 0000 e382 a8e3 8387 e382 a3e3 82bf  *...............
-00000360: e586 85e3 81a7 e8a1 8ce7 95aa e58f b7e3  ................
-00000370: 8292 e8a1 a8e7 a4ba e381 99e3 828b 7512  ..............u.
-00000380: 0000 00e3 8393 e383 a5e3 83bc e383 afe8  ................
-00000390: a8ad e5ae 9a75 3300 0000 e383 86e3 82ad  .....u3.........
-000003a0: e382 b9e3 8388 e7b5 b5e6 9687 e5ad 97e3  ................
-000003b0: 8292 e382 b0e3 83a9 e383 95e3 82a3 e383  ................
-000003c0: 83e3 82af e381 abe5 a489 e68f 9b75 4200  .............uB.
-000003d0: 0000 e383 86e3 82ad e382 b9e3 8388 e7b5  ................
-000003e0: b5e6 9687 e5ad 97e3 8292 e382 b0e3 83a9  ................
-000003f0: e383 95e3 82a3 e382 abe3 83ab e381 aae8  ................
-00000400: a1a8 e78f bee3 81ab e5a4 89e6 8f9b e381  ................
-00000410: 99e3 828b 7516 0000 0054 4f44 4fe3 8292  ....u....TODO...
-00000420: e383 8fe3 82a4 e383 a9e3 82a4 e383 8875  ...............u
-00000430: 3100 0000 e383 86e3 82ad e382 b9e3 8388  1...............
-00000440: e586 85e3 81ae 544f 444f e382 bfe3 82b0  ......TODO......
-00000450: e382 92e5 bcb7 e8aa bfe8 a1a8 e7a4 bae3  ................
-00000460: 8199 e382 8b75 2400 0000 e383 aae3 83b3  .....u$.........
-00000470: e382 afe9 968b e381 8fe5 898d e381 abe7  ................
-00000480: a2ba e8aa 8de3 818c e5bf 85e8 a681 752a  ..............u*
-00000490: 0000 00e3 83aa e383 b3e3 82af e382 92e9  ................
-000004a0: 968b e381 8fe5 898d e381 abe7 a2ba e8aa  ................
-000004b0: 8de3 8292 e6b1 82e3 8281 e382 8b7a 0a4f  .............z.O
-000004c0: 7065 6e41 4920 4150 497a 0741 5049 2055  penAI APIz.API U
-000004d0: 524c 7510 0000 004f 7065 6e41 4920 4150  RLu....OpenAI AP
-000004e0: 49e3 81ae 5552 4c75 0a00 0000 4150 4920  I...URLu....API 
-000004f0: e382 ade3 83bc 7513 0000 004f 7065 6e41  ......u....OpenA
-00000500: 4920 4150 49e3 81ae e382 ade3 83bc 7524  I API.........u$
-00000510: 0000 00e3 82b5 e383 9de3 83bc e383 88e3  ................
-00000520: 8195 e382 8ce3 81a6 e381 84e3 828b e383  ................
-00000530: a2e3 8387 e383 ab75 1200 0000 e383 a2e3  .......u........
-00000540: 8387 e383 abe3 8292 e981 b8e6 8a9e 7533  ..............u3
-00000550: 0000 00e9 81b8 e68a 9ee5 8faf e883 bde3  ................
-00000560: 81aa e382 b5e3 839d e383 bce3 8388 e381  ................
-00000570: 95e3 828c e381 a6e3 8184 e382 8be3 83a2  ................
-00000580: e383 87e3 83ab 7515 0000 00e5 9fba e69c  ......u.........
-00000590: ace3 8391 e383 a9e3 83a1 e383 bce3 82bf  ................
-000005a0: 751b 0000 00e3 82b7 e382 b9e3 8386 e383  u...............
-000005b0: a0e3 8397 e383 ade3 83b3 e383 97e3 8388  ................
-000005c0: 753f 0000 00e5 9084 e383 aae3 82af e382  u?..............
-000005d0: a8e3 82b9 e383 88e3 81ab e585 88e7 ab8b  ................
-000005e0: e381 a4e5 9fba e69c ace3 82b7 e382 b9e3  ................
-000005f0: 8386 e383 a0e3 8397 e383 ade3 83b3 e383  ................
-00000600: 97e3 8388 755d 0000 00e5 9084 e383 aae3  ....u]..........
-00000610: 82af e382 a8e3 82b9 e383 88e3 81ab e585  ................
-00000620: 88e7 ab8b e381 a4e5 9fba e69c ace3 82b7  ................
-00000630: e382 b9e3 8386 e383 a0e3 8397 e383 ade3  ................
-00000640: 83b3 e383 97e3 8388 e380 82e3 8397 e383  ................
-00000650: ace3 83bc e383 b3e3 8386 e382 ade3 82b9  ................
-00000660: e383 88e3 8082 751e 0000 00e5 bf9c e7ad  ......u.........
-00000670: 94e3 81ae e69c 80e5 a4a7 e383 88e3 83bc  ................
-00000680: e382 afe3 83b3 e695 b075 2a00 0000 e5bf  .........u*.....
-00000690: 9ce7 ad94 e381 a7e5 8f97 e381 91e5 8f96  ................
-000006a0: e382 8be6 9c80 e5a4 a7e3 8388 e383 bce3  ................
-000006b0: 82af e383 b3e6 95b0 292d da0c 7769 6e64  ........)-..wind
-000006c0: 6f77 5f74 6974 6c65 da0c 6275 7474 6f6e  ow_title..button
-000006d0: 5f63 6c6f 7365 da0b 7461 625f 6765 6e65  _close..tab_gene
-000006e0: 7261 6cda 1174 6162 5f65 6469 746f 725f  ral..tab_editor_
-000006f0: 636f 6e66 6967 da11 7461 625f 7669 6577  config..tab_view
-00000700: 6572 5f63 6f6e 6669 67da 0d74 6162 5f61  er_config..tab_a
-00000710: 695f 636f 6e66 6967 da18 6765 6e65 7261  i_config..genera
-00000720: 6c5f 6170 705f 636f 6e66 6967 5f6c 6162  l_app_config_lab
-00000730: 656c da1a 6765 6e65 7261 6c5f 6170 705f  el..general_app_
-00000740: 6c61 6e67 7561 6765 5f6c 6162 656c da2b  language_label.+
-00000750: 6765 6e65 7261 6c5f 6170 705f 6c61 6e67  general_app_lang
-00000760: 7561 6765 5f63 6f6d 626f 5f70 6c61 6365  uage_combo_place
-00000770: 686f 6c64 6572 5f74 6578 745a 3167 656e  holder_textZ1gen
-00000780: 6572 616c 5f61 7070 5f6c 616e 6775 6167  eral_app_languag
-00000790: 655f 636f 6d62 6f5f 6163 6365 7373 6962  e_combo_accessib
-000007a0: 6c65 5f64 6573 6372 6970 7469 6f6e da17  le_description..
-000007b0: 6765 6e65 7261 6c5f 6170 705f 7468 656d  general_app_them
-000007c0: 655f 6c61 6265 6cda 2867 656e 6572 616c  e_label.(general
-000007d0: 5f61 7070 5f74 6865 6d65 5f63 6f6d 626f  _app_theme_combo
-000007e0: 5f70 6c61 6365 686f 6c64 6572 5f74 6578  _placeholder_tex
-000007f0: 74da 2e67 656e 6572 616c 5f61 7070 5f74  t..general_app_t
-00000800: 6865 6d65 5f63 6f6d 626f 5f61 6363 6573  heme_combo_acces
-00000810: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000820: 6eda 1b67 656e 6572 616c 5f61 7070 5f6d  n..general_app_m
-00000830: 6169 6e5f 6d65 6e75 5f6c 6162 656c da1e  ain_menu_label..
-00000840: 6765 6e65 7261 6c5f 6170 705f 6d61 696e  general_app_main
-00000850: 5f6d 656e 755f 6368 6563 6b62 6f78 da35  _menu_checkbox.5
-00000860: 6765 6e65 7261 6c5f 6170 705f 6d61 696e  general_app_main
-00000870: 5f6d 656e 755f 6368 6563 6b62 6f78 5f61  _menu_checkbox_a
-00000880: 6363 6573 7369 626c 655f 6465 7363 7269  ccessible_descri
-00000890: 7074 696f 6eda 1b67 656e 6572 616c 5f61  ption..general_a
-000008a0: 7070 5f66 6f6e 745f 7369 7a65 5f6c 6162  pp_font_size_lab
-000008b0: 656c da33 6765 6e65 7261 6c5f 6170 705f  el.3general_app_
-000008c0: 666f 6e74 5f73 697a 655f 736c 6964 6572  font_size_slider
-000008d0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-000008e0: 7269 7074 696f 6eda 1767 656e 6572 616c  ription..general
-000008f0: 5f73 7461 7475 7362 6172 5f6c 6162 656c  _statusbar_label
-00000900: da36 6765 6e65 7261 6c5f 7374 6174 7573  .6general_status
-00000910: 6261 725f 7368 6f77 5f67 6c6f 6261 6c5f  bar_show_global_
-00000920: 6375 7273 6f72 5f70 6f73 6974 696f 6e5f  cursor_position_
-00000930: 6368 6563 6b62 6f78 da4d 6765 6e65 7261  checkbox.Mgenera
-00000940: 6c5f 7374 6174 7573 6261 725f 7368 6f77  l_statusbar_show
-00000950: 5f67 6c6f 6261 6c5f 6375 7273 6f72 5f70  _global_cursor_p
-00000960: 6f73 6974 696f 6e5f 6368 6563 6b62 6f78  osition_checkbox
-00000970: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-00000980: 7269 7074 696f 6eda 1365 6469 746f 725f  ription..editor_
-00000990: 636f 6e66 6967 5f6c 6162 656c da28 6564  config_label.(ed
-000009a0: 6974 6f72 5f63 6f6e 6669 675f 7368 6f77  itor_config_show
-000009b0: 5f6c 696e 655f 6e75 6d62 6572 735f 6368  _line_numbers_ch
-000009c0: 6563 6b62 6f78 da3f 6564 6974 6f72 5f63  eckbox.?editor_c
-000009d0: 6f6e 6669 675f 7368 6f77 5f6c 696e 655f  onfig_show_line_
-000009e0: 6e75 6d62 6572 735f 6368 6563 6b62 6f78  numbers_checkbox
-000009f0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
-00000a00: 7269 7074 696f 6eda 1376 6965 7765 725f  ription..viewer_
-00000a10: 636f 6e66 6967 5f6c 6162 656c da25 7669  config_label.%vi
-00000a20: 6577 6572 5f63 6f6e 6669 675f 7072 6f63  ewer_config_proc
-00000a30: 6573 735f 656d 6f6a 6973 5f63 6865 636b  ess_emojis_check
-00000a40: 626f 78da 3c76 6965 7765 725f 636f 6e66  box.<viewer_conf
-00000a50: 6967 5f70 726f 6365 7373 5f65 6d6f 6a69  ig_process_emoji
-00000a60: 735f 6368 6563 6b62 6f78 5f61 6363 6573  s_checkbox_acces
-00000a70: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000a80: 6eda 2676 6965 7765 725f 636f 6e66 6967  n.&viewer_config
-00000a90: 5f68 6967 686c 6967 6874 5f74 6f64 6f73  _highlight_todos
-00000aa0: 5f63 6865 636b 626f 78da 3d76 6965 7765  _checkbox.=viewe
-00000ab0: 725f 636f 6e66 6967 5f68 6967 686c 6967  r_config_highlig
-00000ac0: 6874 5f74 6f64 6f73 5f63 6865 636b 626f  ht_todos_checkbo
-00000ad0: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
-00000ae0: 6372 6970 7469 6f6e da2d 7669 6577 6572  cription.-viewer
-00000af0: 5f63 6f6e 6669 675f 6f70 656e 5f6c 696e  _config_open_lin
-00000b00: 6b5f 636f 6e66 6972 6d61 7469 6f6e 5f63  k_confirmation_c
-00000b10: 6865 636b 626f 78da 4476 6965 7765 725f  heckbox.Dviewer_
-00000b20: 636f 6e66 6967 5f6f 7065 6e5f 6c69 6e6b  config_open_link
-00000b30: 5f63 6f6e 6669 726d 6174 696f 6e5f 6368  _confirmation_ch
-00000b40: 6563 6b62 6f78 5f61 6363 6573 7369 626c  eckbox_accessibl
-00000b50: 655f 6465 7363 7269 7074 696f 6eda 1a61  e_description..a
-00000b60: 695f 636f 6e66 6967 5f6f 7065 6e61 695f  i_config_openai_
-00000b70: 6170 695f 6c61 6265 6cda 2f61 695f 636f  api_label./ai_co
-00000b80: 6e66 6967 5f6f 7065 6e61 695f 6170 695f  nfig_openai_api_
-00000b90: 7572 6c5f 696e 7075 745f 706c 6163 6568  url_input_placeh
-00000ba0: 6f6c 6465 725f 7465 7874 da35 6169 5f63  older_text.5ai_c
-00000bb0: 6f6e 6669 675f 6f70 656e 6169 5f61 7069  onfig_openai_api
-00000bc0: 5f75 726c 5f69 6e70 7574 5f61 6363 6573  _url_input_acces
-00000bd0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000be0: 6eda 2f61 695f 636f 6e66 6967 5f6f 7065  n./ai_config_ope
-00000bf0: 6e61 695f 6170 695f 6b65 795f 696e 7075  nai_api_key_inpu
-00000c00: 745f 706c 6163 6568 6f6c 6465 725f 7465  t_placeholder_te
-00000c10: 7874 da35 6169 5f63 6f6e 6669 675f 6f70  xt.5ai_config_op
-00000c20: 656e 6169 5f61 7069 5f6b 6579 5f69 6e70  enai_api_key_inp
-00000c30: 7574 5f61 6363 6573 7369 626c 655f 6465  ut_accessible_de
-00000c40: 7363 7269 7074 696f 6eda 2b61 695f 636f  scription.+ai_co
-00000c50: 6e66 6967 5f6f 7065 6e61 695f 6170 695f  nfig_openai_api_
-00000c60: 7375 7070 6f72 7465 645f 6d6f 6465 6c73  supported_models
-00000c70: 5f6c 6162 656c da2f 6169 5f63 6f6e 6669  _label./ai_confi
-00000c80: 675f 6169 5f6d 6f64 656c 5f6e 616d 6573  g_ai_model_names
-00000c90: 5f63 6f6d 626f 5f70 6c61 6365 686f 6c64  _combo_placehold
-00000ca0: 6572 5f74 6578 74da 3561 695f 636f 6e66  er_text.5ai_conf
-00000cb0: 6967 5f61 695f 6d6f 6465 6c5f 6e61 6d65  ig_ai_model_name
-00000cc0: 735f 636f 6d62 6f5f 6163 6365 7373 6962  s_combo_accessib
-00000cd0: 6c65 5f64 6573 6372 6970 7469 6f6e da14  le_description..
-00000ce0: 6169 5f63 6f6e 6669 675f 6261 7365 5f6c  ai_config_base_l
-00000cf0: 6162 656c da22 6169 5f63 6f6e 6669 675f  abel."ai_config_
-00000d00: 6261 7365 5f73 7973 7465 6d5f 7072 6f6d  base_system_prom
-00000d10: 7074 5f6c 6162 656c da32 6169 5f63 6f6e  pt_label.2ai_con
-00000d20: 6669 675f 6261 7365 5f73 7973 7465 6d5f  fig_base_system_
-00000d30: 7072 6f6d 7074 5f65 6469 745f 706c 6163  prompt_edit_plac
-00000d40: 6568 6f6c 6465 725f 7465 7874 da38 6169  eholder_text.8ai
-00000d50: 5f63 6f6e 6669 675f 6261 7365 5f73 7973  _config_base_sys
-00000d60: 7465 6d5f 7072 6f6d 7074 5f65 6469 745f  tem_prompt_edit_
-00000d70: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
-00000d80: 6970 7469 6f6e da28 6169 5f63 6f6e 6669  iption.(ai_confi
-00000d90: 675f 6261 7365 5f72 6573 706f 6e73 655f  g_base_response_
-00000da0: 6d61 785f 746f 6b65 6e73 5f6c 6162 656c  max_tokens_label
-00000db0: da3f 6169 5f63 6f6e 6669 675f 6261 7365  .?ai_config_base
-00000dc0: 5f72 6573 706f 6e73 655f 6d61 785f 746f  _response_max_to
-00000dd0: 6b65 6e73 5f69 6e70 7574 5f61 6363 6573  kens_input_acces
-00000de0: 7369 626c 655f 6465 7363 7269 7074 696f  sible_descriptio
-00000df0: 6e4e 2901 da07 6c65 7865 6d65 73a9 0072  nN)...lexemes..r
-00000e00: 2e00 0000 722e 0000 00fa 4c2f 5573 6572  ....r.....L/User
-00000e10: 732f 7661 6469 6b75 732f 5079 6368 6172  s/vadikus/Pychar
-00000e20: 6d50 726f 6a65 6374 732f 6e6f 746f 6c6f  mProjects/notolo
-00000e30: 672f 6e6f 746f 6c6f 672f 6c65 7865 6d65  g/notolog/lexeme
-00000e40: 732f 6a61 2f73 6574 7469 6e67 735f 6469  s/ja/settings_di
-00000e50: 616c 6f67 2e70 79da 083c 6d6f 6475 6c65  alog.py..<module
-00000e60: 3e04 0000 0073 5a00 0000 0202 0202 0201  >....sZ.........
-00000e70: 0201 0201 0202 0201 0201 0201 0201 0201  ................
-00000e80: 0201 0201 0201 0201 0201 0201 0202 0201  ................
-00000e90: 0202 0202 0201 0201 0202 0201 0201 0201  ................
-00000ea0: 0201 0201 0202 0203 0201 0201 0201 0201  ................
-00000eb0: 0201 0201 0201 0202 0201 0201 0202 0201  ................
-00000ec0: 0201 02c6                                ....
+00000080: 6429 642a 642b 642c 642d 642e 642f 9c2f  d)d*d+d,d-d.d/./
+00000090: 5a00 6430 5300 2931 7506 0000 00e8 a8ad  Z.d0S.)1u.......
+000000a0: e5ae 9a75 0900 0000 e996 89e3 8198 e382  ...u............
+000000b0: 8b75 0600 0000 e4b8 80e8 88ac 750f 0000  .u..........u...
+000000c0: 00e3 82a8 e383 87e3 82a3 e382 bfe3 83bc  ................
+000000d0: 750c 0000 00e3 8393 e383 a5e3 83bc e382  u...............
+000000e0: a275 0900 0000 4149 20e8 a8ad e5ae 9a75  .u....AI ......u
+000000f0: 0f00 0000 e382 a2e3 8397 e383 aae8 a8ad  ................
+00000100: e5ae 9a75 0600 0000 e8a8 80e8 aa9e 750f  ...u..........u.
+00000110: 0000 00e8 a880 e8aa 9ee3 8292 e981 b8e6  ................
+00000120: 8a9e 752a 0000 00e3 82a2 e383 97e3 83aa  ..u*............
+00000130: e381 aee3 82a4 e383 b3e3 82bf e383 bce3  ................
+00000140: 8395 e382 a7e3 83bc e382 b9e8 a880 e8aa  ................
+00000150: 9e75 0900 0000 e383 86e3 83bc e383 9e75  .u.............u
+00000160: 1200 0000 e383 86e3 83bc e383 9ee3 8292  ................
+00000170: e981 b8e6 8a9e 752d 0000 00e3 82a2 e383  ......u-........
+00000180: 97e3 83aa e381 aee3 82a4 e383 b3e3 82bf  ................
+00000190: e383 bce3 8395 e382 a7e3 83bc e382 b9e3  ................
+000001a0: 8386 e383 bce3 839e 7515 0000 00e3 83a1  ........u.......
+000001b0: e382 a4e3 83b3 e383 a1e3 838b e383 a5e3  ................
+000001c0: 83bc 751e 0000 00e3 83a1 e382 a4e3 83b3  ..u.............
+000001d0: e383 a1e3 838b e383 a5e3 83bc e382 92e8  ................
+000001e0: a1a8 e7a4 ba75 3f00 0000 e382 a2e3 8397  .....u?.........
+000001f0: e383 aae3 81ae e383 a1e3 82a4 e383 b3e3  ................
+00000200: 8389 e383 ade3 8383 e383 97e3 8380 e382  ................
+00000210: a6e3 83b3 e383 a1e3 838b e383 a5e3 83bc  ................
+00000220: e382 92e8 a1a8 e7a4 ba75 2000 0000 e383  .........u .....
+00000230: 95e3 82a9 e383 b3e3 8388 e382 b5e3 82a4  ................
+00000240: e382 baef bc9a 7b73 697a 657d 7074 753c  ......{size}ptu<
+00000250: 0000 00e3 82a2 e383 97e3 83aa e381 aee5  ................
+00000260: 85a8 e4bd 93e7 9a84 e381 aae3 8395 e382  ................
+00000270: a9e3 83b3 e383 88e3 82b5 e382 a4e3 82ba  ................
+00000280: e382 92e8 aabf e695 b4e3 8199 e382 8b75  ...............u
+00000290: 1500 0000 e382 b9e3 8386 e383 bce3 82bf  ................
+000002a0: e382 b9e3 8390 e383 bc75 2a00 0000 e382  .........u*.....
+000002b0: b0e3 83ad e383 bce3 8390 e383 abe3 82ab  ................
+000002c0: e383 bce3 82bd e383 abe4 bd8d e7bd aee3  ................
+000002d0: 8292 e8a1 a8e7 a4ba 7548 0000 00e3 82b9  ........uH......
+000002e0: e383 86e3 83bc e382 bfe3 82b9 e383 90e3  ................
+000002f0: 83bc e381 abe3 82b0 e383 ade3 83bc e383  ................
+00000300: 90e3 83ab e382 abe3 83bc e382 bde3 83ab  ................
+00000310: e4bd 8de7 bdae e382 92e8 a1a8 e7a4 bae3  ................
+00000320: 8199 e382 8b75 1200 0000 e382 a8e3 8387  .....u..........
+00000330: e382 a3e3 82bf e8a8 ade5 ae9a 7512 0000  ............u...
+00000340: 00e8 a18c e795 aae5 8fb7 e382 92e8 a1a8  ................
+00000350: e7a4 ba75 2a00 0000 e382 a8e3 8387 e382  ...u*...........
+00000360: a3e3 82bf e586 85e3 81a7 e8a1 8ce7 95aa  ................
+00000370: e58f b7e3 8292 e8a1 a8e7 a4ba e381 99e3  ................
+00000380: 828b 7512 0000 00e3 8393 e383 a5e3 83bc  ..u.............
+00000390: e383 afe8 a8ad e5ae 9a75 3300 0000 e383  .........u3.....
+000003a0: 86e3 82ad e382 b9e3 8388 e7b5 b5e6 9687  ................
+000003b0: e5ad 97e3 8292 e382 b0e3 83a9 e383 95e3  ................
+000003c0: 82a3 e383 83e3 82af e381 abe5 a489 e68f  ................
+000003d0: 9b75 4200 0000 e383 86e3 82ad e382 b9e3  .uB.............
+000003e0: 8388 e7b5 b5e6 9687 e5ad 97e3 8292 e382  ................
+000003f0: b0e3 83a9 e383 95e3 82a3 e382 abe3 83ab  ................
+00000400: e381 aae8 a1a8 e78f bee3 81ab e5a4 89e6  ................
+00000410: 8f9b e381 99e3 828b 7516 0000 0054 4f44  ........u....TOD
+00000420: 4fe3 8292 e383 8fe3 82a4 e383 a9e3 82a4  O...............
+00000430: e383 8875 3100 0000 e383 86e3 82ad e382  ...u1...........
+00000440: b9e3 8388 e586 85e3 81ae 544f 444f e382  ..........TODO..
+00000450: bfe3 82b0 e382 92e5 bcb7 e8aa bfe8 a1a8  ................
+00000460: e7a4 bae3 8199 e382 8b75 2400 0000 e383  .........u$.....
+00000470: aae3 83b3 e382 afe9 968b e381 8fe5 898d  ................
+00000480: e381 abe7 a2ba e8aa 8de3 818c e5bf 85e8  ................
+00000490: a681 752a 0000 00e3 83aa e383 b3e3 82af  ..u*............
+000004a0: e382 92e9 968b e381 8fe5 898d e381 abe7  ................
+000004b0: a2ba e8aa 8de3 8292 e6b1 82e3 8281 e382  ................
+000004c0: 8b75 2a00 0000 e5a4 96e9 83a8 e794 bbe5  .u*.............
+000004d0: 838f e382 92e3 8387 e382 a3e3 82b9 e382  ................
+000004e0: afe3 81ab e887 aae5 8b95 e4bf 9de5 ad98  ................
+000004f0: 7569 0000 00e3 82aa e383 95e3 83a9 e382  ui..............
+00000500: a4e3 83b3 e382 a2e3 82af e382 bbe3 82b9  ................
+00000510: e381 aee3 819f e382 81e3 81ab e5a4 96e9  ................
+00000520: 83a8 e794 bbe5 838f e381 aee3 82b3 e383  ................
+00000530: 94e3 83bc e382 92e3 8387 e382 a3e3 82b9  ................
+00000540: e382 afe3 81ab e887 aae5 8b95 e4bf 9de5  ................
+00000550: ad98 e381 97e3 81be e381 99e3 8082 7a0a  ..............z.
+00000560: 4f70 656e 4149 2041 5049 7a07 4150 4920  OpenAI APIz.API 
+00000570: 5552 4c75 1000 0000 4f70 656e 4149 2041  URLu....OpenAI A
+00000580: 5049 e381 ae55 524c 750a 0000 0041 5049  PI...URLu....API
+00000590: 20e3 82ad e383 bc75 1300 0000 4f70 656e   ......u....Open
+000005a0: 4149 2041 5049 e381 aee3 82ad e383 bc75  AI API.........u
+000005b0: 2400 0000 e382 b5e3 839d e383 bce3 8388  $...............
+000005c0: e381 95e3 828c e381 a6e3 8184 e382 8be3  ................
+000005d0: 83a2 e383 87e3 83ab 7512 0000 00e3 83a2  ........u.......
+000005e0: e383 87e3 83ab e382 92e9 81b8 e68a 9e75  ...............u
+000005f0: 3300 0000 e981 b8e6 8a9e e58f afe8 83bd  3...............
+00000600: e381 aae3 82b5 e383 9de3 83bc e383 88e3  ................
+00000610: 8195 e382 8ce3 81a6 e381 84e3 828b e383  ................
+00000620: a2e3 8387 e383 ab75 1500 0000 e59f bae6  .......u........
+00000630: 9cac e383 91e3 83a9 e383 a1e3 83bc e382  ................
+00000640: bf75 1b00 0000 e382 b7e3 82b9 e383 86e3  .u..............
+00000650: 83a0 e383 97e3 83ad e383 b3e3 8397 e383  ................
+00000660: 8875 3f00 0000 e590 84e3 83aa e382 afe3  .u?.............
+00000670: 82a8 e382 b9e3 8388 e381 abe5 8588 e7ab  ................
+00000680: 8be3 81a4 e59f bae6 9cac e382 b7e3 82b9  ................
+00000690: e383 86e3 83a0 e383 97e3 83ad e383 b3e3  ................
+000006a0: 8397 e383 8875 5d00 0000 e590 84e3 83aa  .....u].........
+000006b0: e382 afe3 82a8 e382 b9e3 8388 e381 abe5  ................
+000006c0: 8588 e7ab 8be3 81a4 e59f bae6 9cac e382  ................
+000006d0: b7e3 82b9 e383 86e3 83a0 e383 97e3 83ad  ................
+000006e0: e383 b3e3 8397 e383 88e3 8082 e383 97e3  ................
+000006f0: 83ac e383 bce3 83b3 e383 86e3 82ad e382  ................
+00000700: b9e3 8388 e380 8275 1e00 0000 e5bf 9ce7  .......u........
+00000710: ad94 e381 aee6 9c80 e5a4 a7e3 8388 e383  ................
+00000720: bce3 82af e383 b3e6 95b0 752a 0000 00e5  ..........u*....
+00000730: bf9c e7ad 94e3 81a7 e58f 97e3 8191 e58f  ................
+00000740: 96e3 828b e69c 80e5 a4a7 e383 88e3 83bc  ................
+00000750: e382 afe3 83b3 e695 b029 2fda 0c77 696e  .........)/..win
+00000760: 646f 775f 7469 746c 65da 0c62 7574 746f  dow_title..butto
+00000770: 6e5f 636c 6f73 65da 0b74 6162 5f67 656e  n_close..tab_gen
+00000780: 6572 616c da11 7461 625f 6564 6974 6f72  eral..tab_editor
+00000790: 5f63 6f6e 6669 67da 1174 6162 5f76 6965  _config..tab_vie
+000007a0: 7765 725f 636f 6e66 6967 da0d 7461 625f  wer_config..tab_
+000007b0: 6169 5f63 6f6e 6669 67da 1867 656e 6572  ai_config..gener
+000007c0: 616c 5f61 7070 5f63 6f6e 6669 675f 6c61  al_app_config_la
+000007d0: 6265 6cda 1a67 656e 6572 616c 5f61 7070  bel..general_app
+000007e0: 5f6c 616e 6775 6167 655f 6c61 6265 6cda  _language_label.
+000007f0: 2b67 656e 6572 616c 5f61 7070 5f6c 616e  +general_app_lan
+00000800: 6775 6167 655f 636f 6d62 6f5f 706c 6163  guage_combo_plac
+00000810: 6568 6f6c 6465 725f 7465 7874 5a31 6765  eholder_textZ1ge
+00000820: 6e65 7261 6c5f 6170 705f 6c61 6e67 7561  neral_app_langua
+00000830: 6765 5f63 6f6d 626f 5f61 6363 6573 7369  ge_combo_accessi
+00000840: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
+00000850: 1767 656e 6572 616c 5f61 7070 5f74 6865  .general_app_the
+00000860: 6d65 5f6c 6162 656c da28 6765 6e65 7261  me_label.(genera
+00000870: 6c5f 6170 705f 7468 656d 655f 636f 6d62  l_app_theme_comb
+00000880: 6f5f 706c 6163 6568 6f6c 6465 725f 7465  o_placeholder_te
+00000890: 7874 da2e 6765 6e65 7261 6c5f 6170 705f  xt..general_app_
+000008a0: 7468 656d 655f 636f 6d62 6f5f 6163 6365  theme_combo_acce
+000008b0: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+000008c0: 6f6e da1b 6765 6e65 7261 6c5f 6170 705f  on..general_app_
+000008d0: 6d61 696e 5f6d 656e 755f 6c61 6265 6cda  main_menu_label.
+000008e0: 1e67 656e 6572 616c 5f61 7070 5f6d 6169  .general_app_mai
+000008f0: 6e5f 6d65 6e75 5f63 6865 636b 626f 78da  n_menu_checkbox.
+00000900: 3567 656e 6572 616c 5f61 7070 5f6d 6169  5general_app_mai
+00000910: 6e5f 6d65 6e75 5f63 6865 636b 626f 785f  n_menu_checkbox_
+00000920: 6163 6365 7373 6962 6c65 5f64 6573 6372  accessible_descr
+00000930: 6970 7469 6f6e da1b 6765 6e65 7261 6c5f  iption..general_
+00000940: 6170 705f 666f 6e74 5f73 697a 655f 6c61  app_font_size_la
+00000950: 6265 6cda 3367 656e 6572 616c 5f61 7070  bel.3general_app
+00000960: 5f66 6f6e 745f 7369 7a65 5f73 6c69 6465  _font_size_slide
+00000970: 725f 6163 6365 7373 6962 6c65 5f64 6573  r_accessible_des
+00000980: 6372 6970 7469 6f6e da17 6765 6e65 7261  cription..genera
+00000990: 6c5f 7374 6174 7573 6261 725f 6c61 6265  l_statusbar_labe
+000009a0: 6cda 3667 656e 6572 616c 5f73 7461 7475  l.6general_statu
+000009b0: 7362 6172 5f73 686f 775f 676c 6f62 616c  sbar_show_global
+000009c0: 5f63 7572 736f 725f 706f 7369 7469 6f6e  _cursor_position
+000009d0: 5f63 6865 636b 626f 78da 4d67 656e 6572  _checkbox.Mgener
+000009e0: 616c 5f73 7461 7475 7362 6172 5f73 686f  al_statusbar_sho
+000009f0: 775f 676c 6f62 616c 5f63 7572 736f 725f  w_global_cursor_
+00000a00: 706f 7369 7469 6f6e 5f63 6865 636b 626f  position_checkbo
+00000a10: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
+00000a20: 6372 6970 7469 6f6e da13 6564 6974 6f72  cription..editor
+00000a30: 5f63 6f6e 6669 675f 6c61 6265 6cda 2865  _config_label.(e
+00000a40: 6469 746f 725f 636f 6e66 6967 5f73 686f  ditor_config_sho
+00000a50: 775f 6c69 6e65 5f6e 756d 6265 7273 5f63  w_line_numbers_c
+00000a60: 6865 636b 626f 78da 3f65 6469 746f 725f  heckbox.?editor_
+00000a70: 636f 6e66 6967 5f73 686f 775f 6c69 6e65  config_show_line
+00000a80: 5f6e 756d 6265 7273 5f63 6865 636b 626f  _numbers_checkbo
+00000a90: 785f 6163 6365 7373 6962 6c65 5f64 6573  x_accessible_des
+00000aa0: 6372 6970 7469 6f6e da13 7669 6577 6572  cription..viewer
+00000ab0: 5f63 6f6e 6669 675f 6c61 6265 6cda 2576  _config_label.%v
+00000ac0: 6965 7765 725f 636f 6e66 6967 5f70 726f  iewer_config_pro
+00000ad0: 6365 7373 5f65 6d6f 6a69 735f 6368 6563  cess_emojis_chec
+00000ae0: 6b62 6f78 da3c 7669 6577 6572 5f63 6f6e  kbox.<viewer_con
+00000af0: 6669 675f 7072 6f63 6573 735f 656d 6f6a  fig_process_emoj
+00000b00: 6973 5f63 6865 636b 626f 785f 6163 6365  is_checkbox_acce
+00000b10: 7373 6962 6c65 5f64 6573 6372 6970 7469  ssible_descripti
+00000b20: 6f6e da26 7669 6577 6572 5f63 6f6e 6669  on.&viewer_confi
+00000b30: 675f 6869 6768 6c69 6768 745f 746f 646f  g_highlight_todo
+00000b40: 735f 6368 6563 6b62 6f78 da3d 7669 6577  s_checkbox.=view
+00000b50: 6572 5f63 6f6e 6669 675f 6869 6768 6c69  er_config_highli
+00000b60: 6768 745f 746f 646f 735f 6368 6563 6b62  ght_todos_checkb
+00000b70: 6f78 5f61 6363 6573 7369 626c 655f 6465  ox_accessible_de
+00000b80: 7363 7269 7074 696f 6eda 2d76 6965 7765  scription.-viewe
+00000b90: 725f 636f 6e66 6967 5f6f 7065 6e5f 6c69  r_config_open_li
+00000ba0: 6e6b 5f63 6f6e 6669 726d 6174 696f 6e5f  nk_confirmation_
+00000bb0: 6368 6563 6b62 6f78 da44 7669 6577 6572  checkbox.Dviewer
+00000bc0: 5f63 6f6e 6669 675f 6f70 656e 5f6c 696e  _config_open_lin
+00000bd0: 6b5f 636f 6e66 6972 6d61 7469 6f6e 5f63  k_confirmation_c
+00000be0: 6865 636b 626f 785f 6163 6365 7373 6962  heckbox_accessib
+00000bf0: 6c65 5f64 6573 6372 6970 7469 6f6e da25  le_description.%
+00000c00: 7669 6577 6572 5f63 6f6e 6669 675f 7361  viewer_config_sa
+00000c10: 7665 5f72 6573 6f75 7263 6573 5f63 6865  ve_resources_che
+00000c20: 636b 626f 78da 3c76 6965 7765 725f 636f  ckbox.<viewer_co
+00000c30: 6e66 6967 5f73 6176 655f 7265 736f 7572  nfig_save_resour
+00000c40: 6365 735f 6368 6563 6b62 6f78 5f61 6363  ces_checkbox_acc
+00000c50: 6573 7369 626c 655f 6465 7363 7269 7074  essible_descript
+00000c60: 696f 6eda 1a61 695f 636f 6e66 6967 5f6f  ion..ai_config_o
+00000c70: 7065 6e61 695f 6170 695f 6c61 6265 6cda  penai_api_label.
+00000c80: 2f61 695f 636f 6e66 6967 5f6f 7065 6e61  /ai_config_opena
+00000c90: 695f 6170 695f 7572 6c5f 696e 7075 745f  i_api_url_input_
+00000ca0: 706c 6163 6568 6f6c 6465 725f 7465 7874  placeholder_text
+00000cb0: da35 6169 5f63 6f6e 6669 675f 6f70 656e  .5ai_config_open
+00000cc0: 6169 5f61 7069 5f75 726c 5f69 6e70 7574  ai_api_url_input
+00000cd0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
+00000ce0: 7269 7074 696f 6eda 2f61 695f 636f 6e66  ription./ai_conf
+00000cf0: 6967 5f6f 7065 6e61 695f 6170 695f 6b65  ig_openai_api_ke
+00000d00: 795f 696e 7075 745f 706c 6163 6568 6f6c  y_input_placehol
+00000d10: 6465 725f 7465 7874 da35 6169 5f63 6f6e  der_text.5ai_con
+00000d20: 6669 675f 6f70 656e 6169 5f61 7069 5f6b  fig_openai_api_k
+00000d30: 6579 5f69 6e70 7574 5f61 6363 6573 7369  ey_input_accessi
+00000d40: 626c 655f 6465 7363 7269 7074 696f 6eda  ble_description.
+00000d50: 2b61 695f 636f 6e66 6967 5f6f 7065 6e61  +ai_config_opena
+00000d60: 695f 6170 695f 7375 7070 6f72 7465 645f  i_api_supported_
+00000d70: 6d6f 6465 6c73 5f6c 6162 656c da2f 6169  models_label./ai
+00000d80: 5f63 6f6e 6669 675f 6169 5f6d 6f64 656c  _config_ai_model
+00000d90: 5f6e 616d 6573 5f63 6f6d 626f 5f70 6c61  _names_combo_pla
+00000da0: 6365 686f 6c64 6572 5f74 6578 74da 3561  ceholder_text.5a
+00000db0: 695f 636f 6e66 6967 5f61 695f 6d6f 6465  i_config_ai_mode
+00000dc0: 6c5f 6e61 6d65 735f 636f 6d62 6f5f 6163  l_names_combo_ac
+00000dd0: 6365 7373 6962 6c65 5f64 6573 6372 6970  cessible_descrip
+00000de0: 7469 6f6e da14 6169 5f63 6f6e 6669 675f  tion..ai_config_
+00000df0: 6261 7365 5f6c 6162 656c da22 6169 5f63  base_label."ai_c
+00000e00: 6f6e 6669 675f 6261 7365 5f73 7973 7465  onfig_base_syste
+00000e10: 6d5f 7072 6f6d 7074 5f6c 6162 656c da32  m_prompt_label.2
+00000e20: 6169 5f63 6f6e 6669 675f 6261 7365 5f73  ai_config_base_s
+00000e30: 7973 7465 6d5f 7072 6f6d 7074 5f65 6469  ystem_prompt_edi
+00000e40: 745f 706c 6163 6568 6f6c 6465 725f 7465  t_placeholder_te
+00000e50: 7874 da38 6169 5f63 6f6e 6669 675f 6261  xt.8ai_config_ba
+00000e60: 7365 5f73 7973 7465 6d5f 7072 6f6d 7074  se_system_prompt
+00000e70: 5f65 6469 745f 6163 6365 7373 6962 6c65  _edit_accessible
+00000e80: 5f64 6573 6372 6970 7469 6f6e da28 6169  _description.(ai
+00000e90: 5f63 6f6e 6669 675f 6261 7365 5f72 6573  _config_base_res
+00000ea0: 706f 6e73 655f 6d61 785f 746f 6b65 6e73  ponse_max_tokens
+00000eb0: 5f6c 6162 656c da3f 6169 5f63 6f6e 6669  _label.?ai_confi
+00000ec0: 675f 6261 7365 5f72 6573 706f 6e73 655f  g_base_response_
+00000ed0: 6d61 785f 746f 6b65 6e73 5f69 6e70 7574  max_tokens_input
+00000ee0: 5f61 6363 6573 7369 626c 655f 6465 7363  _accessible_desc
+00000ef0: 7269 7074 696f 6e4e 2901 da07 6c65 7865  riptionN)...lexe
+00000f00: 6d65 73a9 0072 3000 0000 7230 0000 00fa  mes..r0...r0....
+00000f10: 4c2f 5573 6572 732f 7661 6469 6b75 732f  L/Users/vadikus/
+00000f20: 5079 6368 6172 6d50 726f 6a65 6374 732f  PycharmProjects/
+00000f30: 6e6f 746f 6c6f 672d 6465 762f 6170 702f  notolog-dev/app/
+00000f40: 6c65 7865 6d65 732f 6a61 2f73 6574 7469  lexemes/ja/setti
+00000f50: 6e67 735f 6469 616c 6f67 2e70 79da 083c  ngs_dialog.py..<
+00000f60: 6d6f 6475 6c65 3e04 0000 0073 5e00 0000  module>....s^...
+00000f70: 0202 0202 0201 0201 0201 0202 0201 0201  ................
+00000f80: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+00000f90: 0201 0202 0201 0202 0202 0201 0201 0202  ................
+00000fa0: 0201 0201 0201 0201 0201 0201 0201 0202  ................
+00000fb0: 0202 0201 0201 0201 0201 0201 0201 0201  ................
+00000fc0: 0202 0201 0201 0202 0201 0201 02c5       ..............
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/statusbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 1242 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 da04 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 da04 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0012 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
 00000040: 6409 640a 640b 640c 640d 640e 640f 6410  d.d.d.d.d.d.d.d.
 00000050: 6411 9c11 5a00 6412 5300 2913 7509 0000  d...Z.d.S.).u...
 00000060: 00e3 8194 e381 bfe7 aeb1 751b 0000 00e3  ..........u.....
 00000070: 8194 e381 bfe7 aeb1 e381 aee5 8685 e5ae  ................
@@ -70,13 +70,13 @@
 00000450: 6261 6cda 2b73 7461 7475 7362 6172 5f63  bal.+statusbar_c
 00000460: 7572 736f 725f 6c61 6265 6c5f 7365 6c65  ursor_label_sele
 00000470: 6374 6564 5f77 6974 685f 676c 6f62 616c  cted_with_global
 00000480: 4e29 01da 076c 6578 656d 6573 a900 720e  N)...lexemes..r.
 00000490: 0000 0072 0e00 0000 fa46 2f55 7365 7273  ...r.....F/Users
 000004a0: 2f76 6164 696b 7573 2f50 7963 6861 726d  /vadikus/Pycharm
 000004b0: 5072 6f6a 6563 7473 2f6e 6f74 6f6c 6f67  Projects/notolog
-000004c0: 2f6e 6f74 6f6c 6f67 2f6c 6578 656d 6573  /notolog/lexemes
+000004c0: 2d64 6576 2f61 7070 2f6c 6578 656d 6573  -dev/app/lexemes
 000004d0: 2f6a 612f 7374 6174 7573 6261 722e 7079  /ja/statusbar.py
 000004e0: da08 3c6d 6f64 756c 653e 0300 0000 7322  ..<module>....s"
 000004f0: 0000 0002 0102 0202 0102 0102 0202 0102  ................
 00000500: 0102 0202 0102 0202 0102 0102 0202 0102  ................
 00000510: 0102 0102 ea                             .....
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc` & `notolog-0.9.0b11/app/lexemes/ja/__pycache__/toolbar.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr 28 21:48:23 2024 UTC, .py size: 3000 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 27c4 2e66 b80b 0000  a.......'..f....
+00000000: 610d 0d0a 0000 0000 020f 3066 b80b 0000  a.........0f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0032 0000 0040 0000 0073 6c00 0000 6400  .2...@...sl...d.
 00000030: 6400 6401 6402 6403 6404 6405 6406 6407  d.d.d.d.d.d.d.d.
 00000040: 6408 6409 640a 640b 640c 640d 640e 640f  d.d.d.d.d.d.d.d.
 00000050: 6410 6411 6412 6413 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
 00000060: 6418 6419 641a 641b 641c 641d 641e 641f  d.d.d.d.d.d.d.d.
 00000070: 6420 6421 6422 6423 6424 6425 6426 6427  d d!d"d#d$d%d&d'
@@ -175,15 +175,15 @@
 00000ae0: 7874 da15 7365 6172 6368 5f63 6173 655f  xt..search_case_
 00000af0: 7365 6e73 6974 6976 65da 1973 6561 7263  sensitive..searc
 00000b00: 685f 6d61 7463 685f 6361 7365 5f74 6f6f  h_match_case_too
 00000b10: 6c74 6970 4e29 01da 076c 6578 656d 6573  ltipN)...lexemes
 00000b20: a900 722f 0000 0072 2f00 0000 fa44 2f55  ..r/...r/....D/U
 00000b30: 7365 7273 2f76 6164 696b 7573 2f50 7963  sers/vadikus/Pyc
 00000b40: 6861 726d 5072 6f6a 6563 7473 2f6e 6f74  harmProjects/not
-00000b50: 6f6c 6f67 2f6e 6f74 6f6c 6f67 2f6c 6578  olog/notolog/lex
+00000b50: 6f6c 6f67 2d64 6576 2f61 7070 2f6c 6578  olog-dev/app/lex
 00000b60: 656d 6573 2f6a 612f 746f 6f6c 6261 722e  emes/ja/toolbar.
 00000b70: 7079 da08 3c6d 6f64 756c 653e 0300 0000  py..<module>....
 00000b80: 7362 0000 0002 0102 0102 0102 0102 0102  sb..............
 00000b90: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000ba0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000bb0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000bc0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/ja/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/ja/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/common.py` & `notolog-0.9.0b11/app/lexemes/ja/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "アプリ情報",
     "popup_about_app_name_description": "Markdown エディタ",
 
     "popup_about_version": "バージョン",
     "popup_about_license": "ライセンス",
     "popup_about_website": "ウェブサイト",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "日付",
 
     "update_helper_new_version_is_available": "アプリの新しいバージョン '{latest_version}' が利用可能です",
     "update_helper_latest_version_installed": "アプリの最新バージョンがインストールされています",
 
     "network_connection_error_empty": "応答情報を取得できません",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/ja/main_menu.py` & `notolog-0.9.0b11/app/lexemes/ja/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/statusbar.py` & `notolog-0.9.0b11/app/lexemes/ja/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ja/toolbar.py` & `notolog-0.9.0b11/app/lexemes/ja/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/ko/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/ko/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/common.py` & `notolog-0.9.0b11/app/lexemes/ko/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "애플리케이션 정보",
     "popup_about_app_name_description": "마크다운 에디터",
 
     "popup_about_version": "버전",
     "popup_about_license": "라이선스",
     "popup_about_website": "웹사이트",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "날짜",
 
     "update_helper_new_version_is_available": "앱의 새 버전 '{latest_version}'이(가) 사용 가능합니다",
     "update_helper_latest_version_installed": "앱의 최신 버전이 설치되었습니다",
 
     "network_connection_error_empty": "응답 정보를 가져올 수 없습니다",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/ko/main_menu.py` & `notolog-0.9.0b11/app/lexemes/ko/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/ko/settings_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,17 @@
     "viewer_config_process_emojis_checkbox": "텍스트 이모지를 그래픽으로 변환",
     "viewer_config_process_emojis_checkbox_accessible_description": "텍스트 이모지를 그래픽 표현으로 변환",
     "viewer_config_highlight_todos_checkbox": "할 일 하이라이트",
     "viewer_config_highlight_todos_checkbox_accessible_description": "텍스트 내 할 일 태그 강조",
     "viewer_config_open_link_confirmation_checkbox": "링크 열기 전 확인 요구",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "링크를 열기 전에 확인 요청",
+    "viewer_config_save_resources_checkbox": "외부 이미지를 디스크에 자동 저장",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "오프라인 액세스를 위해 외부 이미지의 복사본을 디스크에 자동으로 저장합니다.",
 
     "ai_config_openai_api_label": "OpenAI API",
     "ai_config_openai_api_url_input_placeholder_text": "API URL",
     "ai_config_openai_api_url_input_accessible_description": "OpenAI API URL",
     "ai_config_openai_api_key_input_placeholder_text": "API 키",
     "ai_config_openai_api_key_input_accessible_description": "OpenAI API 키",
     "ai_config_openai_api_supported_models_label": "지원되는 모델",
```

### Comparing `notolog-0.9.0b10/app/lexemes/ko/statusbar.py` & `notolog-0.9.0b11/app/lexemes/ko/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ko/toolbar.py` & `notolog-0.9.0b11/app/lexemes/ko/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/la/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/la/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/common.py` & `notolog-0.9.0b11/app/lexemes/la/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "De Applicatione",
     "popup_about_app_name_description": "Editor Markdown",
 
     "popup_about_version": "Versio",
     "popup_about_license": "Licentia",
     "popup_about_website": "Situs",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Dies",
 
     "update_helper_new_version_is_available": "Nova versio '{latest_version}' applicationis praesto est",
     "update_helper_latest_version_installed": "Ultima versio applicationis installata est",
 
     "network_connection_error_empty": "Informationes responsi obtineri non possunt",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/la/main_menu.py` & `notolog-0.9.0b11/app/lexemes/la/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/pt/settings_dialog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-# Latin lexemes settings_dialog.py
+# Portuguese lexemes settings_dialog.py
 lexemes = {
-    # Configurationes
-    "window_title": "Configurationes",
+    # Configurações
+    "window_title": "Configurações",
 
-    "button_close": "Claudere",
+    "button_close": "Fechar",
 
-    "tab_general": "Generale",
+    "tab_general": "Geral",
     "tab_editor_config": "Editor",
-    "tab_viewer_config": "Visor",
-    "tab_ai_config": "Configuratio AI",
+    "tab_viewer_config": "Visualizador",
+    "tab_ai_config": "Configuração de IA",
 
-    "general_app_config_label": "Configuratio App",
-    "general_app_language_label": "Lingua",
-    "general_app_language_combo_placeholder_text": "Elige linguam",
-    "general_app_language_combo_accessible_description": "Lingua interfaciei app",
-    "general_app_theme_label": "Thema",
-    "general_app_theme_combo_placeholder_text": "Elige thema",
-    "general_app_theme_combo_accessible_description": "Thema interfaciei app",
-    "general_app_main_menu_label": "Praecipuum Menu",
-    "general_app_main_menu_checkbox": "Praecipuum Menu Ostende",
-    "general_app_main_menu_checkbox_accessible_description": "Praecipuum dropdown menu applicationis ostendere",
-    "general_app_font_size_label": "Magnitudo Fontis: {size}pt",
-    "general_app_font_size_slider_accessible_description": "Regula magnitudinem fontis globalis applicationis",
+    "general_app_config_label": "Configuração do aplicativo",
+    "general_app_language_label": "Idioma",
+    "general_app_language_combo_placeholder_text": "Escolher um idioma",
+    "general_app_language_combo_accessible_description": "Idioma da interface do aplicativo",
+    "general_app_theme_label": "Tema",
+    "general_app_theme_combo_placeholder_text": "Escolher um tema",
+    "general_app_theme_combo_accessible_description": "Tema da interface do aplicativo",
+    "general_app_main_menu_label": "Menu Principal",
+    "general_app_main_menu_checkbox": "Mostrar menu principal",
+    "general_app_main_menu_checkbox_accessible_description": "Exibir o menu dropdown principal do aplicativo",
+    "general_app_font_size_label": "Tamanho da fonte: {size}pt",
+    "general_app_font_size_slider_accessible_description": "Ajustar o tamanho da fonte global do aplicativo",
 
-    "general_statusbar_label": "Status Barra",
-    "general_statusbar_show_global_cursor_position_checkbox": "Ostende Globalem Cursoris Positionem",
+    "general_statusbar_label": "Barra de Status",
+    "general_statusbar_show_global_cursor_position_checkbox": "Mostrar Posição Global do Cursor",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "Ostende globalem cursoris positionem in status barra",
+        "Exibir a posição global do cursor na barra de status",
 
-    "editor_config_label": "Editoris Configuratio",
-    "editor_config_show_line_numbers_checkbox": "Ostende Numeros Linearum",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "Ostende numeros linearum in editor",
+    "editor_config_label": "Configuração do Editor",
+    "editor_config_show_line_numbers_checkbox": "Mostrar Números de Linha",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "Exibir números de linha no editor",
 
-    "viewer_config_label": "Visoris Configuratio",
-    "viewer_config_process_emojis_checkbox": "Converte Textum Emojis ad Graphica",
+    "viewer_config_label": "Configuração do Visualizador",
+    "viewer_config_process_emojis_checkbox": "Converter Emojis de Texto em Gráficos",
     "viewer_config_process_emojis_checkbox_accessible_description":
-        "Converte emojis textuales in representationes graphicas",
-    "viewer_config_highlight_todos_checkbox": "Illustra TODOs",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "In textu TODOs signa illustra",
-    "viewer_config_open_link_confirmation_checkbox": "Postulat Confirmationem ad Aperiendum Nexus",
+        "Converter emojis de texto em representações gráficas",
+    "viewer_config_highlight_todos_checkbox": "Destacar TODOs",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "Destacar tags TODO no texto",
+    "viewer_config_open_link_confirmation_checkbox": "Requerer Confirmação para Abrir Links",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "Quaere confirmationem ante apertionem nexus",
-
-    "ai_config_openai_api_label": "API OpenAI",
-    "ai_config_openai_api_url_input_placeholder_text": "URL API",
-    "ai_config_openai_api_url_input_accessible_description": "URL API OpenAI",
-    "ai_config_openai_api_key_input_placeholder_text": "Clavis API",
-    "ai_config_openai_api_key_input_accessible_description": "Clavis API OpenAI",
-    "ai_config_openai_api_supported_models_label": "Modela sustenta",
-    "ai_config_ai_model_names_combo_placeholder_text": "Modelum elige",
-    "ai_config_ai_model_names_combo_accessible_description": "Modela sustenta ad eligendum",
-
-    "ai_config_base_label": "Parametri Principes",
-    "ai_config_base_system_prompt_label": "Systēma Monitum",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Monitum systēmatis basis quod præcedit singulas postulationes",
+        "Solicitar confirmação antes de abrir links",
+    "viewer_config_save_resources_checkbox": "Salvar automaticamente imagens externas no disco",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Salva automaticamente cópias de imagens externas no disco para acesso offline.",
+
+    "ai_config_openai_api_label": "API da OpenAI",
+    "ai_config_openai_api_url_input_placeholder_text": "URL da API",
+    "ai_config_openai_api_url_input_accessible_description": "URL da API da OpenAI",
+    "ai_config_openai_api_key_input_placeholder_text": "Chave da API",
+    "ai_config_openai_api_key_input_accessible_description": "Chave da API da OpenAI",
+    "ai_config_openai_api_supported_models_label": "Modelos suportados",
+    "ai_config_ai_model_names_combo_placeholder_text": "Escolher modelo",
+    "ai_config_ai_model_names_combo_accessible_description": "Modelos suportados para escolha",
+
+    "ai_config_base_label": "Parâmetros Base",
+    "ai_config_base_system_prompt_label": "Prompt do Sistema",
+    "ai_config_base_system_prompt_edit_placeholder_text": "Prompt do sistema base que antecede cada solicitação",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "Monitum systēmatis basis quod præcedit singulas postulationes. Textus simpliciter.",
-    "ai_config_base_response_max_tokens_label": "Maxima Responsionis Signa",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum signorum quæ in responsione accipiuntur",
+        "Prompt do sistema base que antecede cada solicitação. Texto simples.",
+    "ai_config_base_response_max_tokens_label": "Máximo de Tokens de Resposta",
+    "ai_config_base_response_max_tokens_input_accessible_description": "Número máximo de tokens a receber em resposta",
 }
```

### Comparing `notolog-0.9.0b10/app/lexemes/la/statusbar.py` & `notolog-0.9.0b11/app/lexemes/la/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/la/toolbar.py` & `notolog-0.9.0b11/app/lexemes/la/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/lexemes.py` & `notolog-0.9.0b11/app/lexemes/lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/pt/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/pt/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/common.py` & `notolog-0.9.0b11/app/lexemes/pt/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Informações do Aplicativo",
     "popup_about_app_name_description": "Editor Markdown",
 
     "popup_about_version": "Versão",
     "popup_about_license": "Licença",
     "popup_about_website": "Site",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Data",
 
     "update_helper_new_version_is_available": "Nova versão '{latest_version}' do aplicativo disponível",
     "update_helper_latest_version_installed": "A versão mais recente do aplicativo está instalada",
 
     "network_connection_error_empty": "Não é possível obter informações de resposta",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/pt/main_menu.py` & `notolog-0.9.0b11/app/lexemes/pt/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/it/settings_dialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-# Portuguese lexemes settings_dialog.py
+# Italian lexemes settings_dialog.py
 lexemes = {
-    # Configurações
-    "window_title": "Configurações",
+    # Impostazioni
+    "window_title": "Impostazioni",
 
-    "button_close": "Fechar",
+    "button_close": "Chiudi",
 
-    "tab_general": "Geral",
-    "tab_editor_config": "Editor",
-    "tab_viewer_config": "Visualizador",
-    "tab_ai_config": "Configuração de IA",
-
-    "general_app_config_label": "Configuração do aplicativo",
-    "general_app_language_label": "Idioma",
-    "general_app_language_combo_placeholder_text": "Escolher um idioma",
-    "general_app_language_combo_accessible_description": "Idioma da interface do aplicativo",
+    "tab_general": "Generale",
+    "tab_editor_config": "Editore",
+    "tab_viewer_config": "Visualizzatore",
+    "tab_ai_config": "Configurazione IA",
+
+    "general_app_config_label": "Configurazione dell'app",
+    "general_app_language_label": "Lingua",
+    "general_app_language_combo_placeholder_text": "Scegli una lingua",
+    "general_app_language_combo_accessible_description": "Lingua dell'interfaccia dell'app",
     "general_app_theme_label": "Tema",
-    "general_app_theme_combo_placeholder_text": "Escolher um tema",
-    "general_app_theme_combo_accessible_description": "Tema da interface do aplicativo",
-    "general_app_main_menu_label": "Menu Principal",
-    "general_app_main_menu_checkbox": "Mostrar menu principal",
-    "general_app_main_menu_checkbox_accessible_description": "Exibir o menu dropdown principal do aplicativo",
-    "general_app_font_size_label": "Tamanho da fonte: {size}pt",
-    "general_app_font_size_slider_accessible_description": "Ajustar o tamanho da fonte global do aplicativo",
+    "general_app_theme_combo_placeholder_text": "Scegli un tema",
+    "general_app_theme_combo_accessible_description": "Tema dell'interfaccia dell'app",
+    "general_app_main_menu_label": "Menu Principale",
+    "general_app_main_menu_checkbox": "Mostra il menu principale",
+    "general_app_main_menu_checkbox_accessible_description": "Visualizza il menu a discesa principale dell'app",
+    "general_app_font_size_label": "Dimensione del carattere: {size}pt",
+    "general_app_font_size_slider_accessible_description": "Regola la dimensione del carattere globale dell'app",
 
-    "general_statusbar_label": "Barra de Status",
-    "general_statusbar_show_global_cursor_position_checkbox": "Mostrar Posição Global do Cursor",
+    "general_statusbar_label": "Barra di Stato",
+    "general_statusbar_show_global_cursor_position_checkbox": "Mostra la Posizione Globale del Cursore",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "Exibir a posição global do cursor na barra de status",
+        "Visualizza la posizione globale del cursore nella barra di stato",
 
-    "editor_config_label": "Configuração do Editor",
-    "editor_config_show_line_numbers_checkbox": "Mostrar Números de Linha",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "Exibir números de linha no editor",
+    "editor_config_label": "Configurazione Editor",
+    "editor_config_show_line_numbers_checkbox": "Mostra Numeri di Riga",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "Visualizza i numeri di riga nell'editor",
 
-    "viewer_config_label": "Configuração do Visualizador",
-    "viewer_config_process_emojis_checkbox": "Converter Emojis de Texto em Gráficos",
+    "viewer_config_label": "Configurazione Visualizzatore",
+    "viewer_config_process_emojis_checkbox": "Converti Emoji di Testo in Grafica",
     "viewer_config_process_emojis_checkbox_accessible_description":
-        "Converter emojis de texto em representações gráficas",
-    "viewer_config_highlight_todos_checkbox": "Destacar TODOs",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "Destacar tags TODO no texto",
-    "viewer_config_open_link_confirmation_checkbox": "Requerer Confirmação para Abrir Links",
+        "Converti le emoji di testo in rappresentazioni grafiche",
+    "viewer_config_highlight_todos_checkbox": "Evidenzia TODO",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "Evidenzia le etichette TODO nel testo",
+    "viewer_config_open_link_confirmation_checkbox": "Richiedi Conferma per Aprire i Link",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "Solicitar confirmação antes de abrir links",
-
-    "ai_config_openai_api_label": "API da OpenAI",
-    "ai_config_openai_api_url_input_placeholder_text": "URL da API",
-    "ai_config_openai_api_url_input_accessible_description": "URL da API da OpenAI",
-    "ai_config_openai_api_key_input_placeholder_text": "Chave da API",
-    "ai_config_openai_api_key_input_accessible_description": "Chave da API da OpenAI",
-    "ai_config_openai_api_supported_models_label": "Modelos suportados",
-    "ai_config_ai_model_names_combo_placeholder_text": "Escolher modelo",
-    "ai_config_ai_model_names_combo_accessible_description": "Modelos suportados para escolha",
-
-    "ai_config_base_label": "Parâmetros Base",
-    "ai_config_base_system_prompt_label": "Prompt do Sistema",
-    "ai_config_base_system_prompt_edit_placeholder_text": "Prompt do sistema base que antecede cada solicitação",
+        "Richiedi conferma prima di aprire i link",
+    "viewer_config_save_resources_checkbox": "Salva automaticamente le immagini esterne sul disco",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Salva automaticamente copie delle immagini esterne sul disco per l'accesso offline.",
+
+    "ai_config_openai_api_label": "API OpenAI",
+    "ai_config_openai_api_url_input_placeholder_text": "URL API",
+    "ai_config_openai_api_url_input_accessible_description": "URL dell'API OpenAI",
+    "ai_config_openai_api_key_input_placeholder_text": "Chiave API",
+    "ai_config_openai_api_key_input_accessible_description": "Chiave API di OpenAI",
+    "ai_config_openai_api_supported_models_label": "Modelli supportati",
+    "ai_config_ai_model_names_combo_placeholder_text": "Scegli modello",
+    "ai_config_ai_model_names_combo_accessible_description": "Modelli supportati da scegliere",
+
+    "ai_config_base_label": "Parametri Base",
+    "ai_config_base_system_prompt_label": "Prompt del Sistema",
+    "ai_config_base_system_prompt_edit_placeholder_text": "Prompt di sistema base che precede ogni richiesta",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "Prompt do sistema base que antecede cada solicitação. Texto simples.",
-    "ai_config_base_response_max_tokens_label": "Máximo de Tokens de Resposta",
-    "ai_config_base_response_max_tokens_input_accessible_description": "Número máximo de tokens a receber em resposta",
+        "Prompt di sistema base che precede ogni richiesta. Testo semplice.",
+    "ai_config_base_response_max_tokens_label": "Massimo di Token di Risposta",
+    "ai_config_base_response_max_tokens_input_accessible_description": "Numero massimo di token da ricevere in risposta",
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `notolog-0.9.0b10/app/lexemes/pt/statusbar.py` & `notolog-0.9.0b11/app/lexemes/pt/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/pt/toolbar.py` & `notolog-0.9.0b11/app/lexemes/pt/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/ru/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/ru/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/common.py` & `notolog-0.9.0b11/app/lexemes/ru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "Информация о приложении",
     "popup_about_app_name_description": "Редактор Markdown",
 
     "popup_about_version": "Версия",
     "popup_about_license": "Лицензия",
     "popup_about_website": "Веб-сайт",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "Дата",
 
     "update_helper_new_version_is_available": "Доступна новая версия '{latest_version}' приложения",
     "update_helper_latest_version_installed": "Установлена последняя версия приложения",
 
     "network_connection_error_empty": "Не удаётся получить информацию о ответе",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/ru/main_menu.py` & `notolog-0.9.0b11/app/lexemes/ru/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/ru/settings_dialog.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     "viewer_config_process_emojis_checkbox_accessible_description":
         "Преобразовать текстовые эмодзи в графические изображения",
     "viewer_config_highlight_todos_checkbox": "Выделить задачи TODO",
     "viewer_config_highlight_todos_checkbox_accessible_description": "Выделять задачи TODO в тексте",
     "viewer_config_open_link_confirmation_checkbox": "Требовать подтверждение перед открытием ссылок",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
         "Запрашивать подтверждение перед открытием ссылок",
+    "viewer_config_save_resources_checkbox": "Автосохранение внешних изображений на диск",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Автоматически сохраняет копии внешних изображений на диск для доступа без подключения к интернету.",
 
     "ai_config_openai_api_label": "API OpenAI",
     "ai_config_openai_api_url_input_placeholder_text": "URL API",
     "ai_config_openai_api_url_input_accessible_description": "URL API OpenAI",
     "ai_config_openai_api_key_input_placeholder_text": "Ключ API",
     "ai_config_openai_api_key_input_accessible_description": "Ключ API OpenAI",
     "ai_config_openai_api_supported_models_label": "Поддерживаемые модели",
```

### Comparing `notolog-0.9.0b10/app/lexemes/ru/statusbar.py` & `notolog-0.9.0b11/app/lexemes/ru/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/ru/toolbar.py` & `notolog-0.9.0b11/app/lexemes/ru/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/ai_assistant.py` & `notolog-0.9.0b11/app/lexemes/zh/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/color_picker_dialog.py` & `notolog-0.9.0b11/app/lexemes/zh/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/common.py` & `notolog-0.9.0b11/app/lexemes/zh/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     "popup_about_title": "应用信息",
     "popup_about_app_name_description": "Markdown 编辑器",
 
     "popup_about_version": "版本",
     "popup_about_license": "许可证",
     "popup_about_website": "网站",
     "popup_about_repository": "GitHub",
+    "popup_about_pypi": "PyPi",
     "popup_about_date": "日期",
 
     "update_helper_new_version_is_available": "应用的新版本 '{latest_version}' 现已可用",
     "update_helper_latest_version_installed": "应用的最新版本已安装",
 
     "network_connection_error_empty": "无法获取响应信息",
     "network_connection_error_connection_or_dns":
```

### Comparing `notolog-0.9.0b10/app/lexemes/zh/main_menu.py` & `notolog-0.9.0b11/app/lexemes/zh/main_menu.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/settings_dialog.py` & `notolog-0.9.0b11/app/lexemes/en/settings_dialog.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,63 @@
-# Chinese lexemes settings_dialog.py
+# English lexemes settings_dialog.py
 lexemes = {
-    # 设置
-    "window_title": "设置",
+    # Settings dialog
+    "window_title": "Settings",
 
-    "button_close": "关闭",
+    "button_close": "Close",
 
-    "tab_general": "通用",
-    "tab_editor_config": "编辑器",
-    "tab_viewer_config": "查看器",
-    "tab_ai_config": "AI 配置",
-
-    "general_app_config_label": "应用配置",
-    "general_app_language_label": "语言",
-    "general_app_language_combo_placeholder_text": "选择语言",
-    "general_app_language_combo_accessible_description": "应用界面语言",
-    "general_app_theme_label": "主题",
-    "general_app_theme_combo_placeholder_text": "选择主题",
-    "general_app_theme_combo_accessible_description": "应用界面主题",
-    "general_app_main_menu_label": "主菜单",
-    "general_app_main_menu_checkbox": "显示主菜单",
-    "general_app_main_menu_checkbox_accessible_description": "显示应用的主下拉菜单",
-    "general_app_font_size_label": "字体大小：{size}pt",
-    "general_app_font_size_slider_accessible_description": "调整应用程序的全局字体大小",
+    "tab_general": "General",
+    "tab_editor_config": "Editor",
+    "tab_viewer_config": "Viewer",
+    "tab_ai_config": "AI Config",
+
+    "general_app_config_label": "App config",
+    "general_app_language_label": "Language",
+    "general_app_language_combo_placeholder_text": "Choose a language",
+    "general_app_language_combo_accessible_description": "App's interface language",
+    "general_app_theme_label": "Theme",
+    "general_app_theme_combo_placeholder_text": "Choose a theme",
+    "general_app_theme_combo_accessible_description": "App's interface theme",
+    "general_app_main_menu_label": "Main Menu",
+    "general_app_main_menu_checkbox": "Show Main Menu",
+    "general_app_main_menu_checkbox_accessible_description": "Display the app's main dropdown menu",
+    "general_app_font_size_label": "Font Size: {size}pt",
+    "general_app_font_size_slider_accessible_description": "Adjust the app's global font size",
 
-    "general_statusbar_label": "状态栏",
-    "general_statusbar_show_global_cursor_position_checkbox": "显示全局光标位置",
+    "general_statusbar_label": "Status Bar",
+    "general_statusbar_show_global_cursor_position_checkbox": "Show Global Cursor Position",
     "general_statusbar_show_global_cursor_position_checkbox_accessible_description":
-        "在状态栏显示全局光标位置",
+        "Display the global cursor position in the status bar",
 
-    "editor_config_label": "编辑器配置",
-    "editor_config_show_line_numbers_checkbox": "显示行号",
-    "editor_config_show_line_numbers_checkbox_accessible_description": "在编辑器中显示行号",
-
-    "viewer_config_label": "查看器配置",
-    "viewer_config_process_emojis_checkbox": "将文本表情转换为图形",
-    "viewer_config_process_emojis_checkbox_accessible_description": "将文本表情转换为图形表示",
-    "viewer_config_highlight_todos_checkbox": "突出显示待办事项",
-    "viewer_config_highlight_todos_checkbox_accessible_description": "在文本中突出显示待办事项标签",
-    "viewer_config_open_link_confirmation_checkbox": "打开链接前需确认",
+    "editor_config_label": "Editor Configuration",
+    "editor_config_show_line_numbers_checkbox": "Show Line Numbers",
+    "editor_config_show_line_numbers_checkbox_accessible_description": "Display line numbers in the editor",
+
+    "viewer_config_label": "Viewer Configuration",
+    "viewer_config_process_emojis_checkbox": "Convert Text Emojis to Graphics",
+    "viewer_config_process_emojis_checkbox_accessible_description": "Convert text emojis to graphical representations",
+    "viewer_config_highlight_todos_checkbox": "Highlight TODOs",
+    "viewer_config_highlight_todos_checkbox_accessible_description": "Emphasize TODO tags within the text",
+    "viewer_config_open_link_confirmation_checkbox": "Require Confirmation to Open Links",
     "viewer_config_open_link_confirmation_checkbox_accessible_description":
-        "打开链接前询问确认",
+        "Ask for confirmation before opening links",
+    "viewer_config_save_resources_checkbox": "Auto-save external images to disk",
+    "viewer_config_save_resources_checkbox_accessible_description":
+        "Automatically saves copies of external images to disk for offline access.",
 
     "ai_config_openai_api_label": "OpenAI API",
-    "ai_config_openai_api_url_input_placeholder_text": "API 地址",
-    "ai_config_openai_api_url_input_accessible_description": "OpenAI API 地址",
-    "ai_config_openai_api_key_input_placeholder_text": "API 密钥",
-    "ai_config_openai_api_key_input_accessible_description": "OpenAI API 密钥",
-    "ai_config_openai_api_supported_models_label": "支持的模型",
-    "ai_config_ai_model_names_combo_placeholder_text": "选择模型",
-    "ai_config_ai_model_names_combo_accessible_description": "选择支持的模型",
-
-    "ai_config_base_label": "基础参数",
-    "ai_config_base_system_prompt_label": "系统提示",
-    "ai_config_base_system_prompt_edit_placeholder_text": "基础系统提示，位于每个请求之前",
+    "ai_config_openai_api_url_input_placeholder_text": "API URL",
+    "ai_config_openai_api_url_input_accessible_description": "OpenAI API URL",
+    "ai_config_openai_api_key_input_placeholder_text": "API key",
+    "ai_config_openai_api_key_input_accessible_description": "OpenAI API key",
+    "ai_config_openai_api_supported_models_label": "Supported models",
+    "ai_config_ai_model_names_combo_placeholder_text": "Choose model",
+    "ai_config_ai_model_names_combo_accessible_description": "Supported models to choose",
+
+    "ai_config_base_label": "Base Parameters",
+    "ai_config_base_system_prompt_label": "System Prompt",
+    "ai_config_base_system_prompt_edit_placeholder_text": "Base system prompt that precedes each request",
     "ai_config_base_system_prompt_edit_accessible_description":
-        "基础系统提示，位于每个请求之前。纯文本。",
-    "ai_config_base_response_max_tokens_label": "响应的最大令牌数",
-    "ai_config_base_response_max_tokens_input_accessible_description": "响应中接收的最大令牌数",
+        "Base system prompt that precedes each request. This is plain text.",
+    "ai_config_base_response_max_tokens_label": "Maximum Response Tokens",
+    "ai_config_base_response_max_tokens_input_accessible_description": "Maximum number of tokens to receive in response",
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `notolog-0.9.0b10/app/lexemes/zh/statusbar.py` & `notolog-0.9.0b11/app/lexemes/zh/statusbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/lexemes/zh/toolbar.py` & `notolog-0.9.0b11/app/lexemes/zh/toolbar.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/notolog_editor.py` & `notolog-0.9.0b11/app/notolog_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-"""
-Notolog: An open-source markdown editor written in Python. (https://github.com/notolog/notolog-editor)
+# Notolog
+# An open-source markdown editor written in Python.
 
-Description:
+"""
 The project began as part of the developer's journey to learn Python, which may explain some seemingly redundant
 features. It was developed as a proof of concept to showcase what a markdown editor might look like and to assist
 the developer with daily tasks. Hopefully, you will find it useful too.
 
 The README.md file, located at the very beginning, was created using this editor and serves as a good demonstration
 of the app’s features.
 
 Code Style Disclaimer: While mixing code styles like camelCase and snake_case is generally avoided, many Qt methods
 use camelCase. However, the preferred style for Python 3 is typically PEP-8, which advocates for snake_case. Therefore,
 a compromise has been made in the Notolog codebase to predominantly use snake_case. This deliberate choice helps
 distinguish between the Qt and Notolog codebases, making it easier to identify which methods or classes belong to each.
-
----
-
-Additional Information:
-- GitHub Repository: https://github.com/notolog/notolog-editor
-- WebSite: https://notolog.app
-- Author: Vadim Bakhrenkov
-- License: MIT License
-- Version: 0.9.0b0
 """
 
-"""
-Main UI class to set up the application's UI and to process any user actions.
-"""
+# - GitHub Repository: https://github.com/notolog/notolog-editor
+# - PyPI: https://pypi.org/project/notolog
+# - WebSite: https://notolog.app
+# - Author: Vadim Bakhrenkov
+# - Copyright 2024 Vadim Bakhrenkov
+# - License: MIT License
+
 
 # Core classes
 from .settings import Settings
 from .app_config import AppConfig
 from .file_header import FileHeader
 from .edit_widget import EditWidget
 from .view_widget import ViewWidget
 from .view_processor import ViewProcessor
 from .view_decorator import ViewDecorator
+from .image_downloader import ImageDownloader
 
 # UI
 from .ui.file_system_model import FileSystemModel
 from .ui.sort_filter_proxy_model import SortFilterProxyModel
 from .ui.toolbar import ToolBar
 from .ui.statusbar import StatusBar
 from .ui.line_numbers import LineNumbers
@@ -62,88 +58,77 @@
 from .encrypt.enc_password_reset_dialog import EncPasswordResetDialog
 from cryptography.fernet import InvalidToken, InvalidSignature
 
 # Helpers
 from .helpers.theme_helper import ThemeHelper
 from .helpers.clipboard_helper import ClipboardHelper
 from .helpers.update_helper import UpdateHelper
-from .helpers.file_helper import res_path, size_f, save_file
+from .helpers.file_helper import res_path, size_f, read_file, save_file
 
 # Lexemes
 from .lexemes.lexemes import Lexemes
 
 # Editor state
 from .editor_state import EditorState, Mode, Source, Encryption
 
-from PySide6.QtCore import Qt, QDir, QPoint, QTimer, QSize
+from PySide6.QtCore import Slot, Qt, QDir, QPoint, QTimer, QSize, QUrl
 from PySide6.QtCore import QRegularExpression, QItemSelectionModel, QFileSystemWatcher
-from PySide6.QtGui import QGuiApplication, QIcon, QAction, QColor, QTextDocument, QShortcut
-from PySide6.QtGui import QKeySequence, QTextCursor, QFont, QTextBlock, QDesktopServices, QPalette
+from PySide6.QtGui import QGuiApplication, QIcon, QAction, QColor, QPalette, QShortcut, QFont, QKeySequence
+from PySide6.QtGui import QTextDocument, QTextCursor, QTextBlock, QDesktopServices, QPixmap, QPixmapCache
 from PySide6.QtWidgets import QWidget, QMainWindow, QVBoxLayout, QSplitter, QListView, QTextBrowser
 from PySide6.QtWidgets import QPlainTextEdit, QToolButton, QSizePolicy, QStatusBar, QCheckBox, QToolBar
 from PySide6.QtWidgets import QLabel, QLineEdit, QPushButton, QMenu, QDialog, QMessageBox, QStyle
 from PySide6.QtWidgets import QAbstractItemView, QFileSystemModel, QFileDialog
 
 from qasync import asyncSlot, asyncClose
+import asyncio
 
 # Markdown library
 import markdown
 # Markdown library extensions
 from markdown.extensions.codehilite import CodeHiliteExtension
 # Custom markdown extension to process element tree
 from .etree_extension import ElementTreeExtension
 
 # Emojis support
 import emoji
 
 import os
-import asyncio
-from pkg_resources import resource_filename
 from typing import Union, Optional, Callable, List, Dict, Any
 
 import logging
 
 
-"""
-To change content scale ratio use either:
-    # View widget
-    view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
-    view_widget.setZoomFactor(float(self.scale))
-Or
-    os.environ["QT_SCALE_FACTOR"] = "1.2"
-As it works better than: `body { transform: scale(%s); transform-origin: 0 0; }`
-"""
-
-"""
-Template to apply to the view mode.
-"""
-HTML_TPL = """
-    <!DOCTYPE html>
-    <html lang="en">
-    <head>
-        <meta charset="UTF-8">
-        <title>%s</title>
-        <style type="text/css">
-        %s
-        </style>
-    </head>
-    <body>
-    %s
-    </body>
-    </html>
-    """
-
-
 class NotologEditor(QMainWindow):
+    """
+    Main UI class to set up the application's UI and to process any user actions.
+    """
 
     AREA_WEIGHT = 5
     AREA_WEIGHT_TREE = 1
     AREA_WEIGHT_EDIT = 4
     AREA_WEIGHT_VIEW = 4
 
+    # Template to apply to the view mode.
+    HTML_TPL = """
+        <!DOCTYPE html>
+        <html lang="en">
+        <head>
+            <meta charset="UTF-8">
+            <title>%s</title>
+            <style type="text/css">
+            %s
+            </style>
+        </head>
+        <body>
+        %s
+        </body>
+        </html>
+        """
+
     """
     Some extensions like `codehilite` extension will be included later.
 
     Extra contains:
     * Abbreviations
     * Attribute Lists
     * Definition Lists
@@ -254,14 +239,21 @@
 
         # Markdown instance
         self.md = None  # type: Union[markdown.Markdown, None]
 
         # Highlighters
         self.md_highlighter = None  # type: Union[MdHighlighter, None]
         self.view_highlighter = None  # type: Union[ViewHighlighter, None]
+        # async re-highlight tasks queue
+        self.rehighlight_tasks = []
+
+        # Resource Downloader
+        self.resource_downloader = None  # type: Union[ImageDownloader, None]
+        # async download tasks queue
+        self.resource_tasks = []
 
         # File tree and variable
         self.tree_container = None  # type: Union[QWidget, None]
         self.file_model = None  # type: Union[FileSystemModel, None]
         self.tree_view = None  # type: Union[QListView, None]
         self.tree_filter = None  # type: Union[QLineEdit, None]
         self.tree_proxy_model = None  # type: Union[SortFilterProxyModel, None]
@@ -271,19 +263,14 @@
         self.supported_file_extensions = ['md', 'txt', 'html', 'enc']
 
         # Line numbers within the document
         self.line_numbers = None  # type: Union[LineNumbers, None]
 
         # Toolbar
         self.toolbar = None  # type: Union[ToolBar, QToolBar, None]
-        self.search_input = None  # type: Union[QLineEdit, None]
-        self.btn_search_clear = None  # type: Union[QPushButton, None]
-        self.btn_search_prev = None  # type: Union[QPushButton, None]
-        self.btn_search_next = None  # type: Union[QPushButton, None]
-        self.search_match_case = None  # type: Union[QCheckBox, None]
 
         # Statusbar
         self.statusbar = None  # type: Union[StatusBar, QStatusBar, None]
 
         # Current document's variables
         self.col_num = 0  # Column where cursor located at
         self.line_num = 0  # Machine-readable, starts from 0
@@ -334,15 +321,15 @@
             self
         )
         shortcut_search.activated.connect(self.search_text)
 
     def init_font(self):
         # Use default ratio
         font_size_ratio = 1.0
-        font_size = int(self.settings.app_font_size * font_size_ratio)
+        font_size = int(float(self.settings.app_font_size) * font_size_ratio)
 
         AppConfig.set_font_size(font_size)
 
         font = QFont()  # Accept args like "Sans Serif"
         font.setPointSize(font_size)
 
         if self.debug:
@@ -382,16 +369,14 @@
             # Edit widget
             edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
             edit_widget.document().setDefaultFont(self.font())
             # Apply font from the main window to the widget
             self.tree_view.setFont(self.font())
             # Apply font from the main window to the widget
             self.tree_filter.setFont(self.font())
-            # Update toolbar
-            self.create_icons_toolbar(refresh=True)
             # Re-draw main menu
             self.draw_menu()
             # Update statusbar
             self.create_status_toolbar()
             # Refresh all dependant UI elements that have been initialized
             self.estate.refresh()
             self.statusbar['data_size_label'].setText("%s" % size_f(len(self.content)))
@@ -411,16 +396,17 @@
             self.lexemes = Lexemes(self.settings.app_language)
             # Trigger editor state update
             self.estate.refresh()
             # Update window title
             self.set_app_title()  # Generic title without sub part
             # Update toolbar
             self.create_icons_toolbar(refresh=True)
-            # Search field placeholder to empty
-            self.search_input.setPlaceholderText(self.lexemes.get('search_input_placeholder_text', scope='toolbar'))
+            if hasattr(self.toolbar, 'search_input'):
+                # Search field placeholder to empty
+                self.toolbar.search_input.setPlaceholderText(self.lexemes.get('search_input_placeholder_text', scope='toolbar'))
             # Re-draw main menu
             self.draw_menu()
 
         if 'app_theme' in data and hasattr(self, 'theme_helper'):
             self.theme_helper = ThemeHelper()
             # Update app's palette styles
             self.init_palette()
@@ -440,16 +426,14 @@
             # View widget
             view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
             view_widget.setStyleSheet(self.theme_helper.get_css('viewer'))
             # Update code highlighter to reload color scheme
             self.md_highlighter = MdHighlighter(document=edit_widget.document())
             # Update view highlighter to reload color scheme
             self.view_highlighter = ViewHighlighter(document=view_doc)
-            # Save any unsaved changes before calling file reload
-            self.save_active_file(clear_after=False)
             # To allow view document reload highlighter styles
             self.reload_active_file()
 
         if 'show_main_menu' in data:
             # Re-draw main menu
             self.draw_menu()
 
@@ -984,33 +968,40 @@
             """
             Previous approach was:
             self.tree_proxy_model.setFilterWildcard("*{}*".format(text))
             """
         else:
             self.tree_proxy_model.setFilterRegularExpression(r'')
 
-        self.adjust_tree_current_root_index()  # To re-set an actual file path and current dir for the tree.
-
     def adjust_tree_current_root_index(self) -> None:
         # dir_path = QDir.homePath()
         # dir_path = QDir.currentPath()
-        dir_path = os.path.dirname(str(self.get_current_path()))
+        dir_path = os.path.dirname(str(self.get_current_file_path()))
         root_index = self.file_model.index(dir_path)
         """
         More info about this mapping https://doc.qt.io/qt-6/qsortfilterproxymodel.html#mapFromSource
         """
         proxy_index = self.tree_proxy_model.mapFromSource(root_index)
         self.tree_view.setRootIndex(proxy_index)
 
-    def get_current_path(self, is_base: bool = False) -> str:
+    def get_current_file_path(self, is_base: bool = False) -> str:
         """
         Get current file path.
         """
         return os.path.dirname(self.file_path) if is_base else self.file_path
 
+    def get_active_dir(self):
+        """
+        The directory where the navigation context is currently located. Please note that this directory
+        may not necessarily be the same as the directory where the current file is opened.
+        """
+        root_index = self.tree_view.rootIndex()
+        source_index = self.tree_proxy_model.mapToSource(root_index)
+        return self.file_model.filePath(source_index)
+
     def set_current_path(self, tree_path: str) -> None:
         """
         Set current file path and tree index.
         """
         # Path's index
         index = self.file_model.index(tree_path)
         if os.path.isfile(tree_path):
@@ -1039,15 +1030,15 @@
             self.tree_view.setRootIndex(proxy_dir_index)
 
     def confirm_current_path(self) -> None:
         """
         Confirm current file params.
         It may be necessary to set params after encrypted file opened or so.
         """
-        current_file_path = self.get_current_path()
+        current_file_path = self.get_current_file_path()
         self.settings.file_path = current_file_path
         self.set_encryption(Encryption.ENCRYPTED if self.is_file_encrypted(current_file_path) else Encryption.PLAIN)
 
     def show_tree_context_menu(self, tree_view: QListView, pos: QPoint) -> None:
         """
         Context menu at file tree view.
         """
@@ -1188,15 +1179,15 @@
                 if self.debug:
                     self.logger.debug('File (reversibly) deleted to "%s"', del_file_path)
             else:
                 if self.debug:
                     self.logger.debug('Cannot delete file, error occurred "%s"' % del_file_path)
                 self.message_box(self.lexemes.get('dialog_file_delete_error'), icon_type=2)
             # Check deleted file was actually shown
-            if self.get_current_path() == file_path:
+            if self.get_current_file_path() == file_path:
                 any_file_path = self.get_any_file()
                 if any_file_path is not None:
                     self.load_file(any_file_path)
         else:
             if self.debug:
                 self.logger.debug('File not found "%s"' % file_path)
             self.message_box(self.lexemes.get('dialog_file_delete_error_not_found'), 2)
@@ -1226,22 +1217,23 @@
 
         if self.debug:
             self.logger.debug('Delete file completely "%s" dialog callback with sub-callback %s' % (file_path, callback))
 
         if os.path.isfile(file_path):
             try:
                 os.remove(file_path)
-                print(f"File {file_path} has been completely deleted.")
+                if self.debug:
+                    self.logger.debug(f"File {file_path} has been completely deleted.")
             except OSError as e:
                 if self.logging:
                     self.logger.warning(f"Error: {e.strerror}. Could not delete {file_path}.")
                 self.message_box(self.lexemes.get('dialog_file_delete_error'), icon_type=2)
 
             # Check deleted file was actually shown
-            if self.get_current_path() == file_path:
+            if self.get_current_file_path() == file_path:
                 any_file_path = self.get_any_file()
                 if any_file_path is not None:
                     self.load_file(any_file_path)
         else:
             if self.debug:
                 self.logger.debug('File not found "%s"' % file_path)
             self.message_box(self.lexemes.get('dialog_file_delete_error_not_found'), 2)
@@ -1627,14 +1619,15 @@
             self.logger.debug(f'Creating view widget, signals was blocked "{was_blocked}"')
         # Adjust font to match the size of the default or changed one
         view_widget.document().setDefaultFont(self.font())
         view_widget.setReadOnly(True)
         if isinstance(view_widget, QTextBrowser):
             # Process anchor click separately
             view_widget.setOpenLinks(False)
+            view_widget.setOpenExternalLinks(False)
             view_widget.anchorClicked.connect(self.open_link_dialog_proxy())
         view_widget.setContentsMargins(0, 0, 0, 0)
         """
         More info about the enum: https://doc.qt.io/qt-6/qsizepolicy.html#Policy-enum
         """
         view_widget.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
 
@@ -1675,16 +1668,16 @@
     @asyncClose
     async def closeEvent(self, event):
         if self.logging:
             self.logger.info('Stopping events loop, closing the app... Sayonara!')
 
         # Cancel all pending tasks if exist
         if hasattr(self, 're_tasks'):
-            tasks_total = len(self.re_tasks)
-            for i, task in enumerate(self.re_tasks):
+            tasks_total = len(self.rehighlight_tasks)
+            for i, task in enumerate(self.rehighlight_tasks):
                 if not task.done():
                     task_res = task.cancel()
                     if self.logging:
                         self.logger.info(f'[{i+1}/{tasks_total}] Pending task "{task.get_name()}" canceled with result "{task_res}"')
 
         if self.get_mode() == Mode.EDIT:
             # Save any unsaved changes
@@ -1699,54 +1692,42 @@
         event.accept()
 
     @asyncSlot()
     async def rehighlight_in_queue(self, full_rehighlight: bool = False) -> None:
         """
         More info about asyncio tasks: https://docs.python.org/3/library/asyncio-task.html
         """
-
-        # Create initial array if not exists
-        if not hasattr(self, 're_tasks'):
-            self.re_tasks = []
-
         if self.debug:
-            self.logger.debug('Re-highlight %d tasks in queue' % len(self.re_tasks))
+            self.logger.debug('Re-highlight %d tasks in queue' % len(self.rehighlight_tasks))
 
-        postpone = False if len(self.re_tasks) == 0 else True
+        postpone = False if len(self.rehighlight_tasks) == 0 else True
         if self.debug:
             self.logger.debug('Re-highlight is to postpone "%r"' % postpone)
 
         # To keep only a few tasks in queue
-        if len(self.re_tasks) < 3:
+        if len(self.rehighlight_tasks) < 3:
             task = asyncio.ensure_future(self.rehighlight_async(full_rehighlight, postpone))
             # task = asyncio.create_task(self.rehighlight_async(full_rehighlight, postpone))
             task.add_done_callback(
                 lambda _task:
                     (self.logger.info('%s from total %d completed with callback'
-                                      % (_task.get_name(), len(self.re_tasks))) if self.debug else None,
-                        self.re_tasks.remove(_task),
+                                      % (_task.get_name(), len(self.rehighlight_tasks))) if self.debug else None,
+                        self.rehighlight_tasks.remove(_task),
                         QTimer.singleShot(750,
-                                          lambda: self.rehighlight_editor(True)) if len(self.re_tasks) == 0 else None)
+                            lambda: self.rehighlight_editor(True)) if len(self.rehighlight_tasks) == 0 else None)
             )
-            self.re_tasks.append(task)
+            self.rehighlight_tasks.append(task)
 
         done, pending = await asyncio.wait(
-            self.re_tasks,
-            return_when=asyncio.ALL_COMPLETED,
+            self.rehighlight_tasks,
+            return_when=asyncio.ALL_COMPLETED,  # no pending tasks check
         )
 
-        # Actually, there is only one task in queue
-        for _task in self.re_tasks:
-            if _task in pending:
-                if self.debug:
-                    self.logger.debug('Re-highlight task "%s" is pending' % _task.get_name())
-            if _task in done:
-                if self.debug:
-                    self.logger.debug('Re-highlight task "%s" is done, from [%d]'
-                                      % (_task.get_name(), len(self.re_tasks)))
+        if self.debug:
+            self.logger.debug(f'Re-highlight tasks progress. Done {len(done)}, pending {len(pending)}')
 
     async def rehighlight_async(self, full_rehighlight: bool = False, postpone: bool = False) -> None:
         """
         Run this method not too often to avoid overwhelming the system.
         """
         # First of all check it's necessary
         if self.get_mode() == Mode.EDIT and self.get_source() == Source.MARKDOWN:
@@ -1813,16 +1794,16 @@
         More info about the signal: https://doc.qt.io/qt-6/qplaintextedit.html#textChanged
         """
 
         if self.debug:
             self.logger.debug('Text changed signal from %s' % (self.sender()))
 
         # Make save button active at the toolbar, even if no changes to save resources with no check
-        if hasattr(self, 'toolbar_save_button'):
-            self.toolbar_save_button.setDisabled(False)
+        if hasattr(self.toolbar, 'toolbar_save_button'):
+            self.toolbar.toolbar_save_button.setDisabled(False)
 
         full_rehighlight = (self.get_block_data_param('code', 'opened')
                             or self.get_block_data_param('code', 'closed'))
 
         # Schedule async whole doc re-highlighting task in queue
         self.rehighlight_in_queue(full_rehighlight)
         """
@@ -2003,20 +1984,20 @@
                  'label': self.lexemes.get('actions_file_label_open', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_open', scope='main_menu'),
                  'action': self.action_open_file},
                 {'type': 'action', 'name': 'actions_file_label_save',
                  'system_icon': 'media-floppy', 'theme_icon': 'floppy2-fill.svg',
                  'label': self.lexemes.get('actions_file_label_save', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_save', scope='main_menu'),
-                 'action': self.action_save_file, 'var_name': 'save_button'},
+                 'action': self.action_save_file,},
                 {'type': 'action', 'name': 'actions_file_label_save_as',
                  'system_icon': 'media-floppy', 'theme_icon': 'floppy2.svg',
                  'label': self.lexemes.get('actions_file_label_save_as', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_save_as', scope='main_menu'),
-                 'action': self.action_save_as_file, 'var_name': 'save_as_button'},
+                 'action': self.action_save_as_file,},
                 {'type': 'delimiter'},
                 {'type': 'action', 'name': 'actions_file_label_exit',
                  'system_icon': 'application-exit', 'theme_icon': 'power.svg',
                  'label': self.lexemes.get('actions_file_label_exit', scope='main_menu'),
                  'accessible_name': self.lexemes.get('actions_file_accessible_name_exit', scope='main_menu'),
                  'action': self.action_exit},
             ]},
@@ -2175,35 +2156,35 @@
              'label': self.lexemes.get('actions_label_edit', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_edit', scope='toolbar'),
              'action': self.action_edit_file, 'active_state_check': lambda: self.get_mode() == Mode.EDIT},
             {'type': 'action', 'weight': 5, 'name': 'toolbar_actions_label_source', 'system_icon': 'edit-find',
              'theme_icon': 'code-slash.svg', 'color': self.theme_helper.get_color('toolbar_icon_color_source'),
              'label': self.lexemes.get('actions_label_source', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_source', scope='toolbar'),
-             'action': self.action_source, 'var_name': 'toolbar_source_button',
+             'action': self.action_source,
              'active_state_check': lambda: self.get_mode() != Mode.SOURCE},
             # Active Source Mode icon
             {'type': 'action', 'weight': 5, 'name': 'toolbar_actions_label_source_act', 'system_icon': 'edit-find',
              'theme_icon': 'code-slash.svg', 'color': self.theme_helper.get_color('toolbar_icon_color_source_act'),
              'label': self.lexemes.get('actions_label_source', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_source', scope='toolbar'),
-             'action': self.action_source, 'var_name': 'toolbar_source_active_button',
+             'action': self.action_source,
              'active_state_check': lambda: self.get_mode() == Mode.SOURCE},
             {'type': 'action', 'weight': 6, 'name': 'toolbar_actions_label_encrypt', 'system_icon': 'security-low',
              'theme_icon': 'shield-lock.svg', 'color': self.theme_helper.get_color('toolbar_icon_color_encrypt'),
              'label': self.lexemes.get('actions_label_encrypt', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_encrypt', scope='toolbar'),
-             'action': self.action_encrypt, 'var_name': 'toolbar_encrypt_button',
+             'action': self.action_encrypt,
              'active_state_check': lambda: self.get_encryption() != Encryption.ENCRYPTED},
             # Active Encryption icon
             {'type': 'action', 'weight': 6, 'name': 'toolbar_actions_label_decrypt', 'system_icon': 'security-medium',
              'theme_icon': 'shield-lock-fill.svg', 'color': self.theme_helper.get_color('toolbar_icon_color_decrypt'),
              'label': self.lexemes.get('actions_label_decrypt', scope='toolbar'),
              'accessible_name': self.lexemes.get('actions_accessible_name_decrypt', scope='toolbar'),
-             'action': self.action_decrypt, 'var_name': 'toolbar_decrypt_button',
+             'action': self.action_decrypt,
              'active_state_check': lambda: self.get_encryption() == Encryption.ENCRYPTED},
             {'type': 'delimiter'},
             # Text format
             {'type': 'action', 'weight': 7, 'name': 'toolbar_toolbar_icon_color_bold',
              'system_icon': 'format-text-bold', 'theme_icon': 'type-bold.svg',
              'color': self.theme_helper.get_color('toolbar_icon_color_bold'),
              'label': self.lexemes.get('actions_label_bold', scope='toolbar'),
@@ -2319,199 +2300,32 @@
     def create_icons_toolbar(self, refresh: bool = False) -> None:
         """
         Main toolbar with icons.
         """
         if refresh and hasattr(self, 'toolbar'):
             self.removeToolBar(self.toolbar)
         """
-        Toolbar element:
+        Or Toolbar element:
         toolbar = self.addToolBar("Toolbar")
-        Or create QToolBar object first
         """
         self.toolbar = ToolBar(
             parent=self,
-            labels=self.get_toolbar_actions(),
-            refresh=lambda: self.create_icons_toolbar(refresh=True)
+            actions=self.get_toolbar_actions(),
+            buttons=self.get_toolbar_search_buttons(),
+            refresh=lambda: self.create_icons_toolbar(refresh=True)  # Action to call if refresh needed
         )
-        self.addToolBar(self.toolbar)
-        self.toolbar.setMovable(False)
 
-        prev_type = None
-        for icon in self.get_toolbar_actions():
-            if icon['type'] == 'action':
-                # Check visible icon is checked in settings
-                if not (self.settings.toolbar_icons & pow(2, icon['weight'])):
-                    # Skip if not checked in settings
-                    continue
-                # If the icon has an active state check, check it here
-                if ('active_state_check' in icon
-                        and callable(icon['active_state_check'])
-                        and not icon['active_state_check']()):
-                    # Skip if the icon isn't active
-                    continue
-                result_icon = self.create_toolbar_icon(
-                    system_icon=icon['system_icon'] if 'system_icon' in icon else None,
-                    theme_icon=icon['theme_icon'],
-                    label=icon['label'],
-                    action=icon['action'],
-                    accessible_name=icon['accessible_name'],
-                    color=icon['color'] if 'color' in icon else self.theme_helper.get_color('toolbar_icon_color_default'),
-                    toolbar=self.toolbar
-                )
-                # Add internal variable to access the icon later, say for state toggle
-                if 'var_name' in icon:
-                    if self.debug and hasattr(self, icon['var_name']):
-                        self.logger.debug('Variable "%s" is already set! Re-writing it...' % icon['var_name'])
-                    setattr(self, icon['var_name'], result_icon)  # type: QToolButton
-                # If the icon has a switched off check, check it here
-                if ('switched_off_check' in icon
-                        and callable(icon['switched_off_check'])
-                        and icon['switched_off_check']()):
-                    # Switch the icon off
-                    result_icon.setDisabled(True)
-            elif icon['type'] == 'delimiter' and prev_type != 'delimiter':
-                self.toolbar.addSeparator()
-            # Save prev type
-            prev_type = icon['type']
-
-        central_spacer = QWidget(self)
-        central_spacer.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
-        self.toolbar.addWidget(central_spacer)
+        if hasattr(self.toolbar, 'search_input'):
+            # Connect actions to the search field
+            self.toolbar.search_input.textChanged.connect(self.action_search_on)
+            self.toolbar.search_input.returnPressed.connect(self.action_search_next)
+            # And adjust appearance
+            self.toolbar.search_input.setMaximumWidth(self.weight_to_px_uno)
 
-        search_label = QLabel(self)
-        # Apply font from the main window to the widget
-        search_label.sizeHint()
-        search_label.setText(self.lexemes.get('search_input_label', scope='toolbar'))
-        search_label.setObjectName('search_input_label')  # To differentiate it at styles file
-        self.toolbar.addWidget(search_label)
-
-        self.search_input = QLineEdit(self)
-        self.search_input.setObjectName('search_input')
-        self.search_input.sizeHint()
-        self.search_input.setReadOnly(False)
-        self.search_input.setMaxLength(128)
-        self.search_input.setMaximumWidth(self.weight_to_px_uno)
-        self.search_input.setPlaceholderText(self.lexemes.get('search_input_placeholder_text', scope='toolbar'))
-        self.search_input.setAccessibleDescription(self.lexemes.get('search_input_accessible_description', scope='toolbar'))
-        self.search_input.textChanged.connect(self.action_search_on)
-        self.search_input.returnPressed.connect(self.action_search_next)
-        self.toolbar.addWidget(self.search_input)
-
-        for button in self.get_toolbar_search_buttons():
-            if button['type'] == 'action':
-                result = self.create_toolbar_button(
-                    system_icon=button['system_icon'],
-                    theme_icon=button['theme_icon'],
-                    action=button['action'],
-                    tooltip=button['tooltip'],
-                    default=button['default'],
-                    enabled=button['enabled'],
-                    accessible_name=button['accessible_name'],
-                    color=button['color'] if 'color' in button else self.theme_helper.get_color('toolbar_icon_color_default'),
-                    toolbar=self.toolbar
-                )
-                if 'var_name' in button:
-                    if self.debug and hasattr(self, button['var_name']):
-                        self.logger.debug('Variable "%s" is already set! Re-writing it...' % button['var_name'])
-                    setattr(self, button['var_name'], result)  # type: QPushButton
-
-        search_match_case_label = QLabel(self)
-        search_match_case_label.sizeHint()
-        search_match_case_label.setText(self.lexemes.get('search_case_sensitive', scope='toolbar'))
-        search_match_case_label.setObjectName("search_case_sensitive")  # To differentiate it at styles file
-        self.toolbar.addWidget(search_match_case_label)
-
-        self.search_match_case = QCheckBox(self)
-        self.search_match_case.sizeHint()
-        self.search_match_case.setToolTip(self.lexemes.get('search_match_case_tooltip', scope='toolbar'))
-        self.search_match_case.setCheckState(Qt.CheckState.Unchecked)
-        self.toolbar.addWidget(self.search_match_case)
-
-        """
-        It can be done by setting inline styles, but this is not what can be convenient for customisation,
-        hence the theme:
-        """
-        # self.toolbar.setStyleSheet("""QCheckBox {
-        #    margin-right: 5px;
-        # }""")
-        self.toolbar.setStyleSheet(self.theme_helper.get_css('toolbar'))
-
-    def create_toolbar_icon(self, **kwargs) -> QToolButton:
-        """
-        Helper to create, add to the toolbar and return button with an icon.
-        """
-        name = kwargs['name'] if 'name' in kwargs else None
-        system_icon = kwargs['system_icon'] if 'system_icon' in kwargs else None
-        theme_icon = kwargs['theme_icon'] if 'theme_icon' in kwargs else None
-        theme_icon_color = QColor(kwargs['color']) if 'color' in kwargs and kwargs['color'] else None
-        label = kwargs['label'] if 'label' in kwargs else None
-        # Action triggered on click
-        action = kwargs['action'] if 'action' in kwargs else None
-        accessible_name = kwargs['accessible_name'] if 'accessible_name' in kwargs else  None
-        icon_toolbar = kwargs['toolbar'] if 'toolbar' in kwargs else None
-        # Theme icon with a fallback to a system one
-        icon = self.theme_helper.get_icon(theme_icon=theme_icon, system_icon=system_icon, color=theme_icon_color)
-        icon_action = QAction(icon, label, self)
-        icon_button = QToolButton(self)
-        icon_button.setObjectName(name)
-        icon_button.setToolTip(label)
-        # icon_button.setIconSize(QSize(16, 16));
-        icon_button.setDefaultAction(icon_action)
-        # icon_action.setChecked(True)
-        if action is not None:
-            icon_action.triggered.connect(action)
-        if accessible_name is not None:
-            icon_button.setAccessibleName(accessible_name)
-        # Add the button to the toolbar
-        if icon_toolbar is not None:
-            icon_toolbar.addWidget(icon_button)
-        # Return button as a result
-        return icon_button
-
-    def create_toolbar_button(self, **kwargs) -> QPushButton:
-        """
-        Helper to create and return toolbar push button.
-        """
-        system_icon = kwargs['system_icon'] if 'system_icon' in kwargs else None
-        theme_icon = kwargs['theme_icon'] if 'theme_icon' in kwargs else None
-        theme_icon_color = QColor(kwargs['color']) if 'color' in kwargs and kwargs['color'] else None
-        # Action clicked
-        action = kwargs['action'] if 'action' in kwargs else None
-        accessible_name = kwargs['accessible_name'] if 'accessible_name' in kwargs else  None
-        tooltip = kwargs['tooltip'] if 'tooltip' in kwargs else None
-        default = kwargs['default'] if 'default' in kwargs else None
-        enabled = kwargs['enabled'] if 'enabled' in kwargs else None
-        icon_toolbar = kwargs['toolbar'] if 'toolbar' in kwargs else None
-        # Theme icon with a fallback to a system one
-        icon = self.theme_helper.get_icon(theme_icon=theme_icon, system_icon=system_icon, color=theme_icon_color)
-        # Toolbar button with an icon
-        icon_button = QPushButton(self)
-        icon_button.setFont(self.font())
-        if hasattr(self, 'search_input'):
-            # Adjust size to maintain ratio
-            size_hint = self.search_input.sizeHint()  # As a real height hint check the line edit height
-            icon_button.setFixedSize(QSize(size_hint.height(), size_hint.height()))
-            icon_height = int(size_hint.height() * 0.7)
-            icon_button.setIconSize(QSize(icon_height, icon_height))
-        icon_button.setIcon(icon)
-        if action is not None:
-            icon_button.clicked.connect(action)
-        if accessible_name is not None:
-            icon_button.setAccessibleName(accessible_name)
-        if tooltip is not None:
-            icon_button.setToolTip(tooltip)
-        if default is not None:
-            icon_button.setDefault(default)
-        if enabled is not None:
-            icon_button.setEnabled(enabled)
-        # Add the button to the toolbar
-        if icon_toolbar is not None:
-            icon_toolbar.addWidget(icon_button)
-        # Return button as a result
-        return icon_button
+        self.addToolBar(self.toolbar)
 
     def create_status_toolbar(self) -> None:
         # Statusbar element
         self.statusbar = StatusBar(self)
         self.setStatusBar(self.statusbar)
 
     def action_new_file(self, content: str = None) -> bool:
@@ -2523,17 +2337,16 @@
             self.save_active_file(clear_after=True)
         else:
             # Toggle mode first to start new file in EDIT mode
             self.toggle_mode()
 
         i = 1
         new_file_name_tpl = 'new-document-%d.md'
-
         # Find the file name that is not exist
-        while (file_path := res_path(new_file_name_tpl % i)) and os.path.isfile(file_path):
+        while (file_path := os.path.join(self.get_active_dir(), new_file_name_tpl % i)) and os.path.isfile(file_path):
             i += 1
             # Just to prevent never-ending cycle
             if i > 9999:
                 return False
 
         # Default file content if none provided
         if not content:
@@ -2560,15 +2373,15 @@
         * https://doc.qt.io/qt-6/qfiledialog.html#details
         * https://doc.qt.io/qt-6/qfiledialog.html#getOpenFileName
         """
         file_path, _ = QFileDialog.getOpenFileName(
             self,
             caption=self.lexemes.get('action_open_file_dialog_caption'),
             # Also can be: os.path.expanduser("~") or QDir.currentPath()
-            dir=os.path.expanduser(self.get_current_path(is_base=True)),
+            dir=os.path.expanduser(self.get_current_file_path(is_base=True)),
             # Filter accepts possible file types to show
             filter='Text Files (%s);;All Files (*)' % ' '.join(["*." + ext for ext in self.supported_file_extensions]),
             # QFileDialog.Option.ReadOnly
             # https://doc.qt.io/qt-6/qfiledialog.html#Option-enum
             options=QFileDialog.Option.DontUseCustomDirectoryIcons
         )
         if os.path.isfile(file_path):
@@ -2579,15 +2392,15 @@
 
     def action_save_file(self, file_path: str = None) -> None:
         """
         Action: Save file.
         """
         # Choose currently open file if another one is not explicitly passed
         if file_path is None:
-            file_path = self.get_current_path()
+            file_path = self.get_current_file_path()
 
         if file_path is None:
             if self.logging:
                 self.logger.warning('Cannot save file because of the file path is not set!')
             return
 
         # Save any unsaved changes, keep text edit field's content
@@ -2596,15 +2409,15 @@
     def action_save_as_file(self) -> None:
         """
         Action: Save as a file.
         """
         file_path, _ = QFileDialog.getSaveFileName(
             self,
             caption=self.lexemes.get('action_save_as_file_dialog_caption'),
-            dir=os.path.expanduser(self.get_current_path(is_base=True)),
+            dir=os.path.expanduser(self.get_current_file_path(is_base=True)),
             # Filter accepts possible file types to show
             filter='Text Files (%s);;All Files (*)' % ' '.join(["*." + ext for ext in self.supported_file_extensions]),
             # https://doc.qt.io/qt-6/qfiledialog.html#Option-enum
             # options=QFileDialog.Option.DontUseNativeDialog
         )
         if file_path:
             with open(file_path, 'w', encoding='utf-8') as file:
@@ -2613,15 +2426,15 @@
                 file.write(edit_widget.toPlainText())
 
     def action_edit_file(self) -> None:
         """
         Action: Edit/View mode toggle.
         """
         if self.debug:
-            self.logger.debug('Edit file "%s"' % self.get_current_path())
+            self.logger.debug('Edit file "%s"' % self.get_current_file_path())
 
         # Save any unsaved changes
         self.save_active_file(clear_after=True)
 
         # Toggle mode
         self.toggle_mode()
 
@@ -2670,17 +2483,23 @@
         Do not use `view_widget.setPlainText(html_data)` as it inherit styles from the prev view.
         """
         view_doc.setPlainText(source_data)
 
     def action_encrypt(self) -> None:
         """
         Action: Encrypt file data with symmetric encryption algorithm.
+
+        AES operates on blocks of 16 bytes. If there's no data (i.e., the data is an empty string or byte array),
+        the encryption function may not have anything to process, leading to unexpected behavior or errors.
+
+        Even if the input is an empty byte string (b''), Fernet will still produce a valid encrypted token.
+        This is because Fernet handles padding and other aspects internally.
         """
 
-        current_file_path = self.get_current_path()
+        current_file_path = self.get_current_file_path()
         if self.debug:
             self.logger.debug('Encrypting file "%s"' % current_file_path)
         # Save active file data if needed
         self.save_active_file(clear_after=False)
 
         # The file is already encrypted
         if self.is_file_encrypted(current_file_path):
@@ -2773,15 +2592,15 @@
             callback()
 
     def action_decrypt(self) -> None:
         """
         Action: Decrypt encrypted file data.
         """
 
-        current_file_path = self.get_current_path()
+        current_file_path = self.get_current_file_path()
         if self.debug:
             self.logger.debug('Decrypting file "%s"' % current_file_path)
         # Save active file data if needed
         self.save_active_file(clear_after=False)
 
         # The file is encrypted
         if not self.is_file_encrypted(current_file_path):
@@ -2951,14 +2770,20 @@
                 # TODO for each line after a paragraph and the line starting with ' > '
                 cursor.insertText('> ' + selected_text)
 
     def action_text_color_picker(self) -> None:
         """
         Action: Text format COLOR with a picker.
         """
+        if self.debug:
+            self.logger.debug('Color Picker dialog')
+
+        # Save any unsaved changes before calling a dialog
+        self.save_active_file(clear_after=False)
+
         self.color_picker = ColorPickerDialog(self)
         self.color_picker.color_selected.connect(self.text_color_picker_handler)
         # To update icon within toolbar before dialog
         self.create_icons_toolbar(refresh=True)
         # Run dialog
         self.color_picker.exec()
         # Unset dialog var
@@ -3007,14 +2832,17 @@
         """
         Action: AI assistant.
         """
 
         if self.debug:
             self.logger.debug('AI assistant')
 
+        # Save any unsaved changes before calling a dialog
+        self.save_active_file(clear_after=False)
+
         self.ai_assistant = AIAssistant(self)
         # To update icon within toolbar before dialog
         self.create_icons_toolbar(refresh=True)
         # Run dialog
         self.ai_assistant.exec()
         # Unset dialog var
         self.ai_assistant = None
@@ -3025,14 +2853,17 @@
         """
         Settings.
         """
 
         if self.debug:
             self.logger.debug('Settings dialog')
 
+        # Save any unsaved changes before calling a dialog
+        self.save_active_file(clear_after=False)
+
         settings = SettingsDialog(self)
         settings.exec()
 
     def action_check_for_updates(self) -> None:
         """
         Check the App updates here.
         """
@@ -3075,14 +2906,17 @@
         """
         Show about the App info.
         """
 
         if self.debug:
             self.logger.debug('About the App dialog')
 
+        # Save any unsaved changes before calling a dialog
+        self.save_active_file(clear_after=False)
+
         about = AboutPopup(self)
         about.exec()
 
     def action_exit(self) -> None:
         """
         Action: Exit from the app.
         """
@@ -3097,15 +2931,15 @@
 
     def action_nav_select_file(self, index) -> None:
         """
         Action: Open file selected from the tree view.
         """
 
         # Save any unsaved changes
-        self.save_active_file(clear_after=True)
+        self.save_active_file(clear_after=False)
 
         """
         Get file path by index:
             file_path = self.file_model.filePath(index)  # no proxy model
         Also, the file path can be obtained like this:
             file_path = self.tree_view.model().filePath(index)
         * https://doc.qt.io/qt-6/qsortfilterproxymodel.html#mapToSource
@@ -3162,15 +2996,15 @@
 
     def load_file(self, file_path: str) -> bool:
         """
         Helper: Load content of the file.
         """
 
         # Current file path and a new one can be the same but the MODE can differ
-        current_file_path = self.get_current_path()
+        current_file_path = self.get_current_file_path()
         # Update the tree and related indexes
         self.set_current_path(file_path)
 
         if current_file_path is not None and file_path != current_file_path:
             # Highlight the file to switch from
             in_transit_color = self.theme_helper.get_color('main_tree_file_highlighted_in_transit', True)
             self.file_model.highlight(self.file_model.index(current_file_path), os.path.basename(current_file_path),
@@ -3191,15 +3025,16 @@
             file_iterations = int(file_header.get_enc_param('itr'))
 
             try:
                 decrypted_data = (
                     self.get_encrypt_helper(
                         salt=file_salt, hint=file_header.get_enc_param('hint'),
                         iterations=file_iterations).decrypt_data(file_body.encode("utf-8")))
-                if decrypted_data:
+                # File content can be an empty string
+                if decrypted_data is not None and type(decrypted_data) is bytes:
                     file_body = decrypted_data.decode("utf-8")
                     self.set_encryption(Encryption.ENCRYPTED)
                 else:
                     if self.logging:
                         self.logger.info('Cannot decrypt file "%s"' % file_path)
                     """
                     * https://docs.python.org/3/reference/compound_stmts.html#the-try-statement
@@ -3209,29 +3044,33 @@
                 self.enc_password_dialog_cnt = 0
             except (InvalidToken, InvalidSignature, TypeError):
                 if self.debug:
                     self.logger.debug('Cannot apply encryption password!')
                 # Setup file's cursor position to a very beginning
                 self.settings.line_num = 0
                 self.settings.col_num = 0
+                # Set up password tries count
+                if self.get_enc_password_dialog_cnt() is None:
+                    self.enc_password_dialog_cnt = 0
                 # If currently opened file is encrypted then offer to change the password
                 if self.get_encryption() == Encryption.ENCRYPTED:
                     if self.debug:
                         self.logger.debug('Wrong encryption password but another encrypted file is opened')
                     if self.enc_password is not None:
                         # Show other file password mismatch message
                         self.message_box(self.lexemes.get('load_file_encryption_password_mismatch'), icon_type=2)
                         # If password not matched N-times, load default page then
                         if self.get_enc_password_dialog_cnt() >= 3:
                             # Reset encryption helper
                             self.reset_encrypt_helper()
                             # Reset encryption password dialogue count
                             self.enc_password_dialog_cnt = 0
                             # Mind possible recursion
-                            return self.load_default_page(ignore_settings=True)
+                            # return self.load_default_page(ignore_settings=True)
+                            return False
                         elif self.get_enc_password_dialog_cnt() > 0:
                             # Do not ask confirmation to reset the password as it has been confirmed already
                             self.reset_encrypt_helper()
                         else:
                             """
                             Ask to reset current password that in use by currently opened file.
                             Try to load the file by switch to it if the encryption password has been reset.
@@ -3249,52 +3088,55 @@
                         self.set_current_path(current_file_path)
 
                     # Try to re-load file if encryption password has been reset
                     if self.enc_password is None:
                         # Try to re-load file after encryption password reset
                         if file_path != current_file_path:
                             return self.load_file(file_path)
-                # Show error message and reset password only if the password set
+                # If current file is not encrypted.
+                # Show error message and reset password only if the password set.
                 elif self.enc_password is not None:
                     # Reset encryption helper and password
                     self.reset_encrypt_helper()
                     # Show file password mismatch message
                     self.message_box(self.lexemes.get('load_file_encryption_password_incorrect'), icon_type=3)
                     # If password not matched N-times, load default page then
                     if self.get_enc_password_dialog_cnt() >= 3:
                         # Reset encryption password dialogue count
                         self.enc_password_dialog_cnt = 0
                         # Mind possible recursion
-                        return self.load_default_page(ignore_settings=True)
+                        # return self.load_default_page(ignore_settings=True)
+                        return False
                     # Revert back the tree index if one was set previously
                     if (current_file_path is not None
                             # To avoid cycle between encrypted files when trying to return to a prev file
                             # with an empty password
                             and not self.is_file_encrypted(current_file_path)):
                         self.set_current_path(current_file_path)
                         # Try to re-load file after encryption password reset
                         if file_path != current_file_path:
                             return self.load_file(file_path)
                     else:
                         # Mind possible recursion
                         return self.load_default_page(ignore_settings=True)
                 else:
-                    self.reset_encrypt_helper() # Reset encryption helper and password
+                    self.reset_encrypt_helper()  # Reset encryption helper and password
                     if self.debug:
                         self.logger.debug('Do nothing with the wrong password but check the loaded page')
                     """
                     Just to be sure the editor is not started on encrypted file
                     with cancelled password dialog on very beginning, or without any default file.
                     Revert back the tree index if one was set previously.
                     """
                     if (current_file_path is not None
                             # To avoid cycling between encrypted files when trying to return to a prev file
                             # with no or empty password.
                             and not self.is_file_encrypted(current_file_path)):
-                        return self.load_file(current_file_path)
+                        # return self.load_file(current_file_path)
+                        return False
                     else:
                         # Mind possible recursion
                         return self.load_default_page(ignore_settings=True)
 
                 if current_file_path is not None:
                     # Remove highlighted background
                     default_color = self.theme_helper.get_color('main_tree_background', True)
@@ -3348,24 +3190,25 @@
             # View widget
             view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
             selected_text = view_widget.textCursor().selectedText()
 
         if self.debug:
             self.logger.debug('Searching text "%s"' % selected_text)
 
-        self.search_input.setText(selected_text)
-        self.search_input.setFocus()
+        if hasattr(self.toolbar, 'search_input'):
+            self.toolbar.search_input.setText(selected_text)
+            self.toolbar.search_input.setFocus()
         self.action_search_next()
 
     def reload_active_file(self) -> None:
         """
         Re-load current file's content.
         Save any unsaved changes before calling this file reload method!
         """
-        current_file_path = self.get_current_path()
+        current_file_path = self.get_current_file_path()
 
         if self.debug:
             self.logger.debug('Re-loading current file content "%s"' % current_file_path)
 
         self.load_file(current_file_path)
 
     def auto_save_file(self, file_path: str = None) -> None:
@@ -3392,23 +3235,24 @@
         @param clear_after: bool, clear edit field after saving (when applicable, say switching view mode)
         @param allow_save_empty_content: bool, dialog answer of either to allow to save an empty file or not
         @return: None
         """
 
         # Save cursor position (line count starts from 0)
         self.store_doc_cursor_pos(self.get_mode())
-        # Get current file path
-        current_file_path = self.get_current_path()
 
         if self.get_mode() != Mode.EDIT:
             # Nothing to save
             if self.debug:
                 self.logger.debug('Nothing to save in a non-edit mode')
             return
 
+        # Get current file path
+        current_file_path = self.get_current_file_path()
+
         # The dialog about empty content was shown at least once
         if allow_save_empty_content is not None:
             self.estate.allow_save_empty = allow_save_empty_content
 
         if self.debug:
             self.logger.debug(f"Save active file '{current_file_path}' (clear field after: '{clear_after}')")
 
@@ -3436,24 +3280,24 @@
 
             # Save if any changes
             if (file_content or self.estate.allow_save_empty) and self.content != file_content:
                 # Show saving progress in the status bar
                 if hasattr(self, 'statusbar'):
                     self.statusbar['save_progress_label'].setVisible(True)
                 # Grayscale save button(s) at the toolbar
-                if hasattr(self, 'toolbar_save_button'):
-                    self.toolbar_save_button.setDisabled(True)
+                if hasattr(self.toolbar, 'toolbar_save_button'):
+                    self.toolbar.toolbar_save_button.setDisabled(True)
 
-                    def restore_saving_ui_state() -> None:
-                        if hasattr(self, 'statusbar'):
-                            self.statusbar['save_progress_label'].setVisible(False)
-                        # Keep it switched off to explicitly show the nothing to save state
-                        # self.toolbar_save_button.setEnabled(True)
-                    # Restore saving UI state automatically.
-                    QTimer.singleShot(1500, restore_saving_ui_state)
+                def restore_saving_ui_state() -> None:
+                    if hasattr(self, 'statusbar'):
+                        self.statusbar['save_progress_label'].setVisible(False)
+                    # Keep it switched off to explicitly show the nothing to save state
+                    # self.toolbar.toolbar_save_button.setEnabled(True)
+                # Restore saving UI state automatically.
+                QTimer.singleShot(1500, restore_saving_ui_state)
 
                 if self.header is None or not self.header.is_valid():
                     # Get empty file header here, it's needed for compatibility and will not be applied to the file
                     header = FileHeader()
                     if self.logging:
                         self.logger.info('File "%s" has no header info' % current_file_path)
                 else:
@@ -3491,16 +3335,16 @@
                     # Clear field's data
                     if clear_after:
                         edit_widget.clear()
                 else:
                     self.message_box(self.lexemes.get('save_active_file_error_occurred'), icon_type=2)
 
             # Grayscale save button at the toolbar
-            if hasattr(self, 'toolbar_save_button'):
-                self.toolbar_save_button.setDisabled(True)
+            if hasattr(self.toolbar, 'toolbar_save_button'):
+                self.toolbar.toolbar_save_button.setDisabled(True)
 
     def toggle_mode(self) -> None:
         """
         Helper: Switch between VIEW and EDIT modes to maintain actual state.
         """
         self.estate.toggle_mode()
 
@@ -3557,20 +3401,19 @@
         Helper: Default page when nothing else to show.
         """
         if (not ignore_settings
                 and self.settings.file_path is not None
                 and os.path.isfile(self.settings.file_path)):
             file_path = self.settings.file_path
         else:
-            # Default README.md file should be in the package
-            file_path = resource_filename('notolog', 'README.md')
+            script_dir = os.path.dirname(os.path.realpath(__file__))
+            parent_dir = os.path.dirname(script_dir)
+            file_path = os.path.join(parent_dir, 'README.md')
             # Fallback option
             if not os.path.isfile(file_path):
-                script_dir = os.path.dirname(os.path.realpath(__file__))
-                parent_dir = os.path.dirname(script_dir)
                 file_path = os.path.join(parent_dir, 'docs', 'Examples.md')
             # file_path = res_path('README.md')  # Not working well with venv
         # If no file exist then try to load any file
         if file_path is not None and not os.path.isfile(file_path):
             file_path = self.get_any_file()
         if file_path is not None:
             return self.load_file(file_path)
@@ -3606,15 +3449,15 @@
                 Unregistering is not necessary when extension can be reset.
                 self.md.postprocessors.deregister(name='footnote')
                 self.md.inlinePatterns.deregister('footnote')
                 """
                 for _ext in self.md.registeredExtensions:
                     if _ext and 'FootnoteExtension' in str(_ext):
                         # Without this the extension tends to keep footnotes across the various notes
-                        _ext.reset()
+                        _ext.reset()  # type: ignore
                         # To remove use: self.md.registeredExtensions.remove(_ext)
                         if self.debug:
                             self.logger.debug('Resetting extension "%s"' % _ext)
                         break
             except ValueError as e:
                 if self.logging:
                     self.logger.warning('Extension error', e)
@@ -3631,33 +3474,158 @@
         # Connecting view's mouse press event to the view processor's method
         view_widget.mousePressEvent = view_processor.mouse_click_event
         # Processing changes of the document passed within
         view_processor.process()
 
         """
         There is also possible to update QTextEdit with html:
-        view_widget.setHtml(HTML_TPL % (title, css_data, updated_doc.toHtml()))
+        view_widget.setHtml(self.HTML_TPL % (title, css_data, view_doc.toPlainText()))
         Or update and set up document itself:
         view_widget.setDocument(updated_doc)
         """
-        view_doc.setHtml(HTML_TPL % (title, css_data, view_doc.toPlainText()))
+        view_doc.setHtml(self.HTML_TPL % (title, css_data, view_doc.toPlainText()))
+
+        # TODO do not process twice
+        # Extract string image resources from the document, download and append
+        self.process_document_images(view_doc)
+        """
+        # Load resource from the document
+        res = view_doc.loadResource(QTextDocument.ResourceType.ImageResource, image_url)
+        """
 
         """
         View decorator to modify result text.
         Highlighter object holds the document and may pass it through indirectly.
         """
         vew_decorator = ViewDecorator(highlighter=self.view_highlighter)
         # Processing changes of the document passed within
         vew_decorator.process()
 
         # Set or restore cursor position here. View processors above should preserve the cursor state.
         cursor = view_widget.textCursor()
         cursor.movePosition(QTextCursor.MoveOperation.Start)  # Or just: cursor.setPosition(0)
         view_widget.setTextCursor(cursor)
 
+    def is_resource_attached(self, resource_url: str) -> bool:
+        """
+        Check either resource attached to the document or not.
+        """
+        # View document
+        view_doc = self.get_view_doc()  # type: QTextDocument
+        # Try to find resource attached to the document
+        resource = view_doc.resource(QTextDocument.ResourceType.ImageResource, QUrl(resource_url))
+        if resource:
+            if self.debug:
+                self.logger.debug(f"Resource for {resource_url} is already added.")
+            return True
+        else:
+            if self.debug:
+                self.logger.debug(f"No resource found for {resource_url}.")
+            return False
+
+    def attach_resource(self, resource_name: str, pixmap: QPixmap) -> bool:
+        """
+        Attach pixmap resource to the document.
+        """
+        # View document
+        view_doc = self.get_view_doc()  # type: QTextDocument
+        # url and pixmap data
+        view_doc.addResource(QTextDocument.ResourceType.ImageResource, resource_name, pixmap)
+        if self.debug:
+            self.logger.debug(f"Resource '{resource_name}' added to the document")
+        return True
+
+    def get_cached_resource_pixmap(self, image_url) -> QPixmap:
+        # Convert url to local file name
+        file_name = self.resource_downloader.url_to_filename(image_url)
+        res_folder = self.resource_downloader.get_resource_folder(self.get_active_dir())
+        file_path = os.path.join(res_folder.path(), file_name)
+        if self.debug:
+            self.logger.debug(f"Resource url '{image_url}', local file '{file_path}'")
+        # Check if the image is already downloaded and cached
+        pixmap = QPixmap()
+        if QPixmapCache.find(image_url, pixmap):
+            if self.debug:
+                self.logger.debug(f"Pixmap resource found in cache: {image_url}")
+        elif os.path.exists(file_path):
+            # Load from disk and cache
+            pixmap.load(file_path)
+            QPixmapCache.insert(image_url, pixmap)
+            if self.debug:
+                self.logger.debug(f"Loaded from disk and cached: {image_url}")
+        else:
+            if self.logging:
+                self.logger.warning(f"Resource's '{image_url}' file doesn't exist '{file_path}'")
+        return pixmap
+
+    @Slot()
+    def resource_downloaded_handler(self, data) -> None:
+        if 'resource_name' not in data:
+            if self.logging:
+                self.logger.warning(f'Wrong data for added resource: {data}')
+            return
+        image_url = data['resource_name']
+        # Get cached resource data as handler should process an update
+        pixmap = self.get_cached_resource_pixmap(image_url)
+        if not pixmap.isNull():
+            # Attach resource
+            self.attach_resource(image_url, pixmap)
+        else:
+            if self.logging:
+                self.logger.warning(f"Resource '{image_url}' data not found")
+
+    @Slot()
+    def resource_downloader_finished_handler(self):
+        if self.debug:
+            self.logger.debug(f"All resource downloader tasks have been completed")
+        # View widget
+        view_widget = self.get_view_widget()  # type: Union[ViewWidget, QTextBrowser]
+        # Re-set up view's (or document's) content to get the added resources shown
+        view_widget.setHtml(view_widget.toHtml())
+
+    def process_document_images(self, text_document):
+        """
+        Extract image urls from the given document
+        """
+
+        # Init image downloader instance
+        if self.resource_downloader is None:
+            self.resource_downloader = ImageDownloader()
+            self.resource_downloader.downloaded.connect(self.resource_downloaded_handler)  # Single resource downloaded
+            self.resource_downloader.finished.connect(self.resource_downloader_finished_handler)  # All tasks finished
+
+        block = text_document.begin()
+        # Check doc's block
+        while block.isValid():
+            it = block.begin()
+            while not it.atEnd():
+                fragment = it.fragment()
+                if fragment.isValid():
+                    image_format = fragment.charFormat().toImageFormat()
+                    # Valid image
+                    if image_format.isValid():
+                        image_url = image_format.name()
+                        if self.debug:
+                            self.logger.debug(f"Found image resource url: {image_url}")
+                        # Check if the resource has been already added
+                        if not self.is_resource_attached(image_url):
+                            # Try to get cached resource data
+                            pixmap = self.get_cached_resource_pixmap(image_url)
+                            # Download if not found
+                            if pixmap.isNull():
+                                self.resource_downloader.download_resource_in_queue(image_url)
+                            else:
+                                # Attach resource
+                                self.attach_resource(image_url, pixmap)
+                        else:
+                            if self.debug:
+                                self.logger.debug(f"Resource is already attached: {image_url}")
+                it += 1
+            block = block.next()
+
     def load_content_edit(self, header: FileHeader, content: str) -> None:
         """
         Load and setup content fields for EDIT mode.
         Keep in mind: document's content re-highlighting happens by event, e.g. at on_modification_changed()
         """
 
         # Edit widget
@@ -3707,15 +3675,14 @@
                                           view_widget.verticalScrollBar().value()]
 
     def restore_doc_cursor_pos(self, mode: Mode, source_widget: Union[QPlainTextEdit, QTextBrowser]):
         """
         Move cursor to stored position or defaults.
         Make sure the method called once on startup or cursor will be moved again.
         """
-
         if mode == Mode.EDIT:
             text_cursor = source_widget.textCursor()
             text_cursor.setPosition(0)
             if self.debug:
                 self.logger.debug('Restoring document cursor position %d x %d'
                                   % (self.settings.line_num, self.settings.col_num))
             # Move down to the desired line number (assuming line numbers start from 0)
@@ -3750,40 +3717,45 @@
         self.settings.viewport_pos = [0, 0]
 
     def action_search_on(self) -> None:
         """
         Search: Started; related actions.
         Could be called upon input field's textChanged event.
         """
-        text = self.search_input.text()
-
-        if len(text) > 0:
-            self.btn_search_clear.setEnabled(True)
-            self.btn_search_next.setEnabled(True)
-            self.btn_search_prev.setEnabled(True)
+        text = ''
+        if hasattr(self.toolbar, 'search_input'):
+            text = self.toolbar.search_input.text()
+
+        if len(text) > 0 and hasattr(self.toolbar, 'btn_search_clear'):
+            self.toolbar.btn_search_clear.setEnabled(True)
+            self.toolbar.btn_search_next.setEnabled(True)
+            self.toolbar.btn_search_prev.setEnabled(True)
         else:
             self.action_search_clear()
 
     def action_search_off(self) -> None:
         """
         Search: Stopped; related actions.
         Could be called upon search clear action which could be called upon input field's 'textChanged' event
         in their turn.
         """
-        self.btn_search_clear.setEnabled(False)
-        self.btn_search_next.setEnabled(False)
-        self.btn_search_prev.setEnabled(False)
+        if hasattr(self.toolbar, 'btn_search_clear'):
+            self.toolbar.btn_search_clear.setEnabled(False)
+            self.toolbar.btn_search_next.setEnabled(False)
+            self.toolbar.btn_search_prev.setEnabled(False)
 
     def action_search_clear(self) -> None:
         """
         Search field set to an empty text and reset the search state.
         """
-        self.search_input.setText('')
-        # Case-sensitive checkbox
-        self.search_match_case.setCheckState(Qt.CheckState.Unchecked)
+        if hasattr(self.toolbar, 'search_input'):
+            self.toolbar.search_input.setText('')
+        if hasattr(self.toolbar, 'search_match_case'):
+            # Case-sensitive checkbox
+            self.toolbar.search_match_case.setCheckState(Qt.CheckState.Unchecked)
         # Reset buttons state
         self.action_search_off()
         # Get source of the search
         if self.get_mode() == Mode.EDIT:
             # Edit widget
             edit_widget = self.get_edit_widget()  # type: Union[EditWidget, QPlainTextEdit]
             search_source = edit_widget
@@ -3801,16 +3773,20 @@
         search_source.find('')  # Search a void
 
     def action_search_prev(self) -> None:
         """
         Search: Previous occurrence of string in text (Backward search)
         * https://doc.qt.io/qt-6/qtextdocument.html#FindFlag-enum
         """
-        text = self.search_input.text()
-        check = self.search_match_case.isChecked()
+        text = ''
+        if hasattr(self.toolbar, 'search_input'):
+            text = self.toolbar.search_input.text()
+        check = False
+        if hasattr(self.toolbar, 'search_match_case'):
+            check = self.toolbar.search_match_case.isChecked()
         # Case-sensitive option
         if check:
             find_flags = (QTextDocument.FindFlag.FindBackward | QTextDocument.FindFlag.FindCaseSensitively)
         else:
             find_flags = QTextDocument.FindFlag.FindBackward
         # Find text with correct flags
         if self.get_mode() == Mode.EDIT:
@@ -3832,16 +3808,20 @@
             search_source.find(text, find_flags)
 
     def action_search_next(self) -> None:
         """
         Search: Next occurrence of string in text (Forward search; Default)
         * https://doc.qt.io/qt-6/qtextdocument.html#FindFlag-enum
         """
-        text = self.search_input.text()
-        check = self.search_match_case.isChecked()
+        text = ''
+        if hasattr(self.toolbar, 'search_input'):
+            text = self.toolbar.search_input.text()
+        check = False
+        if hasattr(self.toolbar, 'search_match_case'):
+            check = self.toolbar.search_match_case.isChecked()
         # Case-sensitive option
         if check:
             find_flags = QTextDocument.FindFlag.FindCaseSensitively
         else:
             find_flags = QTextDocument.FindFlag(0)
         # Find text with correct flags
         if self.get_mode() == Mode.EDIT:
```

### Comparing `notolog-0.9.0b10/app/text_block_data.py` & `notolog-0.9.0b11/app/text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/theme.py` & `notolog-0.9.0b11/app/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class Theme:
 
     ASSETS_DIR_NAME = "assets"
 
     _instance = None
 
     def __new__(cls, *args, **kwargs):
-        if cls._instance is None:
+        if cls._instance is None or AppConfig.get_test_mode():  # No cache in test mode
             cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(self, theme: str = None):
         # Load exact theme once
         if getattr(self, 'theme', None) and self.theme == theme:
             return
```

### Comparing `notolog-0.9.0b10/app/ui/about_popup.py` & `notolog-0.9.0b11/app/ui/about_popup.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,19 +42,25 @@
         self.theme_helper = ThemeHelper()
 
         self.init_ui()
 
         self.setModal(True)  # Set the dialog modal to manage focus more effectively
 
         # self.adjustSize()  # Adjust size based on content
+        """
         main_window_size = self.parent.size()
         dialog_width = int(main_window_size.width() * 0.25)
         dialog_height = int(main_window_size.height() * 0.25)
         # Set dialog size derived from the main window size
         self.setMinimumSize(dialog_width, dialog_height)
+        """
+
+        self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        if self.sizeHint().isValid():
+            self.setMinimumSize(self.sizeHint())
 
     def init_ui(self):
         self.setWindowTitle(self.lexemes.get('popup_about_title'))
 
         layout = QVBoxLayout(self)
         self.setLayout(layout)
 
@@ -95,14 +101,16 @@
         info_fields = [
             (self.lexemes.get('popup_about_version'), AppConfig.get_app_version(), []),
             (self.lexemes.get('popup_about_license'), AppConfig.get_app_license(), []),
             (self.lexemes.get('popup_about_website'), AppConfig.get_app_website(),
              [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig.get_app_website()}]),
             (self.lexemes.get('popup_about_repository'), AppConfig.get_app_repository(),
              [{'icon': 'star-fill.svg', 'link': AppConfig.get_app_repository()}]),
+            (self.lexemes.get('popup_about_pypi'), AppConfig.get_app_pypi(),
+             [{'icon': 'box-arrow-up-right.svg', 'link': AppConfig.get_app_pypi()}]),
             (self.lexemes.get('popup_about_date'), AppConfig.get_app_date(), [])
         ]
 
         for i, row in enumerate(info_fields):
             label, value, value_icons = row
             # Label widget
             label_widget = QLabel(f"{label}:", self)
```

### Comparing `notolog-0.9.0b10/app/ui/ai_assistant.py` & `notolog-0.9.0b11/app/ui/ai_assistant.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/color_picker_dialog.py` & `notolog-0.9.0b11/app/ui/color_picker_dialog.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/common_dialog.py` & `notolog-0.9.0b11/app/ui/common_dialog.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PySide6.QtCore import Qt
-from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox
+from PySide6.QtWidgets import QDialog, QLabel, QVBoxLayout, QDialogButtonBox, QSizePolicy
 from PySide6.QtGui import QFontMetrics
 
 from ..app_config import AppConfig
 
 import logging
 
 
@@ -22,19 +22,24 @@
 
         self.logger = logging.getLogger('common_dialog')
 
         self.setWindowTitle(str(title))
         self.setObjectName('common_dialog')
 
         # Set dialog size derived from the main window size
+        """
         main_window_size = parent.size()
         # Will be adjusted with size hint later at resizeEvent()
         dialog_width = int(main_window_size.width() * 0.33)
         dialog_height = int(main_window_size.height() * 0.33)
         self.resize(dialog_width, dialog_height)
+        """
+        self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        if self.sizeHint().isValid():
+            self.setMinimumSize(self.sizeHint())
 
         label = QLabel()
         label.setObjectName('common_label')
         label.setMargin(10)  # Set vertical padding for the dialog label
         label.setText(str(text))
         label.setAlignment(Qt.AlignmentFlag.AlignCenter)
         label.adjustSize()
```

### Comparing `notolog-0.9.0b10/app/ui/enum_combo_box.py` & `notolog-0.9.0b11/app/ui/enum_combo_box.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,30 @@
 
 
 class EnumComboBox(QComboBox):
     def __init__(self, enum_class):
         super().__init__()
         self._enum_class = enum_class
 
+        # Sort the Enum members by value
+        # sorted_members = sorted(enum_class, key=lambda x: x.value)
+
         # Load the Enum values
-        for enum_value in enum_class:
+        for enum_value in enum_class:  # Or: sorted_members
             self.addItem(enum_value.value, userData=enum_value)
 
+            # Add separator. It also adds extra index to the QComboBox
+            # if hasattr(enum_value, 'is_default') and enum_value.is_default:
+            #    self.insertSeparator(i + 1)
+
             # Check if the current item is a legacy item
             if hasattr(enum_value, 'legacy') and enum_value.legacy:
                 # Get the index of the item we just added
                 index = self.count() - 1
                 # Set a custom style for legacy items (e.g., gray text color)
-                self.setItemData(index, QColor('red'), Qt.ItemDataRole.ForegroundRole)
+                self.setItemData(index, QColor('gray'), Qt.ItemDataRole.ForegroundRole)
                 # Alternatively, disable the item if you don't want it selectable
                 # self.model().item(index).setEnabled(False)
 
     @property
     def enum_class(self):
         return self._enum_class
```

### Comparing `notolog-0.9.0b10/app/ui/file_system_model.py` & `notolog-0.9.0b11/app/ui/file_system_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/line_numbers.py` & `notolog-0.9.0b11/app/ui/line_numbers.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/rename_file_dialog.py` & `notolog-0.9.0b11/app/ui/rename_file_dialog.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from PySide6.QtCore import Signal, QSize
-from PySide6.QtWidgets import QInputDialog, QLineEdit, QDialogButtonBox
+from PySide6.QtWidgets import QInputDialog, QLineEdit, QDialogButtonBox, QSizePolicy
 
 from ..settings import Settings
 from ..enums.colors import Colors
 from ..app_config import AppConfig
 from ..lexemes.lexemes import Lexemes
 
 import logging
@@ -42,14 +42,18 @@
         self.setInputMode(QInputDialog.InputMode.TextInput)
         self.setTextEchoMode(QLineEdit.EchoMode.Normal)
         self.setWindowTitle(self.lexemes.get('dialog_file_rename_title'))
         self.setLabelText(self.lexemes.get('dialog_file_rename_field_label'))
         self.setOkButtonText(self.lexemes.get('dialog_file_rename_button_ok'))
         self.setTextValue(self.file_name)
 
+        self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        if self.sizeHint().isValid():
+            self.setMinimumSize(self.sizeHint())
+
         # Set dialog size derived from the main window size
         main_window_size = self.parent.size()
         dialog_width = int(main_window_size.width() * 0.33)
         dialog_height = int(main_window_size.height() * 0.33)
         self.resize(dialog_width, dialog_height)
 
         """
```

### Comparing `notolog-0.9.0b10/app/ui/rotating_label.py` & `notolog-0.9.0b11/app/ui/rotating_label.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/settings_dialog.py` & `notolog-0.9.0b11/app/ui/settings_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,18 @@
         self.debug = AppConfig.get_debug()
 
         # Default language setup, change to settings value to modify it via UI
         self.lexemes = Lexemes(self.settings.app_language, default_scope='settings_dialog')
 
         self.setWindowTitle(self.lexemes.get('window_title'))
 
+        self.setSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Minimum)
+        if self.sizeHint().isValid():
+            self.setMinimumSize(self.sizeHint())
+
         # Set dialog size derived from the main window size
         main_window_size = self.parent.size()
         dialog_width = int(main_window_size.width() * 0.33)
         dialog_height = int(main_window_size.height() * 0.33)
         self.setMinimumSize(dialog_width, dialog_height)
 
         # Tabs widget as a main one
@@ -100,26 +104,26 @@
              "text": self.lexemes.get('general_app_config_label'), "style": {"bold": True},
              "callback": lambda obj: tab_general_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop)},
             # Available languages label
             {"type": QLabel, "name": "settings_dialog_general_app_language_label", "alignment": Qt.AlignmentFlag.AlignLeft,
              "text": self.lexemes.get('general_app_language_label'),
              "callback": lambda obj: tab_general_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop)},
             # Available languages dropdown list
-            {"type": EnumComboBox, "args": [Languages],
+            {"type": EnumComboBox, "args": [sorted(Languages, key=lambda member: (not member.is_default, member.value))],
              "name": "settings_dialog_general_app_language_combo:app_language",  # Lexeme key : Object name
              "callback": lambda obj: tab_general_layout.addWidget(obj),
              "placeholder_text": self.lexemes.get('general_app_language_combo_placeholder_text'),
              "accessible_description":
                  self.lexemes.get('app_language_combo_accessible_description')},
             # Available themes label
             {"type": QLabel, "name": "settings_dialog_general_app_theme_label", "alignment": Qt.AlignmentFlag.AlignLeft,
              "text": self.lexemes.get('general_app_theme_label'),
              "callback": lambda obj: tab_general_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop)},
             # Available themes dropdown list
-            {"type": EnumComboBox, "args": [Themes],
+            {"type": EnumComboBox, "args": [sorted(Themes, key=lambda member: (not member.is_default, member.value))],
              "name": "settings_dialog_general_app_theme_combo:app_theme",  # Lexeme key : Object name
              "callback": lambda obj: tab_general_layout.addWidget(obj),
              "placeholder_text": self.lexemes.get('general_app_theme_combo_placeholder_text'),
              "accessible_description":
                  self.lexemes.get('general_app_theme_combo_accessible_description')},
             # Horizontal spacer
             {"type": self.layout_horizontal_spacer, "args": [tab_general_layout]},
@@ -218,14 +222,25 @@
             {"type": QCheckBox,
              # Lexeme key : Object name
              "name": "settings_dialog_viewer_config_open_link_confirmation_checkbox:viewer_open_link_confirmation",
              "callback": lambda obj: tab_viewer_config_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop),
              "text": self.lexemes.get('viewer_config_open_link_confirmation_checkbox'),
              "accessible_description":
                  self.lexemes.get('viewer_config_open_link_confirmation_checkbox_accessible_description')},
+            # Spacer
+            {"type": QWidget, "name": None, "size_policy": (QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum),
+             "callback": lambda obj: tab_viewer_config_layout.addWidget(obj)},
+            # Auto save downloaded resources on disk
+            {"type": QCheckBox,
+             # Lexeme key : Object name
+             "name": "settings_dialog_viewer_config_save_resources_checkbox:viewer_save_resources",
+             "callback": lambda obj: tab_viewer_config_layout.addWidget(obj, alignment=Qt.AlignmentFlag.AlignTop),
+             "text": self.lexemes.get('viewer_config_save_resources_checkbox'),
+             "accessible_description":
+                 self.lexemes.get('viewer_config_save_resources_checkbox_accessible_description')},
             # Spacer to keep elements above on top
             {"type": QWidget, "name": None, "size_policy": (QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding),
              "callback": lambda obj: tab_viewer_config_layout.addWidget(obj)},
 
             # [AI config]
             # OpenAI API block label
             {"type": QLabel, "name": "settings_dialog_ai_config_openai_api_label", "alignment": Qt.AlignmentFlag.AlignLeft,
@@ -329,19 +344,17 @@
         Method to create setting field with ease.
         @param conf: Config of the field. As the param bounded to the particular method it will be called then.
         @return: Any object instance
         """
         args = conf['args'] if 'args' in conf else [self]
         obj = conf['type'](*args)  # type: conf['type']
         # Align with the dialog font size (mostly for QLabel)
-        if hasattr(obj, 'sizeHint'):
-            """
-            # Also possible to set the font directly:
+        if hasattr(obj, 'setFont'):
             obj.setFont(self.font())
-            """
+        if hasattr(obj, 'sizeHint'):
             obj.sizeHint()
         # Apply methods from props
         if 'props' in conf:
             self.apply_props(obj, conf['props'])
         if 'name' in conf and conf['name']:
             """
             Let's set up object name to make it easier to understand any further callbacks later.
@@ -588,28 +601,32 @@
             # Update self styles
             self.setStyleSheet(self.theme_helper.get_css('settings_dialog'))
 
         if setting_name == 'app_font_size' or sender.objectName().endswith('app_font_size'):
             # Update font from parent as it should be updated and incorporates new font size as well.
             # Simple update of the font size should also work.
             self.setFont(self.parent.font())
-            # Find all QLabel objects
-            found_objects = self.findChildren(QLabel)
-            for obj in found_objects:
-                # Align with the dialog font size (mostly for QLabel)
-                if hasattr(obj, 'sizeHint'):
-                    obj.setFont(self.font())
-                if obj.objectName() == "settings_dialog_general_app_font_size_label":
-                    """
-                    # Update the font weight of the label
-                    font = QFont()
-                    font.setPointSize(setting_value)
-                    app_font_size_label.setFont(font)
-                    """
-                    obj.setText(self.lexemes.get('general_app_font_size_label', size=setting_value))
+            widgets_to_update = [QLabel, QTabWidget, QPushButton, QCheckBox, QLineEdit, QPlainTextEdit, QComboBox,
+                                 QSpinBox, QSlider]
+            for _widget in widgets_to_update:
+                # Find all QLabel objects
+                found_objects = self.findChildren(_widget)
+                for obj in found_objects:
+                    # Align with the dialog font size (mostly for QLabel)
+                    if hasattr(obj, 'setFont'):
+                        # obj.sizeHint()
+                        obj.setFont(self.font())
+                    if obj.objectName() == "settings_dialog_general_app_font_size_label":
+                        """
+                        # Update the font size on the label
+                        font = QFont()
+                        font.setPointSize(setting_value)
+                        app_font_size_label.setFont(font)
+                        """
+                        obj.setText(self.lexemes.get('general_app_font_size_label', size=setting_value))
 
     def set_tab_text(self, object_name, text):
         # Iterate through all the tabs
         for index in range(self.tab_widget.count()):
             # Get the widget for the current index
             widget = self.tab_widget.widget(index)
```

### Comparing `notolog-0.9.0b10/app/ui/sort_filter_proxy_model.py` & `notolog-0.9.0b11/app/ui/sort_filter_proxy_model.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/ui/statusbar.py` & `notolog-0.9.0b11/app/ui/statusbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 
 class StatusBar(QStatusBar):
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.parent = parent
 
-        # Apply font from the dialog instance to the label
-        self.setFont(self.parent.font())
+        if self.parent and hasattr(self.parent, 'font'):
+            # Apply font from the dialog instance to the label
+            self.setFont(self.parent.font())
 
         self.logger = logging.getLogger('statusbar')
 
         self.logging = AppConfig.get_logging()
         self.debug = AppConfig.get_debug()
 
         self.settings = Settings(parent=self)
```

### Comparing `notolog-0.9.0b10/app/view_decorator.py` & `notolog-0.9.0b11/app/view_decorator.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/app/view_processor.py` & `notolog-0.9.0b11/app/view_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
                 cursor.clearSelection()
                 parent_widget.setTextCursor(cursor)
 
     def anchor_click_event(self, url: QUrl, cursor: QTextCursor):
         if self.debug:
             # cursor.charFormat().anchorHref()
-            self.logger.info('Anchor clicked, scheme: %s, path: %s' % (url.scheme(), url.path()))
+            self.logger.debug('Anchor clicked, scheme: %s, path: %s' % (url.scheme(), url.path()))
 
         # This may cause left-right click issue when either the start or end position of token is clicked
         # cursor.movePosition(QTextCursor.MoveOperation.PreviousCharacter, QTextCursor.MoveMode.KeepAnchor)
 
         cursor.select(QTextCursor.SelectionType.WordUnderCursor)
 
         if self.debug:
@@ -319,16 +319,19 @@
 
         i = 0
         # Move to the anchor caption's start position
         while cursor.charFormat().isAnchor() and (i := i + 1):
             cursor.movePosition(QTextCursor.MoveOperation.PreviousCharacter, QTextCursor.MoveMode.MoveAnchor)
         # Move to the anchor caption's end position
         while i > 0 or cursor.charFormat().isAnchor():
-            cursor.movePosition(QTextCursor.MoveOperation.NextCharacter, QTextCursor.MoveMode.KeepAnchor)
             i -= 1
+            cursor.movePosition(QTextCursor.MoveOperation.NextCharacter, QTextCursor.MoveMode.KeepAnchor)
+            # Check it after, not in loop
+            if cursor.atBlockEnd():
+                break
 
         anchor_label = cursor.selectedText()
         if self.debug:
             self.logger.debug('Anchor text: %s' % anchor_label)
 
         cursor.removeSelectedText()
         to_decode = url.path()
```

### Comparing `notolog-0.9.0b10/app/view_widget.py` & `notolog-0.9.0b11/app/view_widget.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,8 +66,13 @@
         """
         # Optionally add new actions or modify existing ones
         customAction = menu.addAction("Custom Action")
         customAction.triggered.connect(self.custom_action_triggered)
         """
 
         # Display the menu
-        menu.exec_(event.globalPos())
+        menu.exec_(event.globalPos())
+
+    def loadResource(self, type, url):
+        # Log the resource request
+        if self.debug:
+            self.logger.debug(f"Requesting resource of type {type} at URL: {url.toString()}")
```

### Comparing `notolog-0.9.0b10/main.py` & `notolog-0.9.0b11/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-"""
-Notolog main file to start up the app and to set up an async loop.
+# Notolog
+# An open-source markdown editor written in Python.
+
+# Main file to start up the app and to set up an async loop.
 
+"""
 This module is the main entry point for the Notolog app. It handles the initialization of the
 application environment, processes command line arguments, and starts the main application loop.
 
 Detailed Description:
 - Initializes the GUI by calling the main module.
 - Set up global logging and debug settings.
 - Initializes the async loop.
 
 Usage:
 Run the module directly from the command line with the necessary arguments:
 python3 main.py
+"""
 
-GitHub Repository: https://github.com/notolog/notolog-editor
+# - GitHub Repository: https://github.com/notolog/notolog-editor
+# - PyPI: https://pypi.org/project/notolog
+# - WebSite: https://notolog.app
+# - Author: Vadim Bakhrenkov
+# - Copyright 2024 Vadim Bakhrenkov
+# - License: MIT License
 
-Author: Vadim Bakhrenkov
-License: MIT License
-"""
 
 from PySide6.QtWidgets import QStyleFactory
 from qasync import QEventLoop, QApplication
 
 from app.app_config import AppConfig
 from app.notolog_editor import NotologEditor
```

### Comparing `notolog-0.9.0b10/notolog.egg-info/PKG-INFO` & `notolog-0.9.0b11/notolog.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 Metadata-Version: 2.1
 Name: notolog
-Version: 0.9.0b10
+Version: 0.9.0b11
 Summary: Notolog Markdown Editor
 Home-page: https://github.com/notolog/notolog-editor
 Author: Vadim Bakhrenkov
 License: MIT
 Project-URL: Bug Reports, https://github.com/notolog/notolog-editor/issues
 Project-URL: Source, https://github.com/notolog/notolog-editor/
+Keywords: notolog,ai,markdown,editor
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Text Editors
+Classifier: Topic :: Text Editors :: Documentation
+Classifier: Topic :: Text Editors :: Emacs
+Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Topic :: Text Editors :: Word Processors
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
+Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi==1.16.0
 Requires-Dist: click==8.1.7
 Requires-Dist: cryptography==42.0.5
 Requires-Dist: emoji==2.11.1
@@ -27,34 +41,40 @@
 Requires-Dist: packaging==24.0
 Requires-Dist: pluggy==1.5.0
 Requires-Dist: pycparser==2.22
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: PySide6==6.7.0
 Requires-Dist: PySide6_Addons==6.7.0
 Requires-Dist: PySide6_Essentials==6.7.0
-Requires-Dist: pytest==8.1.2
+Requires-Dist: pytest==8.2.0
 Requires-Dist: pytest-mock==3.14.0
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: qasync==0.27.1
 Requires-Dist: qt6-applications==6.5.0.2.3
 Requires-Dist: qt6-tools==6.5.0.1.3
 Requires-Dist: shiboken6==6.7.0
 Requires-Dist: tomli==2.0.1
 
-<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-04-29 02:01:37.002734"}} -->
+<!-- {"notolog.app": {"created": "2023-12-25 18:59:43.806614", "updated": "2024-05-04 22:22:51.958596"}} -->
 # Notolog
 
+![Notolog](app/assets/notolog-example-image.png)&nbsp;&nbsp;&nbsp;![PyPI - Version](https://img.shields.io/pypi/v/notolog) ![PyPI - License](https://img.shields.io/pypi/l/notolog) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/notolog)
+
 ## Overview
 
 Notolog is a markdown editor crafted in Python and Qt, offered as an open-source solution.
 
 In short, I was in search of a simple, lightweight, and cross-platform editor to fulfill my daily needs as a software developer. Concurrently, I aimed to deepen my understanding of Python, leading me to embark on creating my own editor. Thus, the Notolog editor was born.
 
 The editor has no aim but the path, hence its proof-of-concept nature and many tasks yet to be completed. Speaking of tasks, the editor features special highlighting for the word 'TODO'; simply type it with '@', like '@todo something', and see what happens.
 
+---
+![Notolog settings UI example](docs/notolog-ui-settings.png)
+
+
 ## Features
 
 * Open sourced under the MIT license for full transparency and collaboration.
 * Markdown syntax highlighting:
 	* Editor mode offers smooth highlighting tailored specifically for Notolog, with line numbers and extended syntax highlighting.
 	* View mode utilizes the Python Markdown library for seamless rendering of Markdown syntax.
 	* Supports multi-line block open-close tokens for improved readability and structure.
@@ -83,94 +103,102 @@
 * In-line context menus:
 	* Right-click context menu options in the file tree for file rename and delete actions.
 	* Customizable toolbar with right-click functionality to show/hide icons based on user preferences.
 * Includes a suite of unit tests to ensure code reliability and maintainability, providing confidence in the editor's functionality.
 * AI Assistant UI to get all things you need in one place:
 	* At the moment the OpenAI API is supported with plans to extend support with other providers.
 
----
 There is no classical web engine integration to make overall package more lightweight and to achieve the best possible performance.
 
-## Prerequisites:
+
+## Prerequisites
 
 **Python 3.9 or higher installed on your system.**
 
 If you haven't already, download and install Python from the official website [python.org](python.org).
 
-Check the version of Python available with this command:
-```sh
-python3 -V
-```
+Check the version of Python available with this command `python3 -V`.
 
 **pip (Python package installer) should be available.**
+
 You can check if pip is installed by running `pip3 --version` in your terminal/command prompt.
 
+**Virtual Environment**
+
+It is highly recommended to use as it helps avoid version conflicts and interference from other packages. Below is a description of how to set up a virtual environment on your machine.
+
+
 ## Installation
 
-### Using pip installer (Recommended)
+### Method 1: pip installer (Recommended)
 
 ```sh
 pip install notolog
 ```
 
-### Run the Python code
+That's it! Starting the app is as simple as `notolog`.
+
+To update to the latest version, use:
+```sh
+pip install --upgrade notolog
+```
+
+### Method 2: Python source code
 
 0. Open Terminal.
 1. Clone project's GitHub repository to get a latest version.
 	* `git clone https://github.com/notolog/notolog-editor.git`
-2. Navigate to your project directory using the **cd** command.
-3. Make sure the virtual environment is activated as it's a common practice to isolate project code (described below).
+2. Navigate to the just cloned project's directory using the **cd** command.
+3. Make sure the virtual environment is activated as it's a common practice to isolate project code (activation described below).
 4. Simply run this command to set up project dependencies:
 
 ```sh
 pip3 install -r requirements.txt
 ```
 
 That's it! Starting the app is as simple as `python3 main.py`
 
-### Using Virtual Environments
+<details>
+<summary>Run tests</summary>
+
+To run all available tests:
+```sh
+pytest
+```
+
+To run a particular file's tests:
+```sh
+pytest tests/test_notolog_editor.py
+```
+</details>
+
+### Virtual Environments
 
-The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html)
+The instructions below contain steps of how to set up **venv** virtual environment to run a Python app safely. Starting from Python 3.6 **venv** is a recommended way to create virtual environments. For more information check [Creation of virtual environments](https://docs.python.org/3/library/venv.html). Alternatively, you can execute the Notolog code and set up virtual environment with your favorite Python code editor.
 
 #### MacOS and Linux
 
 ##### Set Up Virtual Environment
-
 1. Open Terminal.
 2. Navigate to your project directory using the cd command.
 3. Create a virtual environment by running `python3 -m venv notolog`. Replace **notolog** with the desired name for your virtual environment.
 
-Activate Virtual Environment:
+##### Activate Virtual Environment:
 To activate the virtual environment, run:
 ```sh
 source notolog/bin/activate
 ```
 
 To deactivate environment just run this command:
 ```sh
 deactivate
 ```
 
-#### Windows
-
-##### Set Up Virtual Environment
-
-1. Open Command Prompt or PowerShell.
-2. Navigate to your project directory using the `cd` command.
-3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
-
-##### Activate Virtual Environment
-
-To activate the virtual environment, run:
-```
-notolog\Scripts\activate
-```
-_Mind the environment name (**notolog** or any other selected before)._
-
-##### Install venv on Linux systems
+<details>
+<summary>Install venv on Linux systems</summary>
 
 While Python itself comes pre-installed on many Linux distributions, including Ubuntu, some distributions may not include the venv module by default. Therefore, you need to install it separately using the package manager before you can use it to create virtual environments.
 
 **Ubuntu/Debian**
 
 ```sh
 sudo apt-get update
@@ -184,37 +212,32 @@
 ```
 
 **CentOS/RHEL**
 
 ```sh
 sudo yum install python3-venv
 ```
+</details>
 
-### Using IDE
-
-Alternatively, you can execute the Notolog code with your favorite Python code editor.
+#### Windows
 
-## Usage
+##### Set Up Virtual Environment
 
-To start the app simply run this command in a project dir:
-```sh
-python3 main.py
-```
+1. Open Command Prompt or PowerShell.
+2. Navigate to your project directory using the `cd` command.
+3. Create a virtual environment by running `python -m venv notolog`. Replace **notolog** with the name you want to give to your virtual environment.
 
-### Run tests
+##### Activate Virtual Environment
 
-To run all available tests:
-```sh
-pytest
+To activate the virtual environment, run:
 ```
-
-To run a particular file's tests:
-```sh
-pytest tests/test_notolog_editor.py
+notolog\Scripts\activate
 ```
+_Mind the environment name (**notolog** or any other selected before)._
+
 
 ## Contributing
 
 If you encounter any issues or would like to contribute to the project, please don't hesitate to open an issue or submit a pull request on GitHub.
 
 ## License
 
@@ -277,10 +300,10 @@
 This application, primarily designed for educational purposes, employs PBKDF2HMAC for key derivation and AES-256 in CBC mode for encryption, using a 256-bit key. Note that the encryption salt and iteration counts are stored unencrypted in the file's header. While secure for educational and non-critical uses, this setup may not meet the highest security standards. Users can opt to add a password hint in the file header, which should be used judiciously to balance convenience against security risks.
 
 As an educational tool, this software is not intended for high-security needs. Users are encouraged to choose strong passwords to enhance data protection. Distributed under the MIT License, this open-source application requires users to ensure compliance with applicable laws. The developers disclaim liability for misuse or for ensuring legal compliance.
 
 ---
 
 `░░░░░░░░░░░░░░░░░░░░░░░▒▒▒▒▒▒▒▒▒▒▒▒▒▓▓▓▓▓▓▓███■███▓▓▓▓▓▓▓▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒░░░░░░░░░░░░░░░░░░░░░`
-`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`</br>
-`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
+`╔═══════════════════════════════════════════════════════════════════════════════════════════╗`
+`║ This README.md file has been carefully crafted and edited using the Notolog editor itself ║`
 `╚═══════════════════════════════════════════════════════════════════════════════════════════╝`
```

### Comparing `notolog-0.9.0b10/setup.py` & `notolog-0.9.0b11/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README file
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='notolog',
-    version='0.9.0b10',
+    version='0.9.0b11',
     description='Notolog Markdown Editor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/notolog/notolog-editor',
     author='Vadim Bakhrenkov',
     license='MIT',
     py_modules=['main'],
@@ -21,26 +21,36 @@
         ],
     },
     classifiers=[
         # More info https://pypi.org/classifiers/
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
+        'Operating System :: MacOS',
+        'Operating System :: Microsoft :: Windows',
+        'Operating System :: POSIX',
+        'Operating System :: Unix',
+        'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3 :: Only',
+        'Programming Language :: Python :: 3.12',
+        'Topic :: Text Editors',
+        'Topic :: Text Editors :: Documentation',
+        'Topic :: Text Editors :: Emacs',
+        'Topic :: Text Editors :: Integrated Development Environments (IDE)',
+        'Topic :: Text Editors :: Text Processing',
+        'Topic :: Text Editors :: Word Processors',
+        'Topic :: Text Processing',
+        'Topic :: Text Processing :: General',
+        'Topic :: Text Processing :: Markup :: Markdown',
     ],
     packages=find_packages(),  # Find all packages in the directory
     include_package_data=True,  # Include data files specified in MANIFEST.in
-    # package_data={
-    #    'notolog': ['docs/*.md'],
-    # },
-    # data_files=[('notolog-res', ['README.md'])],  # New dir with a content
     python_requires='>=3.9, <4',
     install_requires=[line.strip() for line in open("requirements.txt", "r")],
     project_urls={
         'Bug Reports': 'https://github.com/notolog/notolog-editor/issues',
         'Source': 'https://github.com/notolog/notolog-editor/',
     },
+    keywords='notolog, ai, markdown, editor',
 )
```

### Comparing `notolog-0.9.0b10/tests/test_enc_helper.py` & `notolog-0.9.0b11/tests/test_enc_helper.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_enc_password.py` & `notolog-0.9.0b11/tests/test_enc_password.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_file_header.py` & `notolog-0.9.0b11/tests/test_file_header.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_html_view.py` & `notolog-0.9.0b11/tests/test_html_view.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_lexemes.py` & `notolog-0.9.0b11/tests/test_lexemes.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_notolog_editor.py` & `notolog-0.9.0b11/tests/test_notolog_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,19 +57,21 @@
         mock_method2 = mocker.patch.object(test_obj_notolog_editor, 'load_file', return_value=True)
 
         # Call the method under test
         result = test_obj_notolog_editor.load_default_page()
         assert result is True
 
         # Current working directory
-        test_file_dir = os.getcwd()  # The .py file directory: os.path.dirname(os.path.realpath(__file__))
+        # test_run_from_dir = os.getcwd()
+        test_file_dir = os.path.dirname(os.path.realpath(__file__))
+        test_file_parent_dir = os.path.dirname(test_file_dir)
         # Assert that the method was called once
         mock_method1.assert_not_called()
         # Assert that the method was called once with the param(s)
-        mock_method2.assert_called_once_with('%s/README.md' % test_file_dir)
+        mock_method2.assert_called_once_with('%s/README.md' % test_file_parent_dir)
 
     def test_notolog_editor_load_default_page_any(self, mocker, test_obj_notolog_editor, test_obj_settings):
         """
         Check that an any page is loaded instead of default page
         @param mocker: pytest fixture
         @param test_obj_notolog_editor: NotologEditor instance
         @param test_obj_settings: Settings instance
@@ -113,23 +115,24 @@
     def test_notolog_editor_action_new_file(self, mocker, test_obj_notolog_editor, test_exp_params_fixture):
         mode, file_path, isfile, content, res_path_call_cnt = test_exp_params_fixture
 
         mocker.patch.object(test_obj_notolog_editor, 'get_mode', return_value=mode)
         mocker.patch.object(test_obj_notolog_editor, 'toggle_mode', return_value=None)
         setattr(test_obj_notolog_editor, 'debug', False)
 
-        mock_res_path = mocker.patch('notolog.notolog_editor.res_path', return_value=file_path)
+        mock_res_path = mocker.patch.object(test_obj_notolog_editor, 'get_active_dir', return_value=file_path)
+        #mock_res_path = mocker.patch('app.notolog_editor.res_path', return_value=file_path)
         # fixture arg: monkeypatch
-        # monkeypatch.setattr('notolog.notolog_editor.res_path', lambda _file_path: _file_path == file_path)
+        # monkeypatch.setattr('app.notolog_editor.res_path', lambda _file_path: _file_path == file_path)
         mocker.patch.object(os.path, 'isfile', return_value=isfile)
 
         mock_save_file_content = mocker.patch.object(test_obj_notolog_editor, 'save_file_content', return_value=None)
         mocker.patch.object(test_obj_notolog_editor, 'load_file', return_value=None)
 
         test_obj_notolog_editor.action_new_file(content)
 
         assert mock_res_path.call_count == res_path_call_cnt
         # Check the parameters passed to the mocked function(s)
-        assert str(mock_res_path.call_args) == "call('%s')" % file_path
+        # assert str(mock_res_path.call_args) == "call('%s')" % file_path
         # assert str(mock_save_file_content.call_args) == "call('%s', '%s')" % (file_path, content)
         if content:
             assert str(content) in str(mock_save_file_content.call_args)
```

### Comparing `notolog-0.9.0b10/tests/test_settings.py` & `notolog-0.9.0b11/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_text_block_data.py` & `notolog-0.9.0b11/tests/test_text_block_data.py`

 * *Files identical despite different names*

### Comparing `notolog-0.9.0b10/tests/test_theme_helper.py` & `notolog-0.9.0b11/tests/test_theme_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,34 +11,45 @@
 import os
 import pytest
 
 
 class TestThemeHelper:
 
     @pytest.fixture(scope="function", autouse=True)
-    def test_obj_theme_helper(self, mocker, request):
+    def test_settings_fixture(self):
+
+        settings = Settings()
+
+        yield settings
+
+    @pytest.fixture(scope="function", autouse=True)
+    def test_obj_theme_helper(self, test_settings_fixture, mocker, request):
         """
         Testing object fixture.
         May contain minimal logic for testing purposes.
         """
 
         # Get the parameter value(s) from the request
         theme = request.param if hasattr(request, 'param') else None
 
         mocker.patch.object(AppConfig, 'get_debug', return_value=False)
         # Or: monkeypatch.setattr(Settings, 'theme', theme)
-        mocker.patch('notolog.settings.Settings.app_theme', theme)
+        # mocker.patch('app.settings.Settings.app_theme', theme)
+        test_settings_fixture.app_theme = theme
 
         """
         If themes dir is set read themes from there.
         For test purposes to check theme files are readable.
         """
         test_themes_dir = os.path.join(os.path.dirname(__file__), 'test_themes')
         mocker.patch.object(Theme, 'get_themes_dir', return_value=test_themes_dir)
 
+        # Allow to change theme name during test cycle with no caching
+        AppConfig.set_test_mode(True)
+
         yield ThemeHelper()
 
     @pytest.fixture(scope="function")
     def test_exp_params_fixture(self, request):
         """
         Fixture to pass params and get expected results.
         This method is used only for passing params via pytest fixture.
@@ -77,16 +88,17 @@
         "test_obj_theme_helper, test_exp_params_fixture",
         [
             (None, (None, None, None)),
             ('default', ('test_red', None, 0xFF0000)),
             ('default', ('test_green', True, '#00FF00')),
             ('default', ('test_blue', False, 0x0000FF)),
             ('default', ('test_undefined', None, None)),
-            ('noir', ('test_non_red', False, 0x00FFFF)),
-            ('noir', ('test_light', True, '#FFFFFF')),
+            # 'noir_dark' is real as it can be checked with Themes enum
+            ('noir_dark', ('test_non_red', False, 0x00FFFF)),
+            ('noir_dark', ('test_light', True, '#FFFFFF')),
             ('test_undefined', (None, None, None)),
             ('test_undefined', ('undefined_name', True, None)),
         ],
         indirect=True
     )
     def test_themes_get_color(self, test_obj_theme_helper, test_exp_params_fixture):
         """
@@ -98,15 +110,15 @@
 
     @pytest.mark.parametrize(
         "test_obj_theme_helper, test_exp_params_fixture",
         [
             (None, (None, None)),
             ('default', ('test_smth', None)),
             ('default', ('test_styles', 'QTextEdit {}')),
-            ('noir', ('test_smth', 'QTextEdit {}')),
+            ('noir_dark', ('test_smth', 'QTextEdit {}')),
         ],
         indirect=True
     )
     def test_themes_get_css(self, test_obj_theme_helper, test_exp_params_fixture):
         """
         Test getter for correctly loaded and really existent theme's css files.
         """
```

### Comparing `notolog-0.9.0b10/tests/test_themes.py` & `notolog-0.9.0b11/tests/test_themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         assert test_obj_themes.theme == exp_theme
 
     @pytest.mark.parametrize(
         "test_obj_themes, test_exp_params_fixture",
         [
             (None, os.path.join(os.path.dirname(__file__), 'test_themes')),
             ('default', os.path.join(os.path.dirname(__file__), 'test_themes')),
-            ('noir', os.path.join(os.path.dirname(__file__), 'test_themes')),
+            ('noir_dark', os.path.join(os.path.dirname(__file__), 'test_themes')),
         ],
         indirect=True
     )
     def test_themes_get_themes_dir(self, test_obj_themes, test_exp_params_fixture):
         """
         Test theme dir path.
         """
@@ -117,16 +117,16 @@
     @pytest.mark.parametrize(
         "test_obj_themes, test_exp_params_fixture",
         [
             (None,
              ('default',
               {'default': {'test_red': '0xFF0000', 'test_green': '0x00FF00', 'test_blue': '0x0000FF',
                            'test_void': '0x000000'},
-               'noir': {'test_non_red': '0x00FFFF', 'test_non_green': '0xFF00FF', 'test_non_blue': '0xFFFF00',
-                        'test_light': '0xFFFFFF'}})),
+               'noir_dark': {'test_non_red': '0x00FFFF', 'test_non_green': '0xFF00FF', 'test_non_blue': '0xFFFF00',
+                             'test_light': '0xFFFFFF'}})),
         ],
         indirect=True
     )
     def test_themes_load_themes(self, test_obj_themes, test_exp_params_fixture):
         """
         Test actual theme colors loaded.
         """
@@ -140,16 +140,16 @@
         "test_obj_themes, test_exp_params_fixture",
         [
             (None,
              ('default', {'test_red': 0xFF0000, 'test_green': 0x00FF00, 'test_blue': 0x0000FF, 'test_void': 0x000000})),
             ('default',
              ('default',
               {'test_red': 0xFF0000, 'test_green': 0x00FF00, 'test_blue': 0x0000FF, 'test_void': 0x000000})),
-            ('noir',
-             ('noir',
+            ('noir_dark',
+             ('noir_dark',
               {'test_non_red': 0x00FFFF, 'test_non_green': 0xFF00FF, 'test_non_blue': 0xFFFF00,
                'test_light': 0xFFFFFF})),
         ],
         indirect=True
     )
     def test_themes_get_theme_colors(self, test_obj_themes, test_exp_params_fixture):
         """
@@ -162,15 +162,15 @@
         assert test_obj_themes.get_colors() == exp_colors
 
     @pytest.mark.parametrize(
         "test_obj_themes, test_exp_params_fixture",
         [
             (None, ('default', {'test_styles': 'default/test_styles.css'})),
             ('default', ('default', {'test_styles': 'default/test_styles.css'})),
-            ('noir', ('noir', {'test_smth': 'noir/test_smth.css'})),
+            ('noir_dark', ('noir_dark', {'test_smth': 'noir_dark/test_smth.css'})),
         ],
         indirect=True
     )
     def test_themes_get_theme_css(self, mocker, test_obj_themes, test_exp_params_fixture):
         """
         Test actual theme colors loaded.
         """
```

