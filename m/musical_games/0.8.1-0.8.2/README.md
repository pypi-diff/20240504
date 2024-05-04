# Comparing `tmp/musical_games-0.8.1.tar.gz` & `tmp/musical_games-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "musical_games-0.8.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.8.1.tar` & `musical_games-0.8.2.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.1/.coveragerc
--rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.1/.editorconfig
--rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.1/.gitchangelog.rc
--rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.1/.gitchangelog.tpl
--rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.1/.gitignore
--rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.1/.travis.yml
--rw-r--r--   0        0        0     1605 2024-05-01 12:33:23.050622 musical_games-0.8.1/CHANGELOG.rst
--rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.1/LICENSE
--rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.1/Makefile
--rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.1/README.rst
--rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.1/docs/Makefile
--rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/authors.rst
--rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.1/docs/conf.py
--rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/contributing.rst
--rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/history.rst
--rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/index.rst
--rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/installation.rst
--rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.1/docs/make.bat
--rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/modules.rst
--rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.1/docs/musical_games.converters.rst
--rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.dice_games.lilypond.rst
--rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.dice_games.rst
--rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/musical_games.rst
--rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/readme.rst
--rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.1/docs/usage.rst
--rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/__init__.py
--rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.1/musical_games/__version__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.1/musical_games/data/dice_games/__init__.py
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
--rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
--rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
--rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     2746 2024-05-01 10:01:07.522475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
--rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
--rw-r--r--   0        0        0     2217 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6412 2024-05-01 09:58:30.166473 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     6150 2024-05-01 09:58:30.166473 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2344 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    18686 2024-05-01 09:40:49.846455 musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4062 2024-05-01 10:04:40.962478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
--rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
--rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3532 2024-05-01 10:06:57.114481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
--rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
--rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/__init__.py
--rw-r--r--   0        0        0     8337 2024-04-16 05:05:56.478852 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
--rw-r--r--   0        0        0     1829 2024-05-01 10:07:32.298481 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2795 2024-05-01 10:10:19.590484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3764 2024-05-01 10:10:19.582484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1257 2024-05-01 10:10:19.642484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1475 2024-05-01 10:10:19.558484 musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-01 10:10:19.542484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     2713 2024-05-01 10:10:19.622484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     3712 2024-05-01 10:10:19.610484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1257 2024-05-01 10:10:19.570484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1475 2024-05-01 10:10:19.602484 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
--rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-r--r--   0        0        0     4165 2024-05-01 10:11:25.474485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
--rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
--rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
--rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
--rw-r--r--   0        0        0     2104 2024-05-01 12:32:39.650622 musical_games-0.8.1/musical_games/data/lilypond_utils/clef_changes.ly
--rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.1/musical_games/dice_games/__init__.py
--rw-r--r--   0        0        0    45031 2024-05-01 09:20:19.862435 musical_games-0.8.1/musical_games/dice_games/base.py
--rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.1/musical_games/dice_games/data_csv.py
--rw-r--r--   0        0        0    16662 2024-05-01 09:24:08.890439 musical_games-0.8.1/musical_games/dice_games/dice_games.py
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/base.py
--rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/exceptions.py
--rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/images.py
--rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.1/musical_games/external/lilypond.py
--rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.1/musical_games/external/midi_converters.py
--rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.1/musical_games/external/utils.py
--rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.1/musical_games/external/wav_converters.py
--rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.1/musical_games/utils.py
--rw-r--r--   0        0        0     1117 2024-05-01 12:32:51.034622 musical_games-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.1/scripts/__init__.py
--rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_cpe_bach.py
--rw-r--r--   0        0        0     3501 2024-05-01 12:32:39.650622 musical_games-0.8.1/scripts/demo_gerlach_scottish_dance.py
--rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_kirnberger_meneut_trio.py
--rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_kirnberger_polonaise.py
--rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_mozart_contredanse.py
--rw-r--r--   0        0        0     1852 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_mozart_waltz.py
--rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.1/scripts/demo_stadler_meneut_trio.py
--rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.1/scripts/lilypond_copy.py
--rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.1/scripts/lilypond_copy2.py
--rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.1/tox.ini
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.8.2/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.8.2/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.8.2/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.8.2/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.8.2/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.8.2/.travis.yml
+-rw-r--r--   0        0        0     1975 2024-05-04 12:44:01.582548 musical_games-0.8.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.8.2/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.8.2/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.8.2/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.8.2/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.8.2/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.8.2/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.8.2/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.8.2/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.8.2/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.8.2/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.8.2/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.8.2/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1426 2024-05-01 10:00:27.942474 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1773 2024-05-01 10:01:07.542475 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2987 2024-05-04 11:52:35.602498 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      524 2024-05-01 10:01:25.466475 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      623 2024-05-01 10:01:48.778476 musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-30 09:20:04.502864 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/__init__.py
+-rw-r--r--   0        0        0     2217 2024-05-01 12:32:39.650622 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     8375 2024-05-03 10:05:04.980883 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     6391 2024-05-04 11:52:35.590498 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1208 2024-05-01 12:32:39.650622 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2344 2024-05-01 12:32:39.650622 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    18686 2024-05-01 09:40:49.846455 musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2515 2024-05-01 10:02:26.562476 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:02:36.282477 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4303 2024-05-04 11:52:35.610498 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:04:40.982478 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:04:40.990478 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     5346 2024-04-16 05:05:56.478852 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2867 2024-05-01 10:06:57.106481 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4350 2024-05-01 10:06:57.126481 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3773 2024-05-04 11:54:20.298500 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1634 2024-05-01 10:06:57.134481 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     2046 2024-05-01 10:06:57.086481 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-16 05:05:56.478852 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/__init__.py
+-rw-r--r--   0        0        0     8219 2024-05-04 12:42:02.922546 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv
+-rw-r--r--   0        0        0     1439 2024-05-04 12:39:21.850544 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2929 2024-05-04 12:41:06.802545 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4138 2024-05-04 12:41:06.842545 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:41:06.822545 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.854545 musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1421 2024-05-04 12:21:30.450526 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2847 2024-05-04 12:35:43.522540 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4087 2024-05-04 12:35:43.510540 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      892 2024-05-04 12:22:16.662527 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1090 2024-05-04 12:41:06.830545 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0     9398 2024-05-04 12:21:02.330526 musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2534 2024-05-01 10:10:19.634484 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6430 2024-05-01 10:11:25.454485 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4406 2024-05-04 11:52:35.630499 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1115 2024-05-01 10:11:25.482485 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     1313 2024-05-01 10:11:25.494485 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0     2104 2024-05-01 12:32:39.650622 musical_games-0.8.2/musical_games/data/lilypond_utils/clef_changes.ly
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.8.2/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    45998 2024-05-03 10:15:04.388862 musical_games-0.8.2/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.8.2/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    17130 2024-05-04 12:38:10.242543 musical_games-0.8.2/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/external/images.py
+-rw-r--r--   0        0        0     3595 2024-04-15 05:04:22.919891 musical_games-0.8.2/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.8.2/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.8.2/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.8.2/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4835 2024-04-18 13:39:38.231087 musical_games-0.8.2/musical_games/utils.py
+-rw-r--r--   0        0        0     1117 2024-05-04 12:44:01.466548 musical_games-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.8.2/scripts/__init__.py
+-rw-r--r--   0        0        0     1995 2024-04-18 13:39:38.231087 musical_games-0.8.2/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     2365 2024-05-04 12:17:40.594523 musical_games-0.8.2/scripts/demo_gerlach_scottish_dance.py
+-rw-r--r--   0        0        0     2228 2024-04-18 13:39:38.231087 musical_games-0.8.2/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1896 2024-04-18 13:39:38.231087 musical_games-0.8.2/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1898 2024-04-18 13:39:38.231087 musical_games-0.8.2/scripts/demo_mozart_contredanse.py
+-rw-r--r--   0        0        0     1852 2024-05-04 12:36:25.506541 musical_games-0.8.2/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     2329 2024-04-18 13:39:38.231087 musical_games-0.8.2/scripts/demo_stadler_meneut_trio.py
+-rw-r--r--   0        0        0    26645 2024-04-30 09:20:04.502864 musical_games-0.8.2/scripts/lilypond_copy.py
+-rw-r--r--   0        0        0    29517 2024-04-30 09:20:04.502864 musical_games-0.8.2/scripts/lilypond_copy2.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.8.2/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.8.2/tox.ini
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 musical_games-0.8.2/PKG-INFO
```

### Comparing `musical_games-0.8.1/.gitchangelog.rc` & `musical_games-0.8.2/.gitchangelog.rc`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/.gitignore` & `musical_games-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/CHANGELOG.rst` & `musical_games-0.8.2/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 *********
 Changelog
 *********
 
+v0.8.2 (2024-05-04)
+===================
+
+Changed
+-------
+- Updates the lilypond files to have split lines in the pdf output.
+
+Other
+-----
+- In the Mozart parts, removed the left_hand_alternative as a separate staff and merged it with the left_hand staff. The processing happens now in the template. The reason for this is that it made Opus-Infinity easier to program.
+
+
 v0.8.1 (2024-05-01)
 ===================
 
 Other
 -----
 - Improved the lilypond designs.
 - In Gerlach, fixed some errors and made the clef change only local to the one specific bar.
```

### Comparing `musical_games-0.8.1/LICENSE` & `musical_games-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/Makefile` & `musical_games-0.8.2/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/README.rst` & `musical_games-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/Makefile` & `musical_games-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/conf.py` & `musical_games-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/contributing.rst` & `musical_games-0.8.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/index.rst` & `musical_games-0.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/make.bat` & `musical_games-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/musical_games.converters.rst` & `musical_games-0.8.2/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.8.2/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/musical_games.dice_games.rst` & `musical_games-0.8.2/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/docs/musical_games.rst` & `musical_games-0.8.2/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/__version__.py` & `musical_games-0.8.2/musical_games/__version__.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files 7% similar despite different names*

