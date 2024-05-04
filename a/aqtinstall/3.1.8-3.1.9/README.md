# Comparing `tmp/aqtinstall-3.1.8.tar.gz` & `tmp/aqtinstall-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtinstall-3.1.8.tar", last modified: Tue Oct 31 22:48:52 2023, max compression
+gzip compressed data, was "aqtinstall-3.1.9.tar", last modified: Mon Nov  6 02:57:17 2023, max compression
```

## Comparing `aqtinstall-3.1.8.tar` & `aqtinstall-3.1.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.486359 aqtinstall-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2023-10-31 22:48:52.486359 aqtinstall-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.466359 aqtinstall-3.1.8/aqt/
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25241 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/archives.py
--rw-r--r--   0 runner    (1001) docker     (127)    28454 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/combinations.json
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19294 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    57055 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/logging.ini
--rw-r--r--   0 runner    (1001) docker     (127)    43113 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    13217 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/aqt/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.470359 aqtinstall-3.1.8/aqtinstall.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-31 22:48:52.000000 aqtinstall-3.1.8/aqtinstall.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.470359 aqtinstall-3.1.8/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/accelbubble.7z
--rw-r--r--   0 runner    (1001) docker     (127)    17146 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/generate_azure_pipelines_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/generate_combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/helloworld.7z
--rw-r--r--   0 runner    (1001) docker     (127)  1213852 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/jom_1_1_3.zip
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/logging.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/openglwindow.7z
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/openglwindow_qt6.7z
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/redditclient.7z
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)    19125 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/ci/steps.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.474359 aqtinstall-3.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/CONTRIBUTE.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7672 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/SECURITY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    32379 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26591 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.466359 aqtinstall-3.1.8/docs/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.466359 aqtinstall-3.1.8/docs/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.474359 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/SECURITY.po
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/authors.po
--rw-r--r--   0 runner    (1001) docker     (127)    41059 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/changes.po
--rw-r--r--   0 runner    (1001) docker     (127)    39387 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/cli.po
--rw-r--r--   0 runner    (1001) docker     (127)    14457 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/configuration.po
--rw-r--r--   0 runner    (1001) docker     (127)    46696 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/getting_started.po
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/installation.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.474359 aqtinstall-3.1.8/docs/locale/pot/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/CODE_OF_CONDUCT.pot
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/CONTRIBUTE.pot
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/SECURITY.pot
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/authors.pot
--rw-r--r--   0 runner    (1001) docker     (127)    40934 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/changes.pot
--rw-r--r--   0 runner    (1001) docker     (127)    20318 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/cli.pot
--rw-r--r--   0 runner    (1001) docker     (127)     7649 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/configuration.pot
--rw-r--r--   0 runner    (1001) docker     (127)    22725 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/getting_started.pot
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/index.pot
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/locale/pot/installation.pot
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    25779 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/docs/previous_changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 22:48:52.486359 aqtinstall-3.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.478359 aqtinstall-3.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.482359 aqtinstall-3.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/linux-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/linux-android.html
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/linux-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    30922 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/linux-desktop.html
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    16521 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-android.html
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-sdktool-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-sdktool-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_cmake-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_cmake-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_ifw-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_ifw-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtcreator-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtcreator-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)    28812 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-desktop.html
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-ios-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mac-ios.html
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mirror-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    19653 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mirror-first-td.html
--rw-r--r--   0 runner    (1001) docker     (127)    17200 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mirror-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (127)    23047 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mirror-table-before-pre-a.html
--rw-r--r--   0 runner    (1001) docker     (127)    76947 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/mirror-tag-in-a.html
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/settings.ini
--rw-r--r--   0 runner    (1001) docker     (127)    12460 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/settings_no_concurrency.ini
--rw-r--r--   0 runner    (1001) docker     (127)    79658 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5140-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    72606 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5140-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5140-wasm-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    16692 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5140-wasm-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5150-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)   120616 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5150-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5152-src-doc-example-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    18932 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-5152-src-doc-example-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)    35906 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-620-android-armv7-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-620-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    84709 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-620-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-650-wasm-multi-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-650-wasm-multi-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-650-wasm-single-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-650-wasm-single-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-android-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-android.html
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)     6580 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop-tools-mingw-updates.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop-tools-qtcreator-updates.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6115 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop-tools_vcredist-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop-tools_vcredist-update.xml
--rw-r--r--   0 runner    (1001) docker     (127)    30880 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-desktop.html
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-winrt-expect.json
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/data/windows-winrt.html
--rw-r--r--   0 runner    (1001) docker     (127)    24466 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_archives.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_doc_archives.py
--rw-r--r--   0 runner    (1001) docker     (127)    15284 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    69708 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    50353 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tests/test_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 22:48:52.482359 aqtinstall-3.1.8/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tools/build_standalone.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-10-31 22:48:35.000000 aqtinstall-3.1.8/tools/launch_aqt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.188932 aqtinstall-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-11-06 02:57:17.188932 aqtinstall-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.164932 aqtinstall-3.1.9/aqt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25633 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28454 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/combinations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20255 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57105 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    43197 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13245 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    15146 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/aqt/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.164932 aqtinstall-3.1.9/aqtinstall.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11168 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-11-06 02:57:17.000000 aqtinstall-3.1.9/aqtinstall.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.168932 aqtinstall-3.1.9/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/accelbubble.7z
+-rw-r--r--   0 runner    (1001) docker     (127)    17146 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/generate_azure_pipelines_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7223 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/generate_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/helloworld.7z
+-rw-r--r--   0 runner    (1001) docker     (127)  1213852 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/jom_1_1_3.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/openglwindow.7z
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/openglwindow_qt6.7z
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/redditclient.7z
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    19125 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/ci/steps.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.172932 aqtinstall-3.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/CONTRIBUTE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/SECURITY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    32379 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26631 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.164932 aqtinstall-3.1.9/docs/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.160931 aqtinstall-3.1.9/docs/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.172932 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/SECURITY.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/authors.po
+-rw-r--r--   0 runner    (1001) docker     (127)    41059 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/changes.po
+-rw-r--r--   0 runner    (1001) docker     (127)    39387 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/cli.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/configuration.po
+-rw-r--r--   0 runner    (1001) docker     (127)    46696 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/getting_started.po
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/installation.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.172932 aqtinstall-3.1.9/docs/locale/pot/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/CODE_OF_CONDUCT.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/CONTRIBUTE.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/SECURITY.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/authors.pot
+-rw-r--r--   0 runner    (1001) docker     (127)    40934 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/changes.pot
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/cli.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     7649 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/configuration.pot
+-rw-r--r--   0 runner    (1001) docker     (127)    22725 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/getting_started.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/index.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/locale/pot/installation.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    25780 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/docs/previous_changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 02:57:17.188932 aqtinstall-3.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.176932 aqtinstall-3.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.184932 aqtinstall-3.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/linux-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18093 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/linux-android.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/linux-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30922 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/linux-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16521 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-android.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-sdktool-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-sdktool-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_cmake-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_cmake-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_ifw-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_ifw-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtcreator-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtcreator-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtdesignstudio-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtdesignstudio-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    28812 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-ios-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mac-ios.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mirror-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19653 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mirror-first-td.html
+-rw-r--r--   0 runner    (1001) docker     (127)    17200 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mirror-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23047 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mirror-table-before-pre-a.html
+-rw-r--r--   0 runner    (1001) docker     (127)    76947 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/mirror-tag-in-a.html
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    12460 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/settings_no_concurrency.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    79658 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5140-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72606 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5140-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5140-wasm-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16692 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5140-wasm-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5150-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)   120616 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5150-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5152-src-doc-example-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18932 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-5152-src-doc-example-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    35906 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-620-android-armv7-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-620-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84709 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-620-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-650-wasm-multi-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-650-wasm-multi-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-650-wasm-single-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-650-wasm-single-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-android-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-android.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop-tools-mingw-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop-tools-qtcreator-updates.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6115 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop-tools_vcredist-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop-tools_vcredist-update.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    30880 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-desktop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-winrt-expect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/data/windows-winrt.html
+-rw-r--r--   0 runner    (1001) docker     (127)    24466 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_doc_archives.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69708 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50353 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tests/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 02:57:17.184932 aqtinstall-3.1.9/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tools/build_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-06 02:57:05.000000 aqtinstall-3.1.9/tools/launch_aqt.py
```

### Comparing `aqtinstall-3.1.8/LICENSE` & `aqtinstall-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/MANIFEST.in` & `aqtinstall-3.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/PKG-INFO` & `aqtinstall-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.8
+Version: 3.1.9
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
@@ -26,43 +26,44 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: defusedxml
 Requires-Dist: humanize
 Requires-Dist: patch>=1.16
 Requires-Dist: py7zr>=0.20.6