```diff
@@ -87,9 +87,15 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 \version "2.22.1"
 \include "articulate.ly"
 
-% dance with repeats
+% menuet with repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('dance', 'piano_right_hand')}
-                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_right_hand')}
-                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_right_hand')}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
-                \tempo 4 = 70
+                \key d\major
+                \time 3/4
+                \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('dance', 'piano_left_hand')}
-                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_left_hand')}
-                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_left_hand')}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
-                \tempo 4 = 70
+                \key d\major
+                \time 3/4
+                \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
@@ -76,16 +76,16 @@
             \with {
                 midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_right_hand')}
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_right_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_right_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
+                \key g\major
+                \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
@@ -104,16 +104,16 @@
             \with {
                 midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_left_hand')}
                 midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_left_hand')}
                 midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_left_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
+                \key g\major
+                \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
@@ -127,59 +127,59 @@
 	        	}
             }
         >>
     >>
     \midi { }
 }
 
-% dance without repeats
+% menuet without repeats
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('dance', 'piano_right_hand')}
-                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_right_hand')}
-                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_right_hand')}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
-                \tempo 4 = 70
+                \key d\major
+                \time 3/4
+                \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{composition_bars['dance'][bar_index].get_bar('piano_right_hand').lilypond_str}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('dance', 'piano_left_hand')}
-                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('dance', 'piano_left_hand')}
-                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('dance', 'piano_left_hand')}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
-                \key c \major
-                \time 2/4
-                \tempo 4 = 70
+                \key d\major
+                \time 3/4
+                \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{composition_bars['dance'][bar_index].get_bar('piano_left_hand').lilypond_str}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \midi { }
 }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/composition_pdf.ly`

 * *Files 4% similar despite different names*

```diff
@@ -152,9 +152,15 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/gerlach_scottish_dance/scottish_dance_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 6% similar despite different names*

```diff
@@ -125,9 +125,15 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 \paper {
     print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
     system-system-spacing = #'((basic-distance . 15))
 
     \BLOCK{ if render_settings['single_page'] }
-        paper-height = 370\mm  %% default is 297 for a4
+        paper-height = 410\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Polonaise"
     composer = "Kirnberger"
     tagline = ##f
 }