-Requires-Dist: requests>2.20.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: semantic-version
 Requires-Dist: texttable
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-pep8; extra == "test"
-Requires-Dist: pytest-remotedata<0.4.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-remotedata>=0.4.1; extra == "test"
 Requires-Dist: pytest-socket; extra == "test"
-Requires-Dist: pytest-leaks; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: pympler; extra == "test"
 Provides-Extra: check
 Requires-Dist: mypy>=0.990; extra == "check"
-Requires-Dist: flake8<6; extra == "check"
+Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "check"
 Requires-Dist: flake8-black; extra == "check"
 Requires-Dist: flake8-colors; extra == "check"
-Requires-Dist: flake8-isort<6.0.0,>=5.0.3; extra == "check"
+Requires-Dist: flake8-isort<7.0.0,>=6.0.0; extra == "check"
 Requires-Dist: flake8-pyi; extra == "check"
 Requires-Dist: flake8-typing-imports; extra == "check"
 Requires-Dist: docutils; extra == "check"
 Requires-Dist: check-manifest; extra == "check"
 Requires-Dist: readme-renderer; extra == "check"
 Requires-Dist: pygments; extra == "check"
 Requires-Dist: packaging; extra == "check"
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.3; extra == "docs"
 Requires-Dist: sphinx-py3doc-enhanced-theme>=2.4; extra == "docs"
+Provides-Extra: debug
+Requires-Dist: pytest-leaks; extra == "debug"
 
 Another Qt installer(aqt)
 =========================
 
 - Release: |pypi|
 - Documentation: |docs|
 - Test status: |gha| and Coverage: |coveralls|
```

### Comparing `aqtinstall-3.1.8/README.rst` & `aqtinstall-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/__init__.py` & `aqtinstall-3.1.9/aqt/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/__main__.py` & `aqtinstall-3.1.9/aqt/__main__.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/archives.py` & `aqtinstall-3.1.9/aqt/archives.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from dataclasses import dataclass, field
 from logging import getLogger
 from typing import Dict, Iterable, List, Optional, Set, Tuple
 from xml.etree.ElementTree import Element  # noqa
 
 from defusedxml import ElementTree
 
-from aqt.exceptions import ArchiveDownloadError, ArchiveListError, NoPackageFound
+from aqt.exceptions import ArchiveDownloadError, ArchiveListError, ChecksumDownloadFailure, NoPackageFound
 from aqt.helper import Settings, get_hash, getUrl, ssplit
 from aqt.metadata import QtRepoProperty, Version
 
 
 @dataclass
 class TargetConfig:
     version: str
@@ -386,15 +386,24 @@
         )
         update_xml_url = posixpath.join(os_target_folder, "Updates.xml")
         update_xml_text = self._download_update_xml(update_xml_url)
         self._parse_update_xml(os_target_folder, update_xml_text, target_packages)
 
     def _download_update_xml(self, update_xml_path):
         """Hook for unit test."""
-        xml_hash = get_hash(update_xml_path, "sha256", self.timeout)
+        if not Settings.ignore_hash:
+            try:
+                xml_hash = get_hash(update_xml_path, Settings.hash_algorithm, self.timeout)
+            except ChecksumDownloadFailure:
+                self.logger.warning(
+                    "Failed to download checksum for the file 'Updates.xml'. This may happen on unofficial mirrors."
+                )
+                xml_hash = None
+        else:
+            xml_hash = None
         return getUrl(posixpath.join(self.base, update_xml_path), self.timeout, xml_hash)
 
     def _parse_update_xml(self, os_target_folder, update_xml_text, target_packages: Optional[ModuleToPackage]):
         if not target_packages:
             target_packages = ModuleToPackage({})
         update_xml = Updates.fromstring(self.base, update_xml_text)
         base_url = self.base
```

### Comparing `aqtinstall-3.1.8/aqt/combinations.json` & `aqtinstall-3.1.9/aqt/combinations.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/exceptions.py` & `aqtinstall-3.1.9/aqt/exceptions.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/helper.py` & `aqtinstall-3.1.9/aqt/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,25 +90,33 @@
             raise ArchiveConnectionError(f"Failure to connect to {url}: {type(e).__name__}") from e
         else:
             if r.status_code != 200:
                 msg = f"Failed to retrieve file at {url}\nServer response code: {r.status_code}, reason: {r.reason}"
                 raise ArchiveDownloadError(msg)
         result: str = r.text
         filename = url.split("/")[-1]
-        actual_hash = hashlib.sha256(bytes(result, "utf-8")).digest()
+        _kwargs = {"usedforsecurity": False} if sys.version_info >= (3, 9) else {}
+        if Settings.hash_algorithm == "sha256":
+            actual_hash = hashlib.sha256(bytes(result, "utf-8"), **_kwargs).digest()
+        elif Settings.hash_algorithm == "sha1":
+            actual_hash = hashlib.sha1(bytes(result, "utf-8"), **_kwargs).digest()
+        elif Settings.hash_algorithm == "md5":
+            actual_hash = hashlib.md5(bytes(result, "utf-8"), **_kwargs).digest()
+        else:
+            raise ArchiveChecksumError(f"Unknown hash algorithm: {Settings.hash_algorithm}.\nPlease check settings.ini")
         if expected_hash is not None and expected_hash != actual_hash:
             raise ArchiveChecksumError(
                 f"Downloaded file {filename} is corrupted! Detect checksum error.\n"
                 f"Expect {expected_hash.hex()}: {url}\n"
                 f"Actual {actual_hash.hex()}: {filename}"
             )
     return result
 
 
-def downloadBinaryFile(url: str, out: Path, hash_algo: str, exp: bytes, timeout: Tuple[float, float]) -> None:
+def downloadBinaryFile(url: str, out: Path, hash_algo: str, exp: Optional[bytes], timeout: Tuple[float, float]) -> None:
     logger = getLogger("aqt.helper")
     filename = Path(url).name
     with requests.sessions.Session() as session:
         retries = requests.adapters.Retry(
             total=Settings.max_retries_on_connection_error, backoff_factor=Settings.backoff_factor
         )
         adapter = requests.adapters.HTTPAdapter(max_retries=retries)
@@ -122,15 +130,18 @@
                 logger.info("Redirected: {}".format(urlparse(newurl).hostname))
                 r = session.get(newurl, stream=True, timeout=timeout)
         except requests.exceptions.ConnectionError as e:
             raise ArchiveConnectionError(f"Connection error: {e.args}") from e
         except requests.exceptions.Timeout as e:
             raise ArchiveConnectionError(f"Connection timeout: {e.args}") from e
         else:
-            hash = hashlib.new(hash_algo)
+            if sys.version_info >= (3, 9):
+                hash = hashlib.new(hash_algo, usedforsecurity=False)
+            else:
+                hash = hashlib.new(hash_algo)
             try:
                 with open(out, "wb") as fd:
                     for chunk in r.iter_content(chunk_size=8196):
                         fd.write(chunk)
                         hash.update(chunk)
                     fd.flush()
             except Exception as e:
@@ -453,14 +464,22 @@
         return self.config.getint("requests", "max_retries_on_checksum_error", fallback=int(self.max_retries))
 
     @property
     def max_retries_to_retrieve_hash(self):
         return self.config.getint("requests", "max_retries_to_retrieve_hash", fallback=int(self.max_retries))
 
     @property
+    def hash_algorithm(self):
+        return self.config.get("requests", "hash_algorithm", fallback="sha256")
+
+    @property
+    def ignore_hash(self):
+        return self.config.getboolean("requests", "INSECURE_NOT_FOR_PRODUCTION_ignore_hash", fallback=False)
+
+    @property
     def backoff_factor(self):
         return self.config.getfloat("requests", "retry_backoff", fallback=0.1)
 
     @property
     def trusted_mirrors(self):
         return self.config.getlist("mirrors", "trusted_mirrors", fallback=[self.baseurl])
```

### Comparing `aqtinstall-3.1.8/aqt/installer.py` & `aqtinstall-3.1.9/aqt/installer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1213,20 +1213,20 @@
     logger = getLogger()
     for handler in logger.handlers:
         handler.close()
         logger.removeHandler(handler)
     logger.addHandler(qh)
     #
     timeout = (Settings.connection_timeout, Settings.response_timeout)
-    hash = get_hash(qt_package.archive_path, algorithm="sha256", timeout=timeout)
+    hash = get_hash(qt_package.archive_path, Settings.hash_algorithm, timeout) if not Settings.ignore_hash else None
 
     def download_bin(_base_url):
         url = posixpath.join(_base_url, qt_package.archive_path)
         logger.debug("Download URL: {}".format(url))
-        return downloadBinaryFile(url, archive, "sha256", hash, timeout)
+        return downloadBinaryFile(url, archive, Settings.hash_algorithm, hash, timeout)
 
     retry_on_errors(
         action=lambda: retry_on_bad_connection(download_bin, base_url),
         acceptable_errors=(ArchiveChecksumError,),
         num_retries=Settings.max_retries_on_checksum_error,
         name=f"Downloading {name}",
     )
```

### Comparing `aqtinstall-3.1.8/aqt/logging.ini` & `aqtinstall-3.1.9/aqt/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqt/metadata.py` & `aqtinstall-3.1.9/aqt/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,15 +703,15 @@
             version = Version(qt_ver)
         except ValueError as e:
             raise CliInputError(e) from e
         return version
 
     def fetch_http(self, rest_of_url: str, is_check_hash: bool = True) -> str:
         timeout = (Settings.connection_timeout, Settings.response_timeout)
-        expected_hash = get_hash(rest_of_url, "sha256", timeout) if is_check_hash else None
+        expected_hash = get_hash(rest_of_url, Settings.hash_algorithm, timeout) if is_check_hash else None
         base_urls = self.base_url, random.choice(Settings.fallbacks)
 
         err: BaseException = AssertionError("unraisable")
 
         for i, base_url in enumerate(base_urls):
             try:
                 url = posixpath.join(base_url, rest_of_url)
@@ -788,15 +788,15 @@
             if version.prerelease or self.archive_id.is_preview() or version in SimpleSpec("5.9.0")
             else str(version.patch)
         )
         return f"{version.major}{version.minor}{patch}"
 
     def _fetch_module_metadata(self, folder: str, predicate: Optional[Callable[[Element], bool]] = None):
         rest_of_url = posixpath.join(self.archive_id.to_url(), folder, "Updates.xml")