@@ -98,9 +98,15 @@
                 }
             >>
         >>
     >>
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_dice_table_element.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/contredanse_bars.csv`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-"bar_index","piano_right_hand","piano_left_hand","piano_left_hand_alternative"
-"1","g''8[ g'' e'' c'' ]","c4 r",""
-"2","d''8[ f'' b' d'' ]","g,4 g,",""
-"3","\acciaccatura a''8 g''8 b'' 16 g'' d''4","< b, g > 4 g,",""
-"4","d' 8 [d'' fis'' a'']","d4 <c d>",""
-"5","c''4 c'","c4 c,",""
-"6","d''8 d''16 b' g'8 a'16 b'","g4 g,",""
-"7","c''8[ c'' e'' e'']","c4 c",""
-"8","d''8 [f'' b' d'']","g,4 g,",""
-"9","d''8 b' g'4","g,4 g16 f e d",""
-"10","g''8 [e'' c'' c'']","c4 r",""
-"11","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"12","c''16 b' c'' d'' c''8 c''","c4 r",""
-"13","c''8 [ e'' g'' e'']","c4 c",""
-"14","g''8 [ e'' c'' c'' ]","c4 r",""
-"15","c''16 e'' g'' e'' c''8 c''","c4 c,",""
-"16","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"17","d''16 e'' f'' e'' f'' d'' c'' b'","g,4 g,",""
-"18","e''8 [ c'' b' a']","c4 d",""
-"19","d''16 b' c'' a' g' g'' f'' d''","g,4 r",""
-"20","c''4 c'","c4 c,",""
-"21","d'8 fis'16 a' d'' fis'' a'' fis''","d4 <c d>",""
-"22","a''16 b'' a'' g'' \acciaccatura g''8 fis''8 e''16 d''","d4 <c d>",""
-"23","e''16 c'' e'' c'' a'8 fis''","c4 d",""
-"24","c'''16 b'' a'' g'' f'' e'' d'' c''","c4 r",""
-"25","d'' 8 [fis'' a'' fis'']","d 4 <c d>",""
-"26","e''8 [c'' g'' e'']","c4 c",""
-"27","a''16 g'' fis'' g'' d'' g'' d'' b'","<b, g>4 b,",""
-"28","g''16 fis'' e'' d'' c'' b' a' g'","<b, g>4 r",""
-"29","e''16 c'' g' c'' e'' c'' g'' e''","c4 c",""
-"30","g''8 [d'' d''(dis'')]","<b, g>4 b,",""
-"31","c''8 c''16 e'' f'' e'' g'' e''","c8 [ c c c ]",""
-"32","c'''8 [g'' e'' d'' ]","c4 r",""
-"33","c''16 c' e' g' c'' e'' g'' c'''","c4 c",""
-"34","g''16 b'' g'' d'' b' g'' d'' b'","g8 r g, r",""
-"35","c''16 d'' e'' d'' c'' e' g' c''","c4 c,",""
-"36","c''8 c'16 e' g'8 c''16 e''","c4 c",""
-"37","c''8 e'' g'4","c16 c' b c' c4",""
-"38","c''16 c''' g'' e'' c'' g'' e'' c''","c8 r c r",""
-"39","g''16 fis'' e'' d'' c'' b' a' g'","<b, g>4 r",""
-"40","f''16 e'' d'' c'' b' c'' d'' b'","g8 [g, g, g,]",""
-"41","c''4 c'","c4 c,",""
-"42","c''8 c''16 e'' g''8 g''16 e''","c4 r",""
-"43","d''16 cis'' d'' e'' fis'' g'' a'' fis''","d4 <c d>",""
-"44","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"45","g''8 [c''' g'' e'']","c16 d c b, c d e c",""
-"46","d''8 b' g'4","g16 g, b, d g f e d",""
-"47","c''4 c'","c4 c,",""
-"48","c''8 c''16 e'' g''8 g''16 e''","c4 r",""
-"49","e''16 c'' b' a' g' b' fis' a'","c4 d8 d,",""
-"50","d'16 fis' a' d'' fis'' a'' fis'' d''","d8 r <c d> r",""
-"51","b'16 g'' d'' b' g'4","g,4 g16 f e d",""
-"52","g''8 [ b'' g'' d'' ]","b,16 g, b, d g d b, g,",""
-"53","g''8 [ f'' d'' b']","g,16 b, d b, f d b, g,",""
-"54","c''8 [ e'' e'' e'' ]","c16 e g e c e g e",""
-"55","g''8 [ g'' b'' g'' ]","b,16 d g d b,8 b,",""
-"56","d''8 [ d'' fis'' fis'' ]","d8 fis16 a d' a fis d",""
-"57","f''8 [ f'' d'' d'' ]","g8 g,16 a, b, c d b,",""
-"58","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"59","c''4 c''8 c''","c16 e g e c e g e",""
-"60","f''8 [ f'' d'' d'']","g8 g,16 a, b, c d b,",""
-"61","d''8 [ d'' fis'' a'' ]","d16 fis a fis d8 c",""
-"62","e''8 [ e'' g'' e'' ]","c16 g, e c c' g e c",""
-"63","e''8 [ a'' g'' fis'' ]","c16 b, c a, d cis d d,",""
-"64","g''16 e'' f'' d'' c'' g'' e'' c''","c4 r",""
-"65","c''8 c'' c''4","c4 c,",""
-"66","fis''8 fis''16 a'' d'''8 a''16 fis''","d4 d",""
-"67","g''8 b''16 g'' d''8 g''16 d''","g4 b,",""
-"68","g''8 g''16 e'' c''8 c''16 e''","c4 r",""
-"69","c''8 g'16 e' c'8 c'","c4 r",""
-"70","c''4 c''8 c''","c16 g, a, b, c g, a, b,",""
-"71","<e' c''>8 <e'c''> <e' c''>4","c16c, e, g, c e g e",""
-"72","e''4 c''8 c''","c16 e g e c e g e",""
-"73","e''8 [ g'' fis'' a'' ]","c4 d",""
-"74","c''4 c'","c4 c,",""
-"75","c''4 c''8 c''","c16 g, a, b, c g, a, b,",""
-"76","d''16 c'' b' a' g'4","g,4 g16 f e d",""
-"77","d'8 fis'16 a' d''8 fis''","d4 d",""
-"78","e''8 e''16 g'' fis''8 fis''16 a''","c4 d",""
-"79","g''8 b''16 g'' d''8 g''16 d''","<b, g>4 g,",""
-"80","c''8 [ e'' e'' e'' ]","c4 r",""
-"81","c''8 [ g' c'' e'' ]","c4 r",""
-"82","d''4 d''8 d''","d16 fis a g fis d e fis",""
-"83","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"84","d''8 b' g'4","g,16 b, d g g, f e d",""
-"85","g''8 g''16 e'' c''8 c''16 e''","c4 r",""
-"86","f''8 f''16 d'' b'8 b'16 d''","g,4 g,",""
-"87","e''8 c''16 e'' g''8 e''16 c''","c4 r",""
-"88","c''8 e''16 g'' c''' g'' e'' c''","c4 r",""
-"89","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"90","d''8 [ b' g' b' ]","g8 g,16 a, b, a, b, g,",""
-"91","g''4 b''8 g''","b,16 d g d b, g, a, b,",""
-"92","g''8 [ d'' b' g' ]","g4 r",""
-"93","d''4 a''8 fis''","d16 fis a fis c fis a c",""
-"94","c''8 [ e'' g'' e'' ]","c16 e g e c e g e",""
-"95","f''8 [ d'' g'' e'' ]","g4 g,",""
-"96","d''8 [ d'' b' b' ]","g16 d b, g, g d b, g,",""
-"97","c''8 [ g' c'' e'' ]","e8 e16 e e8 c",""
-"98","c''4 c'","c4 c,",""
-"99","g'8 c''4 e''8","c16 g e g c g e g",""
-"100","b'16 a'g'a'b'c'' d'' b'","g, 4 g,",""
-"101","g''8 e''4 c''8","c16 g e g c g e g",""
-"102","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"103","g''16 c''' g'' f'' e'' c'' e'' g''","c4 r",""
-"104","g''8 d'''16 b'' g''4","g4 g,",""
-"105","c''16 b' c'' d'' e'' d'' e'' f''","c4 c",""
-"106","g''8 e''4 c''8","c16 g e g c g e g",""
-"107","d''8 b'4 g'8","b,16 d g d g f e d",""
-"108","f''16 a'' f'' d'' b' d'' b' g'","g4 g,",""
-"109","d''8 f''4 b'8","g,16 d b, d g, d b, d",""
-"110","c''8 [ e'' c'' g' ]","e8 e16 e e8 c",""
-"111","d'8 fis'16 a' d''8 fis''","d4 d",""
-"112","f''8 [ d'' b' g' ]","g4 g,",""
-"113","c''8 [ g' e' c' ]","c8 c16 c c8 c",""
-"114","g''8 a''16 g'' f'' e'' d'' c''","c4 r",""
-"115","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"116","d''8 fis''4 a''8","d8 cis 16 d c d c d",""
-"117","a''8 fis''4 d''8","d16 a fis a d a fis a",""
-"118","c''4 c'","c4 c,",""
-"119","g''8 [ c''' g'' e'' ]","c4 c",""
-"120","d''16 e'' fis'' g'' a'' b'' c''' a''","d4 fis",""
-"121","c''8 e''16 c'' g'4","c4 g,",""
-"122","c''8 [ g' e' c' ]","c4 c,",""
-"123","g''8 [ d'' b' g' ]","g4 g,",""
-"124","b'8 [ d'' g'' b'' ]","g4 g,",""
-"125","b''16 d''' c''' b'' a'' g'' fis'' g''","g4 b,",""
-"126","b'8 d'' g'4","g,4 g16 f e d",""
-"127","c''4 c'","c4 c,",""
-"128","g'8 c''4 e''8","c16 g e g c g e g",""
-"129","f''8 [ d'' b' g' ]","g4 g,",""
-"130","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"131","f''8 d''4 b'8","g,16 d b, d g, d b, d",""
-"132","e''8 c''4 a'16 fis'","c16 a fis a a, d c d",""
-"133","d''8 g''4 b''8","b,16 d g d b, d g d",""
-"134","c''16 e'' g'' e'' c'' g' c'' e''","c4 r",""
-"135","e''8 g'' f''16 e'' d'' c''","c4 c",""
-"136","d''8 fis''16 a'' d'''8 d'''","d4 fis",""
-"137","e''8 c''' b''16 a'' g'' fis''","c4 d",""
-"138","g''8 e''4 c''8","c16 e g e c e g e",""
-"139","c''8 e'' g'4","c16 g e g c g e g",""
-"140","g''8 d''4 b'8","d16 b g b d b g b",""
-"141","d''8 [ b' g' b' ]","g4 g,",""
-"142","c''8 [ g' c'' e'' ]","c8 c16 c c8 g,",""
-"143","e''8 [ c'' a' fis' ]","c4 c",""
-"144","d'8 fis'16 a' d''8 fis''","d4 d",""
-"145","<g e' c''>4 \arpeggio c''16 d'' e'' f''","c16 e g e c4",""
-"146","c''4 c'","c4 c,",""
-"147","d''16 e'' fis'' g'' a'' fis'' e'' d''","d4 fis",""
-"148","a''16 g'' a'' fis'' d''8 e''16 fis''","d4 fis",""
-"149","d'8 d'' 4 fis''16 a''","d4 r",""
-"150","g''8 e'' c''16 e'' g'' e''","c16 e g e c4",""
-"151","c''4 e''8 g''","c16 e g e c4",""
-"152","g''8 c'''16 g'' e''8 c''","c4 r",""
-"153","g''16 a'' b'' c''' d''' b'' a'' g''","g4 b,",""
-"154","f''8 [ d'' c'' b' ]","g4 b,",""
-"155","a''4 g''16 fis'' e'' d''","d16 fis a fis d8 c",""
-"156","g'' 8 b''4 g''16 d''","g4 r",""
-"157","g''16 a'' b'' c''' d'''4","g4 g,",""
-"158","c''16 d'' e'' f'' g'' e'' d'' c''","c4 c,",""
-"159","d''8 f''4 d''16 b'","g4 g,",""
-"160","d''8 b' g'16 b' d'' b'","g,16 b, d b, g,4",""
-"161","e''16 g'' e'' c'' b' a' g' fis'","c4 d",""
-"162","g''8 c''' \acciaccatura f''8 e'' d''16 c''","c4 c",""
-"163","c''16 b' c'' d'' c''8 c''","c4 c",""
-"164","b'8 [ b' g' g' ]","g,16 a, b, c d e f d",""
-"165","c''8 e''16 c'' g'8 g'","c4 r",""
-"166","g''16 a'' g'' f'' e''8 e''","c4 e16 g e c",""
-"167","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"168","e''8 c''4 a'16 fis'","c4 d",""
-"169","c''16 b' c'' d'' e''8 e''","c4 c16 e g e",""
-"170","b'16 g' b' d'' g''4","g,4 g16 f e d",""
-"171","c''4 c'","c4 c,",""
-"172","<g' b' g''>4 r","g,4 g16 f e d","g,4 g,16 a, b, cis"
-"173","b'16 g' d' b g g' b' d'' |","g,4 r",""
-"174","c''4 e''8 g'' |","c16 e g e c4",""
-"175","c'''8 [ g'' e'' c'' ] |","c4 c",""
-"176","g''8 b'' g''4 |","b,16 g, b, d g d b, g,",""
+"bar_index","piano_right_hand","piano_left_hand"
+"1","g''8[ g'' e'' c'' ]","c4 r"
+"2","d''8[ f'' b' d'' ]","g,4 g,"
+"3","\acciaccatura a''8 g''8 b'' 16 g'' d''4","< b, g > 4 g,"
+"4","d' 8 [d'' fis'' a'']","d4 <c d>"
+"5","c''4 c'","c4 c,"
+"6","d''8 d''16 b' g'8 a'16 b'","g4 g,"
+"7","c''8[ c'' e'' e'']","c4 c"
+"8","d''8 [f'' b' d'']","g,4 g,"
+"9","d''8 b' g'4","g,4 g16 f e d"
+"10","g''8 [e'' c'' c'']","c4 r"
+"11","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"12","c''16 b' c'' d'' c''8 c''","c4 r"
+"13","c''8 [ e'' g'' e'']","c4 c"
+"14","g''8 [ e'' c'' c'' ]","c4 r"
+"15","c''16 e'' g'' e'' c''8 c''","c4 c,"
+"16","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"17","d''16 e'' f'' e'' f'' d'' c'' b'","g,4 g,"
+"18","e''8 [ c'' b' a']","c4 d"
+"19","d''16 b' c'' a' g' g'' f'' d''","g,4 r"
+"20","c''4 c'","c4 c,"
+"21","d'8 fis'16 a' d'' fis'' a'' fis''","d4 <c d>"
+"22","a''16 b'' a'' g'' \acciaccatura g''8 fis''8 e''16 d''","d4 <c d>"
+"23","e''16 c'' e'' c'' a'8 fis''","c4 d"
+"24","c'''16 b'' a'' g'' f'' e'' d'' c''","c4 r"
+"25","d'' 8 [fis'' a'' fis'']","d 4 <c d>"
+"26","e''8 [c'' g'' e'']","c4 c"
+"27","a''16 g'' fis'' g'' d'' g'' d'' b'","<b, g>4 b,"
+"28","g''16 fis'' e'' d'' c'' b' a' g'","<b, g>4 r"
+"29","e''16 c'' g' c'' e'' c'' g'' e''","c4 c"
+"30","g''8 [d'' d''(dis'')]","<b, g>4 b,"
+"31","c''8 c''16 e'' f'' e'' g'' e''","c8 [ c c c ]"
+"32","c'''8 [g'' e'' d'' ]","c4 r"
+"33","c''16 c' e' g' c'' e'' g'' c'''","c4 c"
+"34","g''16 b'' g'' d'' b' g'' d'' b'","g8 r g, r"
+"35","c''16 d'' e'' d'' c'' e' g' c''","c4 c,"
+"36","c''8 c'16 e' g'8 c''16 e''","c4 c"
+"37","c''8 e'' g'4","c16 c' b c' c4"
+"38","c''16 c''' g'' e'' c'' g'' e'' c''","c8 r c r"
+"39","g''16 fis'' e'' d'' c'' b' a' g'","<b, g>4 r"
+"40","f''16 e'' d'' c'' b' c'' d'' b'","g8 [g, g, g,]"
+"41","c''4 c'","c4 c,"
+"42","c''8 c''16 e'' g''8 g''16 e''","c4 r"
+"43","d''16 cis'' d'' e'' fis'' g'' a'' fis''","d4 <c d>"
+"44","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"45","g''8 [c''' g'' e'']","c16 d c b, c d e c"
+"46","d''8 b' g'4","g16 g, b, d g f e d"
+"47","c''4 c'","c4 c,"
+"48","c''8 c''16 e'' g''8 g''16 e''","c4 r"
+"49","e''16 c'' b' a' g' b' fis' a'","c4 d8 d,"
+"50","d'16 fis' a' d'' fis'' a'' fis'' d''","d8 r <c d> r"
+"51","b'16 g'' d'' b' g'4","g,4 g16 f e d"
+"52","g''8 [ b'' g'' d'' ]","b,16 g, b, d g d b, g,"
+"53","g''8 [ f'' d'' b']","g,16 b, d b, f d b, g,"
+"54","c''8 [ e'' e'' e'' ]","c16 e g e c e g e"
+"55","g''8 [ g'' b'' g'' ]","b,16 d g d b,8 b,"
+"56","d''8 [ d'' fis'' fis'' ]","d8 fis16 a d' a fis d"
+"57","f''8 [ f'' d'' d'' ]","g8 g,16 a, b, c d b,"
+"58","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"59","c''4 c''8 c''","c16 e g e c e g e"
+"60","f''8 [ f'' d'' d'']","g8 g,16 a, b, c d b,"
+"61","d''8 [ d'' fis'' a'' ]","d16 fis a fis d8 c"
+"62","e''8 [ e'' g'' e'' ]","c16 g, e c c' g e c"
+"63","e''8 [ a'' g'' fis'' ]","c16 b, c a, d cis d d,"
+"64","g''16 e'' f'' d'' c'' g'' e'' c''","c4 r"
+"65","c''8 c'' c''4","c4 c,"
+"66","fis''8 fis''16 a'' d'''8 a''16 fis''","d4 d"
+"67","g''8 b''16 g'' d''8 g''16 d''","g4 b,"
+"68","g''8 g''16 e'' c''8 c''16 e''","c4 r"
+"69","c''8 g'16 e' c'8 c'","c4 r"
+"70","c''4 c''8 c''","c16 g, a, b, c g, a, b,"
+"71","<e' c''>8 <e'c''> <e' c''>4","c16c, e, g, c e g e"
+"72","e''4 c''8 c''","c16 e g e c e g e"
+"73","e''8 [ g'' fis'' a'' ]","c4 d"
+"74","c''4 c'","c4 c,"
+"75","c''4 c''8 c''","c16 g, a, b, c g, a, b,"
+"76","d''16 c'' b' a' g'4","g,4 g16 f e d"
+"77","d'8 fis'16 a' d''8 fis''","d4 d"
+"78","e''8 e''16 g'' fis''8 fis''16 a''","c4 d"
+"79","g''8 b''16 g'' d''8 g''16 d''","<b, g>4 g,"
+"80","c''8 [ e'' e'' e'' ]","c4 r"
+"81","c''8 [ g' c'' e'' ]","c4 r"
+"82","d''4 d''8 d''","d16 fis a g fis d e fis"
+"83","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"84","d''8 b' g'4","g,16 b, d g g, f e d"
+"85","g''8 g''16 e'' c''8 c''16 e''","c4 r"
+"86","f''8 f''16 d'' b'8 b'16 d''","g,4 g,"
+"87","e''8 c''16 e'' g''8 e''16 c''","c4 r"
+"88","c''8 e''16 g'' c''' g'' e'' c''","c4 r"
+"89","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"90","d''8 [ b' g' b' ]","g8 g,16 a, b, a, b, g,"
+"91","g''4 b''8 g''","b,16 d g d b, g, a, b,"
+"92","g''8 [ d'' b' g' ]","g4 r"
+"93","d''4 a''8 fis''","d16 fis a fis c fis a c"
+"94","c''8 [ e'' g'' e'' ]","c16 e g e c e g e"
+"95","f''8 [ d'' g'' e'' ]","g4 g,"
+"96","d''8 [ d'' b' b' ]","g16 d b, g, g d b, g,"
+"97","c''8 [ g' c'' e'' ]","e8 e16 e e8 c"
+"98","c''4 c'","c4 c,"
+"99","g'8 c''4 e''8","c16 g e g c g e g"
+"100","b'16 a'g'a'b'c'' d'' b'","g, 4 g,"
+"101","g''8 e''4 c''8","c16 g e g c g e g"
+"102","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"103","g''16 c''' g'' f'' e'' c'' e'' g''","c4 r"
+"104","g''8 d'''16 b'' g''4","g4 g,"
+"105","c''16 b' c'' d'' e'' d'' e'' f''","c4 c"
+"106","g''8 e''4 c''8","c16 g e g c g e g"
+"107","d''8 b'4 g'8","b,16 d g d g f e d"
+"108","f''16 a'' f'' d'' b' d'' b' g'","g4 g,"
+"109","d''8 f''4 b'8","g,16 d b, d g, d b, d"
+"110","c''8 [ e'' c'' g' ]","e8 e16 e e8 c"
+"111","d'8 fis'16 a' d''8 fis''","d4 d"
+"112","f''8 [ d'' b' g' ]","g4 g,"
+"113","c''8 [ g' e' c' ]","c8 c16 c c8 c"
+"114","g''8 a''16 g'' f'' e'' d'' c''","c4 r"
+"115","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"116","d''8 fis''4 a''8","d8 cis 16 d c d c d"
+"117","a''8 fis''4 d''8","d16 a fis a d a fis a"
+"118","c''4 c'","c4 c,"
+"119","g''8 [ c''' g'' e'' ]","c4 c"
+"120","d''16 e'' fis'' g'' a'' b'' c''' a''","d4 fis"
+"121","c''8 e''16 c'' g'4","c4 g,"
+"122","c''8 [ g' e' c' ]","c4 c,"
+"123","g''8 [ d'' b' g' ]","g4 g,"
+"124","b'8 [ d'' g'' b'' ]","g4 g,"
+"125","b''16 d''' c''' b'' a'' g'' fis'' g''","g4 b,"
+"126","b'8 d'' g'4","g,4 g16 f e d"
+"127","c''4 c'","c4 c,"
+"128","g'8 c''4 e''8","c16 g e g c g e g"
+"129","f''8 [ d'' b' g' ]","g4 g,"
+"130","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"131","f''8 d''4 b'8","g,16 d b, d g, d b, d"
+"132","e''8 c''4 a'16 fis'","c16 a fis a a, d c d"
+"133","d''8 g''4 b''8","b,16 d g d b, d g d"
+"134","c''16 e'' g'' e'' c'' g' c'' e''","c4 r"
+"135","e''8 g'' f''16 e'' d'' c''","c4 c"
+"136","d''8 fis''16 a'' d'''8 d'''","d4 fis"
+"137","e''8 c''' b''16 a'' g'' fis''","c4 d"
+"138","g''8 e''4 c''8","c16 e g e c e g e"
+"139","c''8 e'' g'4","c16 g e g c g e g"
+"140","g''8 d''4 b'8","d16 b g b d b g b"
+"141","d''8 [ b' g' b' ]","g4 g,"
+"142","c''8 [ g' c'' e'' ]","c8 c16 c c8 g,"
+"143","e''8 [ c'' a' fis' ]","c4 c"
+"144","d'8 fis'16 a' d''8 fis''","d4 d"
+"145","<g e' c''>4 \arpeggio c''16 d'' e'' f''","c16 e g e c4"
+"146","c''4 c'","c4 c,"
+"147","d''16 e'' fis'' g'' a'' fis'' e'' d''","d4 fis"
+"148","a''16 g'' a'' fis'' d''8 e''16 fis''","d4 fis"
+"149","d'8 d'' 4 fis''16 a''","d4 r"
+"150","g''8 e'' c''16 e'' g'' e''","c16 e g e c4"
+"151","c''4 e''8 g''","c16 e g e c4"
+"152","g''8 c'''16 g'' e''8 c''","c4 r"
+"153","g''16 a'' b'' c''' d''' b'' a'' g''","g4 b,"
+"154","f''8 [ d'' c'' b' ]","g4 b,"
+"155","a''4 g''16 fis'' e'' d''","d16 fis a fis d8 c"
+"156","g'' 8 b''4 g''16 d''","g4 r"
+"157","g''16 a'' b'' c''' d'''4","g4 g,"
+"158","c''16 d'' e'' f'' g'' e'' d'' c''","c4 c,"
+"159","d''8 f''4 d''16 b'","g4 g,"
+"160","d''8 b' g'16 b' d'' b'","g,16 b, d b, g,4"
+"161","e''16 g'' e'' c'' b' a' g' fis'","c4 d"
+"162","g''8 c''' \acciaccatura f''8 e'' d''16 c''","c4 c"
+"163","c''16 b' c'' d'' c''8 c''","c4 c"
+"164","b'8 [ b' g' g' ]","g,16 a, b, c d e f d"
+"165","c''8 e''16 c'' g'8 g'","c4 r"
+"166","g''16 a'' g'' f'' e''8 e''","c4 e16 g e c"
+"167","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"168","e''8 c''4 a'16 fis'","c4 d"
+"169","c''16 b' c'' d'' e''8 e''","c4 c16 e g e"
+"170","b'16 g' b' d'' g''4","g,4 g16 f e d"
+"171","c''4 c'","c4 c,"
+"172","<g' b' g''>4 r","<<{\voiceOne g,4 g16 f e d} \new Voice {\voiceTwo g,4 g,16 a, b, cis}>>"
+"173","b'16 g' d' b g g' b' d'' |","g,4 r"
+"174","c''4 e''8 g'' |","c16 e g e c4"
+"175","c'''8 [ g'' e'' c'' ] |","c4 c"
+"176","g''8 b'' g''4 |","b,16 g, b, d g d b, g,"
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/bar_overview.ly`

 * *Files 20% similar despite different names*