-        xml = self.fetch_http(rest_of_url)
+        xml = self.fetch_http(rest_of_url) if not Settings.ignore_hash else self.fetch_http(rest_of_url, False)
         return xml_to_modules(
             xml,
             predicate=predicate if predicate else MetadataFactory._has_nonempty_downloads,
         )
 
     def fetch_modules(self, version: Version, arch: str) -> List[str]:
         """Returns list of modules"""
```

### Comparing `aqtinstall-3.1.8/aqt/settings.ini` & `aqtinstall-3.1.9/aqt/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 [requests]
 connection_timeout: 3.5
 response_timeout: 30
 max_retries_on_connection_error: 5
 retry_backoff: 0.1
 max_retries_on_checksum_error: 5
 max_retries_to_retrieve_hash: 5
+hash_algorithm: sha256
+INSECURE_NOT_FOR_PRODUCTION_ignore_hash: False
 
 [mirrors]
 trusted_mirrors:
     https://download.qt.io
 blacklist:
     http://mirrors.ocf.berkeley.edu
     http://mirrors.tuna.tsinghua.edu.cn
     http://mirrors.geekpie.club
 fallbacks:
     https://qtproject.mirror.liquidtelecom.com/
     https://mirrors.aliyun.com/qt/
-    https://mirrors.sjtug.sjtu.edu.cn/qt/
     https://mirrors.ustc.edu.cn/qtproject/
     https://ftp.jaist.ac.jp/pub/qtproject/
     https://ftp.yz.yamagata-u.ac.jp/pub/qtproject/
     https://qt-mirror.dannhauer.de/
     https://ftp.fau.de/qtproject/
     https://mirror.netcologne.de/qtproject/
     https://mirrors.dotsrc.org/qtproject/
```

### Comparing `aqtinstall-3.1.8/aqt/updater.py` & `aqtinstall-3.1.9/aqt/updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/aqtinstall.egg-info/PKG-INFO` & `aqtinstall-3.1.9/aqtinstall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtinstall
-Version: 3.1.8
+Version: 3.1.9
 Summary: Another unofficial Qt installer
 Author-email: Hiroshi Miura <miurahr@linux.com>
 License: MIT License
 Project-URL: Documentation, https://aqtinstall.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/miurahr/aqtinstall/issues
 Project-URL: Wiki, https://github.com/miurahr/aqtinstall/wiki
 Project-URL: Source, https://github.com/miurahr/aqtinstall
@@ -26,43 +26,44 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: bs4
 Requires-Dist: defusedxml
 Requires-Dist: humanize
 Requires-Dist: patch>=1.16
 Requires-Dist: py7zr>=0.20.6
-Requires-Dist: requests>2.20.0
+Requires-Dist: requests>=2.31.0
 Requires-Dist: semantic-version
 Requires-Dist: texttable
 Provides-Extra: test
 Requires-Dist: pytest>=6.0; extra == "test"
 Requires-Dist: pytest-pep8; extra == "test"
-Requires-Dist: pytest-remotedata<0.4.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: pytest-remotedata>=0.4.1; extra == "test"
 Requires-Dist: pytest-socket; extra == "test"
-Requires-Dist: pytest-leaks; extra == "test"
 Requires-Dist: pytest-timeout; extra == "test"
 Requires-Dist: pympler; extra == "test"
 Provides-Extra: check
 Requires-Dist: mypy>=0.990; extra == "check"
-Requires-Dist: flake8<6; extra == "check"
+Requires-Dist: flake8<7.0.0,>=6.0.0; extra == "check"
 Requires-Dist: flake8-black; extra == "check"
 Requires-Dist: flake8-colors; extra == "check"
-Requires-Dist: flake8-isort<6.0.0,>=5.0.3; extra == "check"
+Requires-Dist: flake8-isort<7.0.0,>=6.0.0; extra == "check"
 Requires-Dist: flake8-pyi; extra == "check"
 Requires-Dist: flake8-typing-imports; extra == "check"
 Requires-Dist: docutils; extra == "check"
 Requires-Dist: check-manifest; extra == "check"
 Requires-Dist: readme-renderer; extra == "check"
 Requires-Dist: pygments; extra == "check"
 Requires-Dist: packaging; extra == "check"
 Provides-Extra: docs
 Requires-Dist: sphinx>=7.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.3; extra == "docs"
 Requires-Dist: sphinx-py3doc-enhanced-theme>=2.4; extra == "docs"
+Provides-Extra: debug
+Requires-Dist: pytest-leaks; extra == "debug"
 
 Another Qt installer(aqt)
 =========================
 
 - Release: |pypi|
 - Documentation: |docs|
 - Test status: |gha| and Coverage: |coveralls|
```

### Comparing `aqtinstall-3.1.8/aqtinstall.egg-info/SOURCES.txt` & `aqtinstall-3.1.9/aqtinstall.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/accelbubble.7z` & `aqtinstall-3.1.9/ci/accelbubble.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/generate_azure_pipelines_matrices.py` & `aqtinstall-3.1.9/ci/generate_azure_pipelines_matrices.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/generate_combinations.py` & `aqtinstall-3.1.9/ci/generate_combinations.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/jom_1_1_3.zip` & `aqtinstall-3.1.9/ci/jom_1_1_3.zip`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/logging.ini` & `aqtinstall-3.1.9/ci/logging.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/openglwindow.7z` & `aqtinstall-3.1.9/ci/openglwindow.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/openglwindow_qt6.7z` & `aqtinstall-3.1.9/ci/openglwindow_qt6.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/redditclient.7z` & `aqtinstall-3.1.9/ci/redditclient.7z`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/settings.ini` & `aqtinstall-3.1.9/ci/settings.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/ci/steps.yml` & `aqtinstall-3.1.9/ci/steps.yml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/CHANGELOG.rst` & `aqtinstall-3.1.9/docs/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,34 @@
 ==========
 
 All notable changes to this project will be documented in this file.
 
 `Unreleased`_
 =============
 