```diff
@@ -41,19 +41,15 @@
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
             }
             {
                 \clef bass
                 \time 2/4
                 \BLOCK{ for bar_ind, bar in bar_collections['contredanse'].get_bars('piano_left_hand').items() }
-                    \BLOCK{ if bar_collections['contredanse'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str != '' }
-                        <<{\voiceOne \VAR{bar.lilypond_str}} \new Voice {\voiceTwo \VAR{bar_collections['contredanse'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str}}>>
-                    \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
-                    \BLOCK{ endif }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_midi.ly`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,18 @@
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} }
+                \alternative {
+                    {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}}
+                    {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}}
+                }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
@@ -53,15 +56,18 @@
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
+                \alternative {
+                    {\VAR{split_voices(composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str)[0]}}
+                    {\VAR{split_voices(composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str)[1]}}
+                }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/composition_pdf.ly`

 * *Files 23% similar despite different names*

```diff
@@ -64,15 +64,18 @@
                 \time 2/4
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}} }
+                \alternative {
+                    {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}}
+                    {\VAR{composition_bars['contredanse'][7].get_bar('piano_right_hand').lilypond_str}}
+                }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
                         \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
@@ -89,15 +92,18 @@
                 \time 2/4
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['contredanse'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
+                \alternative {
+                    {\VAR{split_voices(composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str)[0]}}
+                    {\VAR{split_voices(composition_bars['contredanse'][7].get_bar('piano_left_hand').lilypond_str)[1]}}
+                }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \VAR{composition_bars['contredanse'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
@@ -105,10 +111,15 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
-
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly`

 * *Files 20% similar despite different names*

```diff
@@ -19,31 +19,31 @@
         <<
             {
                 \key c\major
             }
             {
                 \clef treble
                 \time 2/4
+                \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
             }
             {
                 \clef bass
                 \time 2/4
-                \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
-                    <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
-                \BLOCK{ else }
-                    \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
-                \BLOCK{ endif }
+                \BLOCK{ for synchronous_bar in synchronous_bars }
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = #0
     }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_contredanse/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,50 @@
     paper-width = 100\mm
 }
 \header{
     title = ""
     tagline = ##f
 }
 \score {
-    \header {
-        piece = \markup { \fontsize #1 "" }
-        title = ""
-    }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \key c\major
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef treble
-                \time 2/4
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
-                \key c\major
+                \BLOCK{ if table_name == 'menuet' }
+                    \key d\major
+                \BLOCK{ else }
+                    \key g\major
+                \BLOCK{ endif }
             }
             {
                 \clef bass
-                \time 2/4
+                \time 3/4
                 \BLOCK{ for synchronous_bar in synchronous_bars }
-                    \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
-                        <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
-                    \BLOCK{ else }
-                        \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
-                    \BLOCK{ endif }
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
-        indent = #0
+        indent = 0\mm
     }
 }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files 20% similar despite different names*

```diff
@@ -41,19 +41,15 @@
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
             }
             {
                 \clef bass
                 \time 3/8
                 \BLOCK{ for bar_ind, bar in bar_collections['waltz'].get_bars('piano_left_hand').items() }
-                    \BLOCK{ if bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str != '' }
-                        <<{\voiceOne \VAR{bar.lilypond_str}} \new Voice {\voiceTwo \VAR{bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str}}>>
-                    \BLOCK{ else }
-                        \VAR{bar.lilypond_str}
-                    \BLOCK{ endif }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,18 @@
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} }
+                \alternative {
+                    {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}}
+                    {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}}
+                }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
                         \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
@@ -53,15 +56,18 @@
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
+                \alternative {
+                    {\VAR{split_voices(composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str)[0]}}
+                    {\VAR{split_voices(composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str)[1]}}
+                }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files 13% similar despite different names*

```diff
@@ -64,15 +64,18 @@
                 \time 3/8
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
                         \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} }
+                \alternative {
+                    {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}}
+                    {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}}
+                }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
                         \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
@@ -89,15 +92,18 @@
                 \time 3/8
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
 		                \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
+                \alternative {
+                    {\VAR{split_voices(composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str)[0]}}
+                    {\VAR{split_voices(composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str)[1]}}
+                }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
     		            \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
@@ -105,10 +111,16 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_dice_table_element.ly`

 * *Files 20% similar despite different names*

```diff
@@ -19,31 +19,31 @@
         <<
             {
                 \key c\major
             }
             {
                 \clef treble
                 \time 3/8
+                \BLOCK{ for synchronous_bar in synchronous_bars }
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
             }
             {
                 \clef bass
                 \time 3/8
-                \BLOCK{ if synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str != '' }
-                    <<{\voiceOne \VAR{synchronous_bar.get_bar('piano_left_hand').lilypond_str}} \new Voice {\voiceTwo \VAR{synchronous_bar.get_bar('piano_left_hand_alternative').lilypond_str}}>>
-                \BLOCK{ else }
-                    \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
-                \BLOCK{ endif }
+                \BLOCK{ for synchronous_bar in synchronous_bars }
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
+                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = #0
     }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-"bar_index","piano_right_hand","piano_left_hand","piano_left_hand_alternative"