+`v3.1.9`_ (6, Nov. 2023)
+========================
+
+Security
+--------
+* CVE-2023-32681: Bump requests@2.31.0 (#724)
+
+Changed
+-------
+* Remove a specific mirror from fallback (#688)
+* add ``debug`` extras for test and check (#725)
+* Bump pytest-remotedata@0.4.1
+* Bump flake8,flake8-isort@6.0.0 (#726)
+* docs: change interpreted text to inline literals (#728)
+
+Added
+-----
+* macOS binary build (#722)
+* ``ignore_hash`` and ``hash_algorithm`` options (#684)
+
 `v3.1.8`_ (1, Nov. 2023)
 ========================
 
 Changed
 -------
 - Add 6.5.3 and openssl as known versions (#718)
 - Docs: remove deprecated configuration description (#714)
@@ -263,15 +283,16 @@
 --------
 * Use secrets for secure random numbers(#498)
 * Use defusedxml to parse Updates.xml file to avoid attack(#498)
 * Improve get_hash function(#504)
 * Check Update.xml file with SHA256 hash (#493)
 
 
-.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.8...HEAD
+.. _Unreleased: https://github.com/miurahr/aqtinstall/compare/v3.1.9...HEAD
+.. _v3.1.9: https://github.com/miurahr/aqtinstall/compare/v3.1.8...v3.1.9
 .. _v3.1.8: https://github.com/miurahr/aqtinstall/compare/v3.1.7...v3.1.8
 .. _v3.1.7: https://github.com/miurahr/aqtinstall/compare/v3.1.6...v3.1.7
 .. _v3.1.6: https://github.com/miurahr/aqtinstall/compare/v3.1.5...v3.1.6
 .. _v3.1.5: https://github.com/miurahr/aqtinstall/compare/v3.1.4...v3.1.5
 .. _v3.1.4: https://github.com/miurahr/aqtinstall/compare/v3.1.3...v3.1.4
 .. _v3.1.3: https://github.com/miurahr/aqtinstall/compare/v3.1.2...v3.1.3
 .. _v3.1.2: https://github.com/miurahr/aqtinstall/compare/v3.1.1...v3.1.2
```

### Comparing `aqtinstall-3.1.8/docs/CODE_OF_CONDUCT.rst` & `aqtinstall-3.1.9/docs/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/CONTRIBUTE.rst` & `aqtinstall-3.1.9/docs/CONTRIBUTE.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/Makefile` & `aqtinstall-3.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/authors.rst` & `aqtinstall-3.1.9/docs/authors.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 Original qli-installer is written by Linus Jahn
 
 Significant contributions for improvements of version 2.0 and 2.1 by David Dalcino
 David also leads many developments and reviews effort after 2.0.
 
 All contributors, listed alphabetically, are:
 
+* Alberto Mardegan(ignore_hash option)
 * Andrei Yankovich (tools ifw installation)
 * Aurélien Gâteau (patching to qmake)
 * Benjamin O (Github Actions and more)
 * Christian Hoffmann (Update mirror list)
 * David Dalcino (Many improvements on CI automations, commands, tests, documents and so on)
 * Doronin Stanislav (document)
 * Fabrice Le Bars (32bit binary)
 * Felix Barz (Android, Explicit extra module installation)
 * Gamso (improve parsing of update.xml)
 * Julien Marrec (mypy, type hints)
 * Kyle Altendorf (7z binary path search)
-* lightmare (Documents)
-* Mike Tzou (Update fallback url)
+* @lebarsfa (ignore_hash/hash_algorithm options)
+* @lightmare (Documents)
 * Martin Delille (Documents)
+* Mike Tzou (Update fallback url)
 * mite-user (folder index handling of download web sites)
 * Mizux Seihax (Qt versions)
 * Mozi (CI/workflow improvement, log format)
 * Nelson Chen (CI tests)
 * @nikitalita (Binary distribution)
 * @pylipp (Documents)
+* @Steveice10 (MacOS binary build)
 * Sztergbaum Roman (Version database)
 * Thomas Grainger (CLI entry point)
 * @tsteven4 (fix patching to qmake, pkgconfig and libtool)
 * Vadim Peretokin (Version database)
 * Vladyslav Hnatiuk (Version database)
 * @ypnos (Documents)
```

### Comparing `aqtinstall-3.1.8/docs/cli.rst` & `aqtinstall-3.1.9/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/conf.py` & `aqtinstall-3.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/configuration.rst` & `aqtinstall-3.1.9/docs/configuration.rst`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     [requests]
     connection_timeout: 3.5
     response_timeout: 30
     max_retries_on_connection_error: 5
     retry_backoff: 0.1
     max_retries_on_checksum_error: 5
     max_retries_to_retrieve_hash: 5
+    hash_algorithm: sha256
+    INSECURE_NOT_FOR_PRODUCTION_ignore_hash: False
 
     [mirrors]
     trusted_mirrors:
         https://download.qt.io
     blacklist:
         http://mirrors.ustc.edu.cn
         http://mirrors.tuna.tsinghua.edu.cn
@@ -93,15 +95,15 @@
     This is the minimum decompressed size, in bytes, of the modules that aqt is permitted to list.
     The authors of aqt have discovered that the Qt repository contains a few mysteriously
     "empty" modules, including the examples modules for `qtlottie` and `qtquicktimeline`.
     These modules consist of a single archive that contains empty directories,
     and they are exactly 40 bytes when uncompressed.
     The authors feel that it is not useful for ``aqt list-*`` to list these empty modules.
     If you want to print these modules with ``aqt list-*``, please feel free to change
-    the `min_module_size` value to something less than 40.
+    the ``min_module_size`` value to something less than 40.
 
     This setting has no effect on your ability to install these modules.
     ``aqt install-*`` can will still install them without any warnings.
 
 
 The ``[requests]`` section controls the way that ``aqt`` makes network requests.
 
@@ -126,14 +128,26 @@
     Setting this value too low will hammer the server, and may result
     in no successful connections at all.
 
 max_retries_on_checksum_error:
     This setting controls how many times ``aqt`` will attempt to download a file,
     in the case of a checksum error.
 
+hash_algorithm:
+    This is either ``sha256``, ``sha1`` or ``md5``. ``sha256`` is the only safe 
+    value to use here. Default is ``sha256`` if not set.
+    See also ``trusted_mirrors`` setting.
+
+INSECURE_NOT_FOR_PRODUCTION_ignore_hash:
+    This is either ``True`` or ``False``.
+    The ``True`` setting disables hash checking when downloading files. Although
+    this is not recommended, this may help when hashes are not available.
+    The ``False`` setting will enforce hash checking. This is highly recommended
+    to avoid corrupted files.
+
 
 The ``[mirrors]`` section is a configuration for mirror handling.
 
 trusted_mirrors:
     ``trusted_mirrors`` is a list of URLs that you trust to provide accurate
     checksums for all downloaded archives.
     This is a security feature; please do not change this value unless you know
```

### Comparing `aqtinstall-3.1.8/docs/getting_started.rst` & `aqtinstall-3.1.9/docs/getting_started.rst`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 Notice that this is a very small subset of the architectures listed in the 
 `Available Qt versions`_ wiki page. If we need to use some architecture that
 is not on this list, we can use the `Available Qt versions`_ wiki page to get
 a rough idea of what versions support the architecture we want, and then use
 :ref:`aqt list-qt <list-qt command>` to confirm that the architecture is available.
 
-Let's say that we want to install Qt 6.2.0 with architecture `win64_mingw81`.
+Let's say that we want to install Qt 6.2.0 with architecture ``win64_mingw81``.
 The installation command we need is:
 
 .. code-block:: console
 
     $ aqt install-qt windows desktop 6.2.0 win64_mingw81
 
 Let's say that we want to install the next version of Qt 6.2 as soon as it is available.
@@ -116,23 +116,23 @@
 installed by default, using this command:
 
 .. code-block:: console
 
     $ aqt install-qt linux desktop 6.2.0 gcc_64 --external 7z
 
 .. _py7zr: https://pypi.org/project/py7zr/
-.. _p7zip: http://p7zip.sourceforge.net/
+.. _p7zip: https://p7zip.sourceforge.net/
 .. _7-zip: https://www.7-zip.org/
 
 Changing the output directory
 -----------------------------
 
 By default, ``aqt`` will install all of the Qt packages into the current
 working directory, in the subdirectory ``./<Qt version>/<arch>/``.
-For example, if we install Qt 6.2.0 for Windows desktop with arch `win64_mingw81`,
+For example, if we install Qt 6.2.0 for Windows desktop with arch ``win64_mingw81``,
 it would end up in ``./6.2.0/win64_mingw81``.
 
 If you would prefer to install it to another location, you
 will need to use the ``-O`` or ``--outputdir`` flag.
 This option also works for all of the other subcommands that begin with
 ``aqt install-``.
 
@@ -180,15 +180,15 @@
     qtquicktimeline     Qt Quick Timeline for MinGW 8.1.0 64-bit
     qtscript            Qt Script for MinGW 8.1.0 64-bit
     qtvirtualkeyboard   Qt Virtual Keyboard for MinGW 8.1.0 64-bit
     qtwebglplugin       Qt WebGL Streaming Plugin for MinGW 8.1.0 64-bit
 
 Note that if your terminal is wider than 95 characters, this command will show
 release dates and sizes in extra columns to the right.
-If you try this, you will notice that `debug_info` is 5.9 gigabytes installed.
+If you try this, you will notice that ``debug_info`` is 5.9 gigabytes installed.
 
 Also, notice that the 'Display Name' indicates which compiler the module is
 intended to be used with. In this case, for the architecture ``win64_mingw81``,
 you will most likely want to use the "MinGW 8.1.0 64-bit" compiler.
 Here's what the command prints when you use it with the ambiguously-named
 ``win64_mingw`` architecture:
 
@@ -202,16 +202,16 @@
     qt5compat           Qt 5 Compatibility Module for MinGW 11.2.0 64-bit
     qtactiveqt          Qt 3D for MinGW 11.2.0 64-bit
     qtcharts            Qt Charts for MinGW 11.2.0 64-bit
     ...
 
 You can find out how to install MinGW 8.1.0 and 11.2.0 in the `Installing Tools`_ section.
 
-Let's say that we want to install `qtcharts` and `qtnetworkauth`. 
-We can do that by using the `-m` flag with the :ref:`aqt install-qt <qt installation command>` command.
+Let's say that we want to install ``qtcharts`` and ``qtnetworkauth``.
+We can do that by using the ``-m`` flag with the :ref:`aqt install-qt <qt installation command>` command.
 This flag receives the name of at least one module as an argument:
 
 .. code-block:: console
 
     $ aqt install-qt windows desktop 5.15.2 win64_mingw81 -m qtcharts qtnetworkauth
 
 If we wish to install all the modules that are available, we can do that with the ``all`` keyword:
@@ -231,16 +231,16 @@
 
 You will need a Unix-style shell to run this command, or at least git-bash on Windows.
 The ``xargs`` equivalent to this command is an exercise left to the reader.
 
 If you want to install all available modules, you are probably better off using
 the ``all`` keyword, as discussed above. This scripting example is presented to
 give you a sense of how to accomplish something more complicated.
-Perhaps you want to install all modules except `qtnetworkauth`; you could write a script
-that removes `qtnetworkauth` from the output of :ref:`aqt list-qt <list-qt command>`,
+Perhaps you want to install all modules except ``qtnetworkauth``; you could write a script
+that removes ``qtnetworkauth`` from the output of :ref:`aqt list-qt <list-qt command>`,
 and pipe that into :ref:`aqt install-qt <qt installation command>`.
 This exercise is left to the reader.
 
 
 Installing Qt for Android
 -------------------------
 
@@ -336,15 +336,15 @@
     tools_ninja
     tools_mingw
     tools_mingw90
     tools_ifw
     tools_conan
     tools_cmake
 
-Let's see what tool variants are available in `tools_mingw`:
+Let's see what tool variants are available in ``tools_mingw``:
 
 .. code-block:: console
 
     $ aqt list-tool windows desktop tools_mingw
     qt.tools.mingw47
     qt.tools.win32_mingw48
     qt.tools.win32_mingw482
@@ -374,15 +374,15 @@
     qt.tools.win32_mingw530   5.3.0-2                2017-04-27
     qt.tools.win32_mingw730   7.3.0-1-202004170606   2020-04-17
     qt.tools.win32_mingw810   8.1.0-1-202004170606   2020-04-17
     qt.tools.win64_mingw730   7.3.0-1-202004170606   2020-04-17
     qt.tools.win64_mingw810   8.1.0-1-202004170606   2020-04-17
 
 The ``-l`` flag causes :ref:`aqt list-tool <list-tool command>` to print a table
-that shows plenty of data pertinent to each tool variant available in `tools_mingw`.
+that shows plenty of data pertinent to each tool variant available in ``tools_mingw``.
 :ref:`aqt list-tool <list-tool command>` additionally prints the 'Display Name'
 and 'Description' for each tool if your terminal is wider than 95 characters;
 terminals that are narrower than this cannot display this table in a readable way.
 
 Please be aware that the tool ``tools_mingw90`` appears to be mislabelled:
 
 .. code-block:: console
@@ -403,34 +403,34 @@
 
 The 'narrow display' for ``tools_mingw90`` cuts off the two columns of the table that
 show you what's really in that package: ``MinGW 11.2.0 64-bit``.
 If you are using the ``win64_mingw`` architecture for Qt 6.2.2+, then this is
 probably the compiler you want to install (see `long_modules explanation`_).
 
 
-Now let's install `mingw`, using the :ref:`aqt install-tool <tools installation command>` command.
+Now let's install ``mingw``, using the :ref:`aqt install-tool <tools installation command>` command.
 This command receives four parameters:
 
 1. The host operating system (windows, mac, or linux)
 2. The target SDK (desktop, android, ios, or winrt)
-3. The name of the tool (this is `tools_mingw` in our case)
+3. The name of the tool (this is ``tools_mingw`` in our case)
 4. (Optional) The tool variant name. We saw a list of these when we ran
-   :ref:`aqt list-tool <list-tool command>` with the `tool name` argument filled in.
+   :ref:`aqt list-tool <list-tool command>` with the ``tool name`` argument filled in.
 
-To install `mingw`, you could use this command (please don't):
+To install ``mingw``, you could use this command (please don't):
 
 .. code-block:: console
 
     $ aqt install-tool windows desktop tools_mingw    # please don't run this!
 
-Using this command will install every tool variant available in `tools_mingw`;
+Using this command will install every tool variant available in ``tools_mingw``;
 in this case, you would install 10 different versions of the same tool.
-For some tools, like `qtcreator` or `ifw`, this is an appropriate thing to do,
+For some tools, like ``qtcreator`` or ``ifw``, this is an appropriate thing to do,
 since each tool variant is a different program.
-However, for tools like `mingw` and `vcredist`, it would make more sense to use
+However, for tools like ``mingw`` and ``vcredist``, it would make more sense to use
 :ref:`aqt list-tool <list-tool command>` to see what tool variants are available,
 and then install just the tool variant you are interested in, like this:
 
 .. code-block:: console
 
     $ aqt install-tool windows desktop tools_mingw qt.tools.win64_mingw730
 
@@ -452,15 +452,15 @@
 archives that you may or may not need, and a typical installation can take up
 more disk space than necessary. If you installed the module ``debug_info``, it
 may have installed more than 1 gigabyte of data. This section will help you to
 reduce the footprint of your Qt installation.
 
 .. note::
 
-    Be careful about using the ``--archives`` flag; it is marked `Advanced` for a reason!
+    Be careful about using the ``--archives`` flag; it is marked ``Advanced`` for a reason!
     It is very easy to misuse this command and end up with a Qt installation that
     is missing the components that you need.
     Don't use it unless you know what you are doing!
 
 
 Minimum Qt Installation
 ```````````````````````
```

### Comparing `aqtinstall-3.1.8/docs/installation.rst` & `aqtinstall-3.1.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/CODE_OF_CONDUCT.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/CONTRIBUTE.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/SECURITY.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/SECURITY.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/authors.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/authors.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/changes.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/changes.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/cli.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/cli.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/configuration.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/configuration.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/getting_started.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/getting_started.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/index.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/ja/LC_MESSAGES/installation.po` & `aqtinstall-3.1.9/docs/locale/ja/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/CODE_OF_CONDUCT.pot` & `aqtinstall-3.1.9/docs/locale/pot/CODE_OF_CONDUCT.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/CONTRIBUTE.pot` & `aqtinstall-3.1.9/docs/locale/pot/CONTRIBUTE.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/SECURITY.pot` & `aqtinstall-3.1.9/docs/locale/pot/SECURITY.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/authors.pot` & `aqtinstall-3.1.9/docs/locale/pot/authors.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/changes.pot` & `aqtinstall-3.1.9/docs/locale/pot/changes.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/cli.pot` & `aqtinstall-3.1.9/docs/locale/pot/cli.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/configuration.pot` & `aqtinstall-3.1.9/docs/locale/pot/configuration.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/getting_started.pot` & `aqtinstall-3.1.9/docs/locale/pot/getting_started.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/index.pot` & `aqtinstall-3.1.9/docs/locale/pot/index.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/locale/pot/installation.pot` & `aqtinstall-3.1.9/docs/locale/pot/installation.pot`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/make.bat` & `aqtinstall-3.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/docs/previous_changes.rst` & `aqtinstall-3.1.9/docs/previous_changes.rst`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
 -------
 
 * Improve error messages when command argument is wrong.
 
 Fixed
 -----
 
-* Work around for http://download.qt.io/ returns wrong metalink xml data.(#105, #106)
+* Work around for https://download.qt.io/ returns wrong metalink xml data.(#105, #106)
 
 
 `v0.8a1`_ (28, Feb., 2020)
 ==========================
 
 Changed
 -------
```

### Comparing `aqtinstall-3.1.8/pyproject.toml` & `aqtinstall-3.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 requires-python = ">=3.7"
 dependencies = [
     "bs4",  # canonical name is beautifulsoup4
     "defusedxml",
     "humanize",
     "patch>=1.16",
     "py7zr>=0.20.6",
-    "requests>2.20.0",
+    "requests>=2.31.0",
     "semantic-version",
     "texttable",
 ]
 dynamic = ["version", "readme"]
 
 [tool.setuptools]
 packages = ["aqt"]
@@ -45,40 +45,42 @@
 [project.scripts]
 aqt = "aqt.__main__:main"
 
 [project.optional-dependencies]
 test = [
     "pytest>=6.0",
     "pytest-pep8",
-    "pytest-remotedata<0.4.0",
     "pytest-cov",
+    "pytest-remotedata>=0.4.1",
     "pytest-socket",
-    "pytest-leaks",
     "pytest-timeout",
     "pympler",
 ]
 check = [
     "mypy>=0.990",
-    "flake8<6",
+    "flake8>=6.0.0,<7.0.0",
     "flake8-black",
     "flake8-colors",
-    "flake8-isort>=5.0.3,<6.0.0",
+    "flake8-isort>=6.0.0,<7.0.0",
     "flake8-pyi",
     "flake8-typing-imports",
     "docutils",
     "check-manifest",
     "readme-renderer",
     "pygments",
     "packaging",
 ]
 docs = [
     "sphinx>=7.0",
     "sphinx_rtd_theme>=1.3",
     "sphinx-py3doc-enhanced-theme>=2.4",
 ]
+debug = [
+    "pytest-leaks",
+]
 
 [project.urls]
 Documentation = "https://aqtinstall.readthedocs.io/"
 "Bug Tracker" = "https://github.com/miurahr/aqtinstall/issues"
 Wiki = "https://github.com/miurahr/aqtinstall/wiki"
 Source = "https://github.com/miurahr/aqtinstall"
 Changelog = "https://aqtinstall.readthedocs.io/en/latest/CHANGELOG.html"
@@ -207,35 +209,31 @@
 extras = docs
 commands =
     sphinx-build {posargs:-E} -W -b html docs build/docs
     sphinx-build -W -b linkcheck docs build/docs
 
 [testenv:py39d]
 basepython = python3.9d
-extras = test
+extras = test, debug
 commands =
     python3.9-dbg -m pytest -v --no-cov -R : -k "test_install"
-deps =
-    pytest
-    pytest-leaks
-    pytest-remotedata<0.4.0
-    pytest-socket
-    pytest-cov
 
 [testenv:mprof]
 basepython = python3.9
+extras = debug
 commands =
     mprof run --multiprocess python -m aqt install-qt -O /tmp -d /tmp linux desktop 6.2.1
     mprof plot --output memory-profile.png
 deps =
     memory_profiler
     matplotlib
 
 [testenv:fil]
 basepython = python3.9
+extras = debug
 commands =
     fil-profile run -m aqt install-qt -O /tmp -d /tmp linux desktop 6.2.1
 deps =
     filprofiler
 
 [testenv:coveralls]
 deps =
```

### Comparing `aqtinstall-3.1.8/tests/data/linux-android-expect.json` & `aqtinstall-3.1.9/tests/data/linux-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/linux-android.html` & `aqtinstall-3.1.9/tests/data/linux-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/linux-desktop-expect.json` & `aqtinstall-3.1.9/tests/data/linux-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/linux-desktop.html` & `aqtinstall-3.1.9/tests/data/linux-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-android-expect.json` & `aqtinstall-3.1.9/tests/data/mac-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-android.html` & `aqtinstall-3.1.9/tests/data/mac-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-expect.json` & `aqtinstall-3.1.9/tests/data/mac-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-sdktool-update.xml` & `aqtinstall-3.1.9/tests/data/mac-desktop-sdktool-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_cmake-update.xml` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_cmake-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_ifw-update.xml` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_ifw-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtcreator-expect.json` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtcreator-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtcreator-update.xml` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtcreator-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtdesignstudio-expect.json` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtdesignstudio-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop-tools_qtdesignstudio-update.xml` & `aqtinstall-3.1.9/tests/data/mac-desktop-tools_qtdesignstudio-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-desktop.html` & `aqtinstall-3.1.9/tests/data/mac-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-ios-expect.json` & `aqtinstall-3.1.9/tests/data/mac-ios-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mac-ios.html` & `aqtinstall-3.1.9/tests/data/mac-ios.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mirror-expect.json` & `aqtinstall-3.1.9/tests/data/mirror-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mirror-first-td.html` & `aqtinstall-3.1.9/tests/data/mirror-first-td.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mirror-pre-a.html` & `aqtinstall-3.1.9/tests/data/mirror-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mirror-table-before-pre-a.html` & `aqtinstall-3.1.9/tests/data/mirror-table-before-pre-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/mirror-tag-in-a.html` & `aqtinstall-3.1.9/tests/data/mirror-tag-in-a.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/settings_no_concurrency.ini` & `aqtinstall-3.1.9/tests/data/settings_no_concurrency.ini`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5140-expect.json` & `aqtinstall-3.1.9/tests/data/windows-5140-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5140-update.xml` & `aqtinstall-3.1.9/tests/data/windows-5140-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5140-wasm-update.xml` & `aqtinstall-3.1.9/tests/data/windows-5140-wasm-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5150-expect.json` & `aqtinstall-3.1.9/tests/data/windows-5150-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5150-update.xml` & `aqtinstall-3.1.9/tests/data/windows-5150-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5152-src-doc-example-expect.json` & `aqtinstall-3.1.9/tests/data/windows-5152-src-doc-example-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-5152-src-doc-example-update.xml` & `aqtinstall-3.1.9/tests/data/windows-5152-src-doc-example-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-620-android-armv7-update.xml` & `aqtinstall-3.1.9/tests/data/windows-620-android-armv7-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-620-expect.json` & `aqtinstall-3.1.9/tests/data/windows-620-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-620-update.xml` & `aqtinstall-3.1.9/tests/data/windows-620-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-650-wasm-multi-update.xml` & `aqtinstall-3.1.9/tests/data/windows-650-wasm-multi-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-650-wasm-single-update.xml` & `aqtinstall-3.1.9/tests/data/windows-650-wasm-single-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-android-expect.json` & `aqtinstall-3.1.9/tests/data/windows-android-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-android.html` & `aqtinstall-3.1.9/tests/data/windows-android.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop-expect.json` & `aqtinstall-3.1.9/tests/data/windows-desktop-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop-tools-mingw-updates.xml` & `aqtinstall-3.1.9/tests/data/windows-desktop-tools-mingw-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop-tools-qtcreator-updates.xml` & `aqtinstall-3.1.9/tests/data/windows-desktop-tools-qtcreator-updates.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop-tools_vcredist-expect.json` & `aqtinstall-3.1.9/tests/data/windows-desktop-tools_vcredist-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop-tools_vcredist-update.xml` & `aqtinstall-3.1.9/tests/data/windows-desktop-tools_vcredist-update.xml`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-desktop.html` & `aqtinstall-3.1.9/tests/data/windows-desktop.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-winrt-expect.json` & `aqtinstall-3.1.9/tests/data/windows-winrt-expect.json`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/data/windows-winrt.html` & `aqtinstall-3.1.9/tests/data/windows-winrt.html`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_archives.py` & `aqtinstall-3.1.9/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_cli.py` & `aqtinstall-3.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_connection.py` & `aqtinstall-3.1.9/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_doc_archives.py` & `aqtinstall-3.1.9/tests/test_doc_archives.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_helper.py` & `aqtinstall-3.1.9/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_install.py` & `aqtinstall-3.1.9/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_list.py` & `aqtinstall-3.1.9/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tests/test_updater.py` & `aqtinstall-3.1.9/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `aqtinstall-3.1.8/tools/build_standalone.py` & `aqtinstall-3.1.9/tools/build_standalone.py`

 * *Files identical despite different names*