-"1","f''8 d''8 g''8","f8 d8 g8",""
-"2","a'8 fis'16 g'16 b'16 g''16","<b, g>4 r8",""
-"3","g''8 c''8 e''8","<c e>4 r8",""
-"4","g''8 d''4 \trill","g,16 b,16 g8 b,8",""
-"5","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"6","g'8 c''8 e''8","<c e>4 r8",""
-"7","e''16 c''16 e''16 g''16 c'''16 g''16","<c g>4 r8",""
-"8","c''4 r8","c8 g,8 c,8",""
-"9","<c'' e''>8 <b' d''>8 r8","g4 g,8",""
-"10","b'16 a'16 b'16 c''16 d''16 b'16","g4 r8",""
-"11","e''16 c''16 b'16 a'16 g'16 fis'16","c8 d8 d,8",""
-"12","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8",""
-"13","c''8 g'8 e'8","<g e>4 r8",""
-"14","c''4 r8","c8 g,8 c,8",""
-"15","e''8 g''16 e''16 c''8","<c g>4 <c e>8",""
-"16","a''8 fis''8 d''8","<d fis>4 <c fis>8",""
-"17","c''16 g'16 c''16 e''16 g'16 c''16","<e g>4 r8",""
-"18","g'8 (c''8 e''8)","<c e>4 <c g>8",""
-"19","e''16 c''16 e''8 g''8","<c g>4 <c e>8",""
-"20","g''8 b''16 d'''16 d''8","b,4 r8",""
-"21","c''16 e''16 g''16 d''16 a'16 fis''16","c8 d8 d,8",""
-"22","e''8 c''8 g'8","c4 r8",""
-"23","f''16 e''16 d''16 e''16 f''16 g''16","f16 e16 d16 e16 f16 g16",""
-"24","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"25","d'16 fis'16 a'16 d''16 fis''16 a''16","d4 c8",""
-"26","<c'' e''>8 <c'' e''>8 <c'' e''>8","c16 e16 g16 e16 c'16 c16",""
-"27","f''16 e''16 f''16 d''16 c''16 b'16","<g b>4 r8",""
-"28","fis''16 d''16 a'16 a''16 fis''16 d''16","<c a>4 r8",""
-"29","b'16 d''16 g''16 d''16 b'8","g4 g,8",""
-"30","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"31","e''16 c''16 g'8 e''8","<c g>4 <c g>8",""
-"32","g'8 c''8 e''8","<c e>4 r8",""
-"33","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"34","e''16 c''16 d''16 b'16 g'8","g4 r8",""
-"35","a'8 d''8 fis''8","<d fis>4 <c a>8",""
-"36","a'16 e''16 d''16 g''16 fis''16 a''16","c8 d8 d,8",""
-"37","g''16 b''16 g''16 d''16 b'8","<b, d>4 r8",""
-"38","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"39","g''8 g'8 g'8","b,16 d16 g16 d16 b,16 g,16",""
-"40","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 r8",""
-"41","c''16 b'16 c''16 e''16 g'8","<c e>4 r8",""
-"42","b'16 c''16 d''16 b'16 a'16 g'16","g,4 r8",""
-"43","g''8 f''16 e''16 d''16 c''16","<c e>4 r8",""
-"44","a'8 f''16 d''16 a'16 b'16","f4 g8",""
-"45","c''16 b'16 c''16 g'16 e'16 c'16","<e g>4 r8",""
-"46","g''8 b''16 g''16 d''16 b'16","<b, d>4 r8",""
-"47","g''8 g''16 d''16 g''8","<b, d>4 r8",""
-"48","e''8 c''16 e''16 g''16 c'''16","<c g>4 <c e>8",""
-"49","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"50","c''8 e''16 c''16 g'8","<e g>4 r8",""
-"51","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8",""
-"52","d''16 cis''16 d''16 f''16 g'16 b'16","f4 g8",""
-"53","<c'' e''>8 <c'' e''>16 <d'' f''>16 <e'' g''>8","c4 r8",""
-"54","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8",""
-"55","g''8 b''8 d''8","<b, d>4 r8",""
-"56","d''16 b'16 g'8 r8","<g, g>4 g8",""
-"57","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"58","g''8 e''8 c''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"59","g''8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"60","g''8 f''16 e''16 d''16 c''16","<c e>4 r8",""
-"61","c''8 e''16 c''16 g''8","<c g>4 r8",""
-"62","e''16 c''16 b'16 g'16 a'16 fis'16","c8 d8 d,8",""
-"63","e''16 c''16 b'16 c''16 g'8","c4 r8",""
-"64","e''16 g''16 c'''16 g''16 e''16 c''16","<c g>4 <c g>8",""
-"65","d''16 a'16 d''8 fis''8","{<< {\voiceOne fis4} \new Voice {\voiceTwo d4} >> r8}",""
-"66","fis''8 a''8 fis''8","{<< {\voiceOne a8 fis8 d8} \new Voice {\voiceTwo d8 d8 c8} >>}",""
-"67","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 <e g>8",""
-"68","g''8 b''16 g''16 b'16 g''16","b,4 r8",""
-"69","g''8 e''8 c''8","<c e>4 r8",""
-"70","fis''8 a''16 fis''16 d''16 fis''16","d4 c8",""
-"71","g''16 b''16 d'''16 b''16 g''8","<b, d>4 <b, d>8",""
-"72","f''16 e''16 d''16 c''16 b'16 d''16","f4 g8",""
-"73","g''8 e''8 c''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"74","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8",""
-"75","<d'' fis''>8 <d'' fis''>8 <d'' fis''>8","c8 c8 c8",""
-"76","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 <c g>8",""
-"77","g''16 b''16 g''8 d''8","<b, d>4 <b, g>8",""
-"78","c''8 c'8 r8","c4 c,8",""
-"79","c''4 r8","c8 g,8 c,8",""
-"80","d''8 a'8 fis''8","c4 r8",""
-"81","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"82","d''16 b'16 g'8 g''8","<b, g>4 <b, d>8",""
-"83","c''4 r8","c8 g,8 c,8",""
-"84","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8",""
-"85","c''8 e''8 g'8","<e g>4 r8",""
-"86","d''8 d''16 g''16 b''8","<b, g>4 r8",""
-"87","g''8 c''8 e''8","<c e>4 <c g>8",""
-"88","g''16 d''16 g''16 b''16 g''16 d''16","<b, d>4 <b, d>8",""
-"89","f''16 e''16 d''8 g''8","f16 e16 d8 g8",""
-"90","fis''16 a''16 d'''16 a''16 fis''16 a''16","<c a>4 <c a>8",""
-"91","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"92","<b' d''>8 g''16 b''16 d''8","<g, g>4 g8",""
-"93","c''4 r8","c8 g,8 c,8",""
-"94","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"95","g''8 e''8 c''8","<c e>4 r8",""
-"96","e''8 c''8 g'8","c4 r8",""
-"97","g''16 fis''16 g''16 d''16 b'16 g'16","<b, d>4 <b, g>8",""
-"98","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"99","fis''8 a''8 d''8","<c a>4 <c a>8",""
-"100","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"101","e''16 d''16 e''16 g''16 c'''16 g''16","<c g>4 <c e>8",""
-"102","fis''16 d''16 a'8 fis''8","<c a>4 <c a>8",""
-"103","c''16 e''16 c''16 g'16 e'8","<e g>4 r8",""
-"104","e''16 d''16 e''16 g''16 c'''16 g''16","c4 r8",""
-"105","fis''8 a''16 fis''16 d''16 fis''16","c4 r8",""
-"106","a'8 d''16 c''16 b'16 a'16","c8 d8 d,8",""
-"107","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"108","e''8 g''8 c'''8","<c g>4 <c e>8",""
-"109","d''16 f''16 d''16 f''16 b'16 d''16","<f a>4 <g d'>8",""
-"110","<b' d''>16 <a' c''>16 <a' c''>16 <g' b'>16 <g' b'>16 <fis' a'>16","c8 d8 d,8",""
-"111","c''4 r8","c8 g,8 c,8",""
-"112","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"113","f''8 d''8 b'8","<g b>4 r8",""
-"114","<b' d''>8 <b' d''>8 <b' d''>8","g8 g8 g8",""
-"115","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8",""
-"116","d''16 f''16 a''16 f''16 d''16 b'16","f4 g8",""
-"117","d''16 a'16 d''16 fis''16 a''16 fis''16","<d fis>4 r8",""
-"118","e''16 a''16 g''16 b''16 fis''16 a''16","c8 d8 d,8",""
-"119","e''16 c''16 g''16 e''16 c'''16 g''16","<c e>4 r8",""
-"120","d'''8 a''16 fis''16 d''16 a'16","<d fis>4 <c fis>8",""
-"121","g''8 b''16 g''16 d''8","<b, g>4 r8",""
-"122","g''16 fis''16 g''16 b''16 d''8","<b, d>8 <b, d>8 <b, d>8",""
-"123","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"124","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8",""
-"125","g''16 e''16 d''16 b'16 g'8","g8 g,8 r8",""
-"126","c''16 g'16 c''16 e''16 g''16 <c'' e''>16","e4 e16 c16",""
-"127","<g' b' d'' g''>4 r8","g,8 g16 f16 e16 d16","g,8 b16 g16 fis16 e16"
-"128","b'8 d''8 g''8","g,4 r8",""
-"129","a''16 g''16 fis''16 g''16 d''8","<b, d>8 <b, d>8 <b, g>8",""
-"130","<e' c''>8 <e' c''>8 <e' c''>8","c8 c8 c8",""
-"131","c''4 r8","c8 g,8 c,8",""
-"132","<c'' e''>8 <b' d''>16 <g' b'>16 g'8","g8 g,8 r8",""
-"133","d''8 g''16 d''16 b'16 d''16","<b, g>4 r8",""
-"134","a'16 e''16 <b' d''>16 <a' c''>16 <g' b'>16 <fis' a'>16","c8 d8 d,8",""
-"135","fis''8 fis''16 d''16 a''8","<c d>8 <c d>8 <c d>8",""
-"136","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8",""
-"137","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"138","<a' d'' fis''>8 fis''4 \trill","d,16 d16 cis16 d16 c16 d16",""
-"139","g''16 b''16 g''16 b''16 d''8","g,4 r8",""
-"140","a'8 a'16 d''16 fis''8","<c fis>8 <c fis>8 <c a>8",""
-"141","d''16 e''16 f''16 d''16 c''16 b'16","<b, g>4 g,8",""
-"142","c''8 g'8 e''8","<c e>4 r8",""
-"143","g''8 d''16 b'16 g'8","<b, d>4 <b, d>8",""
-"144","g''8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"145","d''16 f''16 a'16 d''16 b'16 d''16","f4 g8",""
-"146","<fis' d''>8 <d'' fis''>8 <fis'' a''>8","c8 c8 c8",""
-"147","e''16 c'''16 b''16 g''16 a''16 fis''16","c8 d8 d,8",""
-"148","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8",""
-"149","f''16 d''16 a'8 b'8","f4 g8",""
-"150","<g' c'' e''>8 e''4 \trill","c16 b,16 c16 d16 e16 fis16",""
-"151","c''4 r8","c8 g,8 c,8",""
-"152","g''8 f''16 e''16 d''16 c''16","<c e>4 r8",""
-"153","d''16 a'16 fis''16 d''16 a''16 fis''16","c4 r8",""
-"154","d''16 cis''16 d''16 fis''16 a''16 fis''16","c4 r8",""
-"155","g''16 b''16 g''16 d''16 b'16 g'16","<b, d>4 r8",""
-"156","c''16 g'16 e''16 c''16 g''8","<e g>4 r8",""
-"157","e''16 d''16 e''16 g''16 c'''16 g''16","c4 r8",""
-"158","b'8 d''16 b'16 a'16 g'16","g,4 r8",""
-"159","e''16 g''16 d''16 c''16 b'16 a'16","c8 d8 d,8",""
-"160","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 <c e>8",""
-"161","<fis' d''>8 <fis' d''>8 <fis' d''>8","c8 c8 c8",""
-"162","e''16 d''16 e''16 g''16 c'''16 g''16","<c g>4 <c e>8",""
-"163","g''16 fis''16 g''16 d''16 b'16 g'16","<b, d>4 r8",""
-"164","d''8 g'4","g16 fis16 g16 d16 b,16 g,16",""
-"165","d''8 b'8 g'8","b,4 r8",""
-"166","d''16 b''16 g''16 d''16 b'8","<g b>4 r8",""
-"167","c''8 c''16 d''16 e''8","<c e>4 r8",""
-"168","g''8 f''16 e''16 d''16 c''16","<c e>4 <e g>8",""
-"169","e''16 g''16 d''16 g''16 a'16 fis''16","c8 d8 d,8",""
-"170","c''4 r8","c8 g,8 c,8",""
-"171","b'16 c''16 d''16 e''16 f''16 d''16","<g, g>4 <b, g>8",""
-"172","c''4 r8","c8 g,8 c,8",""
-"173","f''16 a''16 a'8 b'16 d''16","f4 g8",""
-"174","g'8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16",""
-"175","e''16 c''16 b'16 d''16 g''8","g8 g,8 r8",""
-"176","a''16 g''16 b''16 g''16 d''16 g''16","<b, d>4 <b, d>8",""
+"bar_index","piano_right_hand","piano_left_hand"
+"1","f''8 d''8 g''8","f8 d8 g8"
+"2","a'8 fis'16 g'16 b'16 g''16","<b, g>4 r8"
+"3","g''8 c''8 e''8","<c e>4 r8"
+"4","g''8 d''4 \trill","g,16 b,16 g8 b,8"
+"5","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"6","g'8 c''8 e''8","<c e>4 r8"
+"7","e''16 c''16 e''16 g''16 c'''16 g''16","<c g>4 r8"
+"8","c''4 r8","c8 g,8 c,8"
+"9","<c'' e''>8 <b' d''>8 r8","g4 g,8"
+"10","b'16 a'16 b'16 c''16 d''16 b'16","g4 r8"
+"11","e''16 c''16 b'16 a'16 g'16 fis'16","c8 d8 d,8"
+"12","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8"
+"13","c''8 g'8 e'8","<g e>4 r8"
+"14","c''4 r8","c8 g,8 c,8"
+"15","e''8 g''16 e''16 c''8","<c g>4 <c e>8"
+"16","a''8 fis''8 d''8","<d fis>4 <c fis>8"
+"17","c''16 g'16 c''16 e''16 g'16 c''16","<e g>4 r8"
+"18","g'8 (c''8 e''8)","<c e>4 <c g>8"
+"19","e''16 c''16 e''8 g''8","<c g>4 <c e>8"
+"20","g''8 b''16 d'''16 d''8","b,4 r8"
+"21","c''16 e''16 g''16 d''16 a'16 fis''16","c8 d8 d,8"
+"22","e''8 c''8 g'8","c4 r8"
+"23","f''16 e''16 d''16 e''16 f''16 g''16","f16 e16 d16 e16 f16 g16"
+"24","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"25","d'16 fis'16 a'16 d''16 fis''16 a''16","d4 c8"
+"26","<c'' e''>8 <c'' e''>8 <c'' e''>8","c16 e16 g16 e16 c'16 c16"
+"27","f''16 e''16 f''16 d''16 c''16 b'16","<g b>4 r8"
+"28","fis''16 d''16 a'16 a''16 fis''16 d''16","<c a>4 r8"
+"29","b'16 d''16 g''16 d''16 b'8","g4 g,8"
+"30","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"31","e''16 c''16 g'8 e''8","<c g>4 <c g>8"
+"32","g'8 c''8 e''8","<c e>4 r8"
+"33","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"34","e''16 c''16 d''16 b'16 g'8","g4 r8"
+"35","a'8 d''8 fis''8","<d fis>4 <c a>8"
+"36","a'16 e''16 d''16 g''16 fis''16 a''16","c8 d8 d,8"
+"37","g''16 b''16 g''16 d''16 b'8","<b, d>4 r8"
+"38","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"39","g''8 g'8 g'8","b,16 d16 g16 d16 b,16 g,16"
+"40","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 r8"
+"41","c''16 b'16 c''16 e''16 g'8","<c e>4 r8"
+"42","b'16 c''16 d''16 b'16 a'16 g'16","g,4 r8"
+"43","g''8 f''16 e''16 d''16 c''16","<c e>4 r8"
+"44","a'8 f''16 d''16 a'16 b'16","f4 g8"
+"45","c''16 b'16 c''16 g'16 e'16 c'16","<e g>4 r8"
+"46","g''8 b''16 g''16 d''16 b'16","<b, d>4 r8"
+"47","g''8 g''16 d''16 g''8","<b, d>4 r8"
+"48","e''8 c''16 e''16 g''16 c'''16","<c g>4 <c e>8"
+"49","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"50","c''8 e''16 c''16 g'8","<e g>4 r8"
+"51","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8"
+"52","d''16 cis''16 d''16 f''16 g'16 b'16","f4 g8"
+"53","<c'' e''>8 <c'' e''>16 <d'' f''>16 <e'' g''>8","c4 r8"
+"54","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8"
+"55","g''8 b''8 d''8","<b, d>4 r8"
+"56","d''16 b'16 g'8 r8","<g, g>4 g8"
+"57","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"58","g''8 e''8 c''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"59","g''8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"60","g''8 f''16 e''16 d''16 c''16","<c e>4 r8"
+"61","c''8 e''16 c''16 g''8","<c g>4 r8"
+"62","e''16 c''16 b'16 g'16 a'16 fis'16","c8 d8 d,8"
+"63","e''16 c''16 b'16 c''16 g'8","c4 r8"
+"64","e''16 g''16 c'''16 g''16 e''16 c''16","<c g>4 <c g>8"
+"65","d''16 a'16 d''8 fis''8","{<< {\voiceOne fis4} \new Voice {\voiceTwo d4} >> r8}"
+"66","fis''8 a''8 fis''8","{<< {\voiceOne a8 fis8 d8} \new Voice {\voiceTwo d8 d8 c8} >>}"
+"67","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 <e g>8"
+"68","g''8 b''16 g''16 b'16 g''16","b,4 r8"
+"69","g''8 e''8 c''8","<c e>4 r8"
+"70","fis''8 a''16 fis''16 d''16 fis''16","d4 c8"
+"71","g''16 b''16 d'''16 b''16 g''8","<b, d>4 <b, d>8"
+"72","f''16 e''16 d''16 c''16 b'16 d''16","f4 g8"
+"73","g''8 e''8 c''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"74","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8"
+"75","<d'' fis''>8 <d'' fis''>8 <d'' fis''>8","c8 c8 c8"
+"76","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 <c g>8"
+"77","g''16 b''16 g''8 d''8","<b, d>4 <b, g>8"
+"78","c''8 c'8 r8","c4 c,8"
+"79","c''4 r8","c8 g,8 c,8"
+"80","d''8 a'8 fis''8","c4 r8"
+"81","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"82","d''16 b'16 g'8 g''8","<b, g>4 <b, d>8"
+"83","c''4 r8","c8 g,8 c,8"
+"84","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8"
+"85","c''8 e''8 g'8","<e g>4 r8"
+"86","d''8 d''16 g''16 b''8","<b, g>4 r8"
+"87","g''8 c''8 e''8","<c e>4 <c g>8"
+"88","g''16 d''16 g''16 b''16 g''16 d''16","<b, d>4 <b, d>8"
+"89","f''16 e''16 d''8 g''8","f16 e16 d8 g8"
+"90","fis''16 a''16 d'''16 a''16 fis''16 a''16","<c a>4 <c a>8"
+"91","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"92","<b' d''>8 g''16 b''16 d''8","<g, g>4 g8"
+"93","c''4 r8","c8 g,8 c,8"
+"94","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"95","g''8 e''8 c''8","<c e>4 r8"
+"96","e''8 c''8 g'8","c4 r8"
+"97","g''16 fis''16 g''16 d''16 b'16 g'16","<b, d>4 <b, g>8"
+"98","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"99","fis''8 a''8 d''8","<c a>4 <c a>8"
+"100","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"101","e''16 d''16 e''16 g''16 c'''16 g''16","<c g>4 <c e>8"
+"102","fis''16 d''16 a'8 fis''8","<c a>4 <c a>8"
+"103","c''16 e''16 c''16 g'16 e'8","<e g>4 r8"
+"104","e''16 d''16 e''16 g''16 c'''16 g''16","c4 r8"
+"105","fis''8 a''16 fis''16 d''16 fis''16","c4 r8"
+"106","a'8 d''16 c''16 b'16 a'16","c8 d8 d,8"
+"107","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"108","e''8 g''8 c'''8","<c g>4 <c e>8"
+"109","d''16 f''16 d''16 f''16 b'16 d''16","<f a>4 <g d'>8"
+"110","<b' d''>16 <a' c''>16 <a' c''>16 <g' b'>16 <g' b'>16 <fis' a'>16","c8 d8 d,8"
+"111","c''4 r8","c8 g,8 c,8"
+"112","e''8 c''8 g'8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"113","f''8 d''8 b'8","<g b>4 r8"
+"114","<b' d''>8 <b' d''>8 <b' d''>8","g8 g8 g8"
+"115","c''16 g'16 e''16 c''16 g''16 e''16","<c e>4 r8"
+"116","d''16 f''16 a''16 f''16 d''16 b'16","f4 g8"
+"117","d''16 a'16 d''16 fis''16 a''16 fis''16","<d fis>4 r8"
+"118","e''16 a''16 g''16 b''16 fis''16 a''16","c8 d8 d,8"
+"119","e''16 c''16 g''16 e''16 c'''16 g''16","<c e>4 r8"
+"120","d'''8 a''16 fis''16 d''16 a'16","<d fis>4 <c fis>8"
+"121","g''8 b''16 g''16 d''8","<b, g>4 r8"
+"122","g''16 fis''16 g''16 b''16 d''8","<b, d>8 <b, d>8 <b, d>8"
+"123","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"124","<c'' e'>8 <c'' e'>8 <c'' e'>8","c8 c8 c8"
+"125","g''16 e''16 d''16 b'16 g'8","g8 g,8 r8"
+"126","c''16 g'16 c''16 e''16 g''16 <c'' e''>16","e4 e16 c16"
+"127","<g' b' d'' g''>4 r8","<<{\voiceOne g,8 g16 f16 e16 d16} \new Voice {\voiceTwo g,8 b16 g16 fis16 e16}>>"
+"128","b'8 d''8 g''8","g,4 r8"
+"129","a''16 g''16 fis''16 g''16 d''8","<b, d>8 <b, d>8 <b, g>8"
+"130","<e' c''>8 <e' c''>8 <e' c''>8","c8 c8 c8"
+"131","c''4 r8","c8 g,8 c,8"
+"132","<c'' e''>8 <b' d''>16 <g' b'>16 g'8","g8 g,8 r8"
+"133","d''8 g''16 d''16 b'16 d''16","<b, g>4 r8"
+"134","a'16 e''16 <b' d''>16 <a' c''>16 <g' b'>16 <fis' a'>16","c8 d8 d,8"
+"135","fis''8 fis''16 d''16 a''8","<c d>8 <c d>8 <c d>8"
+"136","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8"
+"137","c''8 g'8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"138","<a' d'' fis''>8 fis''4 \trill","d,16 d16 cis16 d16 c16 d16"
+"139","g''16 b''16 g''16 b''16 d''8","g,4 r8"
+"140","a'8 a'16 d''16 fis''8","<c fis>8 <c fis>8 <c a>8"
+"141","d''16 e''16 f''16 d''16 c''16 b'16","<b, g>4 g,8"
+"142","c''8 g'8 e''8","<c e>4 r8"
+"143","g''8 d''16 b'16 g'8","<b, d>4 <b, d>8"
+"144","g''8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"145","d''16 f''16 a'16 d''16 b'16 d''16","f4 g8"
+"146","<fis' d''>8 <d'' fis''>8 <fis'' a''>8","c8 c8 c8"
+"147","e''16 c'''16 b''16 g''16 a''16 fis''16","c8 d8 d,8"
+"148","c'''16 b''16 c'''16 g''16 e''16 c''16","<c e>4 r8"
+"149","f''16 d''16 a'8 b'8","f4 g8"
+"150","<g' c'' e''>8 e''4 \trill","c16 b,16 c16 d16 e16 fis16"
+"151","c''4 r8","c8 g,8 c,8"
+"152","g''8 f''16 e''16 d''16 c''16","<c e>4 r8"
+"153","d''16 a'16 fis''16 d''16 a''16 fis''16","c4 r8"
+"154","d''16 cis''16 d''16 fis''16 a''16 fis''16","c4 r8"
+"155","g''16 b''16 g''16 d''16 b'16 g'16","<b, d>4 r8"
+"156","c''16 g'16 e''16 c''16 g''8","<e g>4 r8"
+"157","e''16 d''16 e''16 g''16 c'''16 g''16","c4 r8"
+"158","b'8 d''16 b'16 a'16 g'16","g,4 r8"
+"159","e''16 g''16 d''16 c''16 b'16 a'16","c8 d8 d,8"
+"160","c''16 b'16 c''16 e''16 g'16 c''16","<c e>4 <c e>8"
+"161","<fis' d''>8 <fis' d''>8 <fis' d''>8","c8 c8 c8"
+"162","e''16 d''16 e''16 g''16 c'''16 g''16","<c g>4 <c e>8"
+"163","g''16 fis''16 g''16 d''16 b'16 g'16","<b, d>4 r8"
+"164","d''8 g'4","g16 fis16 g16 d16 b,16 g,16"
+"165","d''8 b'8 g'8","b,4 r8"
+"166","d''16 b''16 g''16 d''16 b'8","<g b>4 r8"
+"167","c''8 c''16 d''16 e''8","<c e>4 r8"
+"168","g''8 f''16 e''16 d''16 c''16","<c e>4 <e g>8"
+"169","e''16 g''16 d''16 g''16 a'16 fis''16","c8 d8 d,8"
+"170","c''4 r8","c8 g,8 c,8"
+"171","b'16 c''16 d''16 e''16 f''16 d''16","<g, g>4 <b, g>8"
+"172","c''4 r8","c8 g,8 c,8"
+"173","f''16 a''16 a'8 b'16 d''16","f4 g8"
+"174","g'8 c''8 e''8","<c e>16 g16 <c e>16 g16 <c e>16 g16"
+"175","e''16 c''16 b'16 d''16 g''8","g8 g,8 r8"
+"176","a''16 g''16 b''16 g''16 d''16 g''16","<b, d>4 <b, d>8"
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 4% similar despite different names*

```diff
@@ -128,9 +128,15 @@
     >>
     \layout {
         indent = 0\mm
     }
 }
 
 \BLOCK{ if render_settings['comment'] is not none }
-    \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ if '\n' in render_settings['comment'] }
+    \BLOCK{ for line in render_settings['comment'].split('\n') }
+        \markup {\fill-line \italic {"" "" "\VAR{ line }"}}
+    \BLOCK{ endfor }
+    \BLOCK{ else }
+        \markup {\fill-line \italic {"" "" "\VAR{ render_settings['comment'] }"}}
+    \BLOCK{ endif }
 \BLOCK{ endif }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_dice_table_element.ly` & `musical_games-0.8.2/musical_games/data/dice_games/mozart_contredanse/lilypond/single_bar.ly`

 * *Files 23% similar despite different names*

```diff
@@ -5,50 +5,42 @@
     paper-width = 100\mm
 }
 \header{
     title = ""
     tagline = ##f
 }
 \score {
+    \header {
+        piece = \markup { \fontsize #1 "" }
+        title = ""
+    }
     \new PianoStaff
     <<
         \new Staff
         <<
             {
-                \BLOCK{ if table_name == 'menuet' }
-                    \key d\major
-                \BLOCK{ else }
-                    \key g\major
-                \BLOCK{ endif }
+                \key c\major
             }
             {
                 \clef treble
-                \time 3/4
-                \BLOCK{ for synchronous_bar in synchronous_bars }
+                \time 2/4
                 \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
-                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
-                \BLOCK{ if table_name == 'menuet' }
-                    \key d\major
-                \BLOCK{ else }
-                    \key g\major
-                \BLOCK{ endif }
+                \key c\major
             }
             {
                 \clef bass
-                \time 3/4
-                \BLOCK{ for synchronous_bar in synchronous_bars }
+                \time 2/4
                 \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
-                \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
-        indent = 0\mm
+        indent = #0
     }
 }
```

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv` & `musical_games-0.8.2/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/data/lilypond_utils/clef_changes.ly` & `musical_games-0.8.2/musical_games/data/lilypond_utils/clef_changes.ly`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/dice_games/base.py` & `musical_games-0.8.2/musical_games/dice_games/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,33 @@
         """Get the title of this dice game.
 
         Returns:
             The title of the dice game.
         """
 
     @abstractmethod
+    def get_dice_table_names(self) -> list[str_dice_table_name]:
+        """Get a list of dice table names in this dice game.
+
+        Returns:
+            A list of the dice table names supported by this dice game.
+        """
+
+    @abstractmethod
+    def get_staff_names(self) -> dict[str_dice_table_name, list[str_staff_name]]:
+        """For each dice table name, get the staff names in the corresponding bar collection.
+
+        This is a convenience method for getting the staff names a dice table can select. Each dice table is connected
+        to a bar collection. Each of those bar collections may have one or more staffs associated with it.
+
+        Returns:
+            A dictionary mapping dice table names to list of staff names.
+        """
+
+    @abstractmethod
     def get_dice_tables(self) -> dict[str_dice_table_name, DiceTable]:
         """Get dice tables in this dice game.
 
         This should return the dice tables as a dictionary mapping an arbitrary name to a dice table. The names may be
         used by users of this class to refer to specific measures of a specific dice table. For instance in
         :meth:`compile_single_bar`.
 
@@ -57,17 +76,14 @@
             The available dice tables in this game.
         """
 
     @abstractmethod
     def get_bar_collections(self) -> dict[str_dice_table_name, BarCollection]:
         """Get the collection of bars for each dice table.
 
-        Args:
-            dice_table_name: the name of the dice table
-
         Returns:
             The collection of bars for each dice table as a bar collection object.
         """
 
     @abstractmethod
     def get_duplicate_dice_table_elements(self, dice_table_name: str_dice_table_name) -> list[set[DiceTableElement]]:
         """Get a list of all the duplicate bars for a specific dice table.
@@ -221,24 +237,28 @@
         self._author = author
         self._title = title
         self._dice_tables = dice_tables
         self._bar_collections = bar_collections
         self._jinja2_environment = jinja2_environment
         self._default_midi_settings = default_midi_settings
 
-    @classmethod
-
     @property
     def author(self) -> str:
         return self._author
 
     @property
     def title(self) -> str:
         return self._title
 
+    def get_dice_table_names(self) -> list[str_dice_table_name]:
+        return list(self._dice_tables.keys())
+
+    def get_staff_names(self) -> dict[str_dice_table_name, list[str_staff_name]]:
+        return {k: bc.get_staff_names() for k, bc in self._bar_collections.items()}
+
     def get_dice_tables(self) -> dict[str_dice_table_name, DiceTable]:
         return self._dice_tables
 
     def get_bar_collections(self) -> dict[str_dice_table_name, BarCollection]:
         return self._bar_collections
 
     def get_duplicate_dice_table_elements(self, dice_table_name: str_dice_table_name) -> list[set[DiceTableElement]]:
```

### Comparing `musical_games-0.8.1/musical_games/dice_games/data_csv.py` & `musical_games-0.8.2/musical_games/dice_games/data_csv.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/dice_games/dice_games.py` & `musical_games-0.8.2/musical_games/dice_games/dice_games.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __author__ = 'Robbert Harms'
 __date__ = '2024-04-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
+import re
 from importlib import resources
 
 import jinja2
 
 from musical_games.dice_games.base import (SimpleDiceTable, SimpleMidiSettings, SimpleDiceGame)
 from musical_games.dice_games.data_csv import SimpleBarCollectionCSVReader
 
@@ -166,16 +167,22 @@
                                                         f'data/dice_games/{data_name}/contredanse_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'contredanse': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'contredanse': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'contredanse': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
+        def split_voices(voices):
+            return re.findall(r'<<{\\voiceOne ([^}]*)} \\new Voice {\\voiceTwo ([^}]*)}>>', voices)[0]
+
+        jinja2_env = self._generate_jinja2_environment(data_name)
+        jinja2_env.globals['split_voices'] = split_voices
+
         super().__init__('Mozart', 'Contredanse', dice_tables, bar_collections,
-                         self._generate_jinja2_environment(data_name), midi_settings)
+                         jinja2_env, midi_settings)
 
 
 class MozartWaltz(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Waltz dice game by Mozart."""
         dice_tables = {
@@ -199,16 +206,22 @@
                                                         f'data/dice_games/{data_name}/waltz_bars.csv')}
 
         midi_settings = SimpleMidiSettings(
             {'waltz': {'piano_right_hand': 'acoustic grand', 'piano_left_hand': 'acoustic grand'}},
             {'waltz': {'piano_right_hand': 0, 'piano_left_hand': 0}},
             {'waltz': {'piano_right_hand': 1, 'piano_left_hand': 0.75}})
 
+        def split_voices(voices):
+            return re.findall(r'<<{\\voiceOne ([^}]*)} \\new Voice {\\voiceTwo ([^}]*)}>>', voices)[0]
+
+        jinja2_env = self._generate_jinja2_environment(data_name)
+        jinja2_env.globals['split_voices'] = split_voices
+
         super().__init__('Mozart', 'Waltz', dice_tables, bar_collections,
-                         self._generate_jinja2_environment(data_name), midi_settings)
+                         jinja2_env, midi_settings)
 
 
 class StadlerMenuetTrio(SimpleDiceGame):
 
     def __init__(self):
         """Implementation of a Menuet and Trio dice game by Stadler.
```

### Comparing `musical_games-0.8.1/musical_games/external/base.py` & `musical_games-0.8.2/musical_games/external/base.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/external/images.py` & `musical_games-0.8.2/musical_games/external/images.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/external/lilypond.py` & `musical_games-0.8.2/musical_games/external/lilypond.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/external/midi_converters.py` & `musical_games-0.8.2/musical_games/external/midi_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/external/utils.py` & `musical_games-0.8.2/musical_games/external/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/external/wav_converters.py` & `musical_games-0.8.2/musical_games/external/wav_converters.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/musical_games/utils.py` & `musical_games-0.8.2/musical_games/utils.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/pyproject.toml` & `musical_games-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "musical_games"
 description = "Implementation of musical dice games from the 18th century."
 readme = "README.rst"
-version = "0.8.1"
+version = "0.8.2"
 requires-python = ">=3.11"
 keywords = ["Musical games", "Dice games", "Piano music"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
```

### Comparing `musical_games-0.8.1/scripts/demo_cpe_bach.py` & `musical_games-0.8.2/scripts/demo_cpe_bach.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/demo_kirnberger_meneut_trio.py` & `musical_games-0.8.2/scripts/demo_kirnberger_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/demo_kirnberger_polonaise.py` & `musical_games-0.8.2/scripts/demo_kirnberger_polonaise.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/demo_mozart_contredanse.py` & `musical_games-0.8.2/scripts/demo_mozart_contredanse.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/demo_mozart_waltz.py` & `musical_games-0.8.2/scripts/demo_mozart_waltz.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/demo_stadler_meneut_trio.py` & `musical_games-0.8.2/scripts/demo_stadler_meneut_trio.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/lilypond_copy.py` & `musical_games-0.8.2/scripts/lilypond_copy.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/scripts/lilypond_copy2.py` & `musical_games-0.8.2/scripts/lilypond_copy2.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/tox.ini` & `musical_games-0.8.2/tox.ini`

 * *Files identical despite different names*

### Comparing `musical_games-0.8.1/PKG-INFO` & `musical_games-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: musical_games
-Version: 0.8.1
+Version: 0.8.2
 Summary: Implementation of musical dice games from the 18th century.
 Keywords: Musical games,Dice games,Piano music
 Author-email: Robbert Harms <robbert@xkls.nl>
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

