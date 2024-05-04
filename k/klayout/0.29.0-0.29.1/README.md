# Comparing `tmp/klayout-0.29.0.tar.gz` & `tmp/klayout-0.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klayout-0.29.0.tar", last modified: Mon Apr  1 08:11:21 2024, max compression
+gzip compressed data, was "klayout-0.29.1.tar", last modified: Sat May  4 16:37:22 2024, max compression
```

## Comparing `klayout-0.29.0.tar` & `klayout-0.29.1.tar`

### file list

```diff
@@ -1,1105 +1,1110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:21.022328 klayout-0.29.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-01 08:11:15.000000 klayout-0.29.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-01 08:11:15.000000 klayout-0.29.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 08:11:21.022328 klayout-0.29.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-01 08:11:15.000000 klayout-0.29.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-01 08:11:15.000000 klayout-0.29.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 08:11:21.022328 klayout-0.29.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-04-01 08:11:15.000000 klayout-0.29.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.822328 klayout-0.29.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.810328 klayout-0.29.0/src/ant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.826328 klayout-0.29.0/src/ant/ant/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antConfig.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antConfigPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antConfigPage.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    23487 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19423 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antObject.h
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antPlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antPropertiesPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antPropertiesPage.h
--rw-r--r--   0 runner    (1001) docker     (127)    83308 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antService.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antService.h
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antTemplate.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/antTemplate.h
--rw-r--r--   0 runner    (1001) docker     (127)    56210 2024-04-01 08:11:15.000000 klayout-0.29.0/src/ant/ant/gsiDeclAnt.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.810328 klayout-0.29.0/src/db/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.902328 klayout-0.29.0/src/db/db/
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbArray.cc
--rw-r--r--   0 runner    (1001) docker     (127)    78404 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbArray.h
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)    31463 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)    59769 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbAsIfFlatTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBox.cc
--rw-r--r--   0 runner    (1001) docker     (127)    34694 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBoxConvert.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBoxConvert.h
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBoxScanner.cc
--rw-r--r--   0 runner    (1001) docker     (127)    37098 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBoxScanner.h
--rw-r--r--   0 runner    (1001) docker     (127)    57744 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbBoxTree.h
--rw-r--r--   0 runner    (1001) docker     (127)    29399 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCell.cc
--rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCell.h
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellGraphUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellGraphUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellHullGenerator.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellHullGenerator.h
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellInst.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellInst.h
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellMapping.h
--rw-r--r--   0 runner    (1001) docker     (127)    25546 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellVariants.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCellVariants.h
--rw-r--r--   0 runner    (1001) docker     (127)    29433 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCircuit.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCircuit.h
--rw-r--r--   0 runner    (1001) docker     (127)    22620 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClip.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClip.h
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClipboard.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClipboard.h
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClipboardData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbClipboardData.h
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbColdProxy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbColdProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCommonReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCommonReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    69872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCompoundOperation.cc
--rw-r--r--   0 runner    (1001) docker     (127)   104566 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbCompoundOperation.h
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbConverters.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbConverters.h
--rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)    59720 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)    83561 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)    42357 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepShapeStore.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28569 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepShapeStore.h
--rw-r--r--   0 runner    (1001) docker     (127)    22077 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeepTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDevice.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDevice.h
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeviceAbstract.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeviceAbstract.h
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeviceClass.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23269 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbDeviceClass.h
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdge.cc
--rw-r--r--   0 runner    (1001) docker     (127)    39777 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdge.h
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgeBoolean.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgeBoolean.h
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePair.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePair.h
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairFilters.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairFilters.h
--rw-r--r--   0 runner    (1001) docker     (127)    14247 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairRelations.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairRelations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairsDelegate.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgePairsDelegate.h
--rw-r--r--   0 runner    (1001) docker     (127)    80400 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgeProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    37357 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgeProcessor.h
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)    45249 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesDelegate.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesDelegate.h
--rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesLocalOperations.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesLocalOperations.h
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesToContours.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesToContours.h
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17680 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEdgesUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbEmptyTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFillTool.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFillTool.h
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFlatTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFuzzyCellMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbFuzzyCellMapping.h
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbGenericShapeIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbGenericShapeIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbGlyphs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbGlyphs.h
--rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHash.h
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHershey.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHershey.h
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHersheyFont.h
--rw-r--r--   0 runner    (1001) docker     (127)   107868 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierNetworkProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    48042 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierNetworkProcessor.h
--rw-r--r--   0 runner    (1001) docker     (127)   105181 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierProcessor.h
--rw-r--r--   0 runner    (1001) docker     (127)    31693 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierarchyBuilder.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18045 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbHierarchyBuilder.h
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInit.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInit.h
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInstElement.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInstElement.h
--rw-r--r--   0 runner    (1001) docker     (127)    55675 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInstances.cc
--rw-r--r--   0 runner    (1001) docker     (127)    59367 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbInstances.h
--rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayer.h
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayerMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayerMapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayerProperties.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayerProperties.h
--rw-r--r--   0 runner    (1001) docker     (127)    87323 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayout.cc
--rw-r--r--   0 runner    (1001) docker     (127)    66842 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayout.h
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutContextHandler.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutContextHandler.h
--rw-r--r--   0 runner    (1001) docker     (127)    59320 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutDiff.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutDiff.h
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutLayers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutLayers.h
--rw-r--r--   0 runner    (1001) docker     (127)    93131 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutQuery.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutQuery.h
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutStateModel.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutStateModel.h
--rw-r--r--   0 runner    (1001) docker     (127)    75266 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlist.cc
--rw-r--r--   0 runner    (1001) docker     (127)    46904 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlist.h
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistEnums.h
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistFormatDefs.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistFormatDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)    35202 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistSoftConnections.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistSoftConnections.h
--rw-r--r--   0 runner    (1001) docker     (127)    31028 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutToNetlistWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematic.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematic.h
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicFormatDefs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicFormatDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicReader.h
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLayoutVsSchematicWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibrary.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibrary.h
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibraryManager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibraryManager.h
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibraryProxy.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLibraryProxy.h
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLoadLayoutOptions.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLoadLayoutOptions.h
--rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLocalOperation.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLocalOperation.h
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLocalOperationUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLocalOperationUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLog.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbLog.h
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbManager.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbManager.h
--rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28996 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMatrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMemStatistics.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMemStatistics.h
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMetaInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbMutableTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNamedLayerReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNamedLayerReader.h
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNet.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNet.h
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetShape.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetShape.h
--rw-r--r--   0 runner    (1001) docker     (127)    30142 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlist.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlist.h
--rw-r--r--   0 runner    (1001) docker     (127)    70642 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompare.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompare.h
--rw-r--r--   0 runner    (1001) docker     (127)    57796 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareCore.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareCore.h
--rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareGraph.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareGraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCompareUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCrossReference.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistCrossReference.h
--rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceClasses.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceClasses.h
--rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceExtractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceExtractor.h
--rw-r--r--   0 runner    (1001) docker     (127)    35073 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceExtractorClasses.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistDeviceExtractorClasses.h
--rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistExtractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistExtractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistObject.h
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    33086 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    21100 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReaderDelegate.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReaderDelegate.h
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReaderExpressionParser.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceReaderExpressionParser.h
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistSpiceWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbNetlistWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbObjectTag.h
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbObjectWithProperties.h
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerEdgePairs.h
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerEdges.h
--rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbOriginalLayerTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellDeclaration.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21064 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellDeclaration.h
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellHeader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellHeader.h
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellVariant.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPCellVariant.h
--rw-r--r--   0 runner    (1001) docker     (127)    19796 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPath.cc
--rw-r--r--   0 runner    (1001) docker     (127)    29202 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPath.h
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPin.h
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPoint.h
--rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)    97025 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    29218 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygonGenerators.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygonGenerators.h
--rw-r--r--   0 runner    (1001) docker     (127)    84353 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygonTools.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26980 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPolygonTools.h
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPropertiesRepository.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPropertiesRepository.h
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbPropertyConstraint.h
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    19122 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRecursiveInstanceIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRecursiveInstanceIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    30225 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRecursiveShapeIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    33107 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRecursiveShapeIterator.h
--rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    62283 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegion.h
--rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionCheckUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionCheckUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionDelegate.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionDelegate.h
--rw-r--r--   0 runner    (1001) docker     (127)    73054 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionLocalOperations.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionLocalOperations.h
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionProcessors.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14536 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionProcessors.h
--rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbRegionUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbSaveLayoutOptions.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbSaveLayoutOptions.h
--rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShape.cc
--rw-r--r--   0 runner    (1001) docker     (127)    87753 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShape.h
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeCollection.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeCollection.h
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeCollectionUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeCollectionUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeFlags.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeFlags.h
--rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31002 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeProcessor.h
--rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapeRepository.h
--rw-r--r--   0 runner    (1001) docker     (127)    60032 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    64769 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapes.h
--rw-r--r--   0 runner    (1001) docker     (127)    40124 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapes2.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapes2.h
--rw-r--r--   0 runner    (1001) docker     (127)    47851 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbShapes3.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStatic.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStatic.h
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStream.h
--rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStreamLayers.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbStreamLayers.h
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbSubCircuit.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbSubCircuit.h
--rw-r--r--   0 runner    (1001) docker     (127)    13800 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTechnology.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTechnology.h
--rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTestSupport.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTestSupport.h
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbText.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbText.h
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTexts.h
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextsDelegate.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextsDelegate.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextsUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTextsUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTilingProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTilingProcessor.h
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTrans.cc
--rw-r--r--   0 runner    (1001) docker     (127)    62716 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTrans.h
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTriangle.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTriangle.h
--rw-r--r--   0 runner    (1001) docker     (127)    47748 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTriangles.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTriangles.h
--rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbUserObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbUserObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbVariableWidthPath.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbVariableWidthPath.h
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbVector.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbWriterTools.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/dbWriterTools.h
--rw-r--r--   0 runner    (1001) docker     (127)   325050 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/fonts.cc_gen
--rw-r--r--   0 runner    (1001) docker     (127)   184001 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/glyphs.cc_gen
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbBox.cc
--rw-r--r--   0 runner    (1001) docker     (127)   206678 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbCell.cc
--rw-r--r--   0 runner    (1001) docker     (127)    24674 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbCellMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbCommonStreamOptions.cc
--rw-r--r--   0 runner    (1001) docker     (127)    61256 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbCompoundOperation.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18336 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbContainerHelpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbDeepShapeStore.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27090 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbEdge.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbEdgePair.cc
--rw-r--r--   0 runner    (1001) docker     (127)    55659 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbEdgePairs.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31684 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbEdgeProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)   115432 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbEdges.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbGlyphs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbHelpers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbHierNetworkProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbInstElement.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayerMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)   131530 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayout.cc
--rw-r--r--   0 runner    (1001) docker     (127)    37095 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayoutDiff.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayoutQuery.cc
--rw-r--r--   0 runner    (1001) docker     (127)    55810 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayoutToNetlist.cc
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayoutUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLayoutVsSchematic.cc
--rw-r--r--   0 runner    (1001) docker     (127)    42937 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLibrary.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbLog.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbManager.cc
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbMatrix.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbMetaInfo.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbMetaInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)   141898 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbNetlist.cc
--rw-r--r--   0 runner    (1001) docker     (127)    34214 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbNetlistCompare.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbNetlistCrossReference.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbNetlistDeviceClasses.cc
--rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbNetlistDeviceExtractor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbPath.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbPoint.cc
--rw-r--r--   0 runner    (1001) docker     (127)    80774 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbRecursiveInstanceIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)    39585 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbRecursiveShapeIterator.cc
--rw-r--r--   0 runner    (1001) docker     (127)   214600 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbRegion.cc
--rw-r--r--   0 runner    (1001) docker     (127)    78922 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbShape.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbShapeCollection.cc
--rw-r--r--   0 runner    (1001) docker     (127)    24866 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbShapeProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    69049 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbShapes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbTechnologies.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18118 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbText.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31749 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbTexts.cc
--rw-r--r--   0 runner    (1001) docker     (127)    40313 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbTilingProcessor.cc
--rw-r--r--   0 runner    (1001) docker     (127)    65198 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbTrans.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-04-01 08:11:15.000000 klayout-0.29.0/src/db/db/gsiDeclDbVector.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/edt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.906329 klayout-0.29.0/src/edt/edt/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtConfig.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)    20396 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtDialogs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtDialogs.h
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtDistribute.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtDistribute.h
--rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtEditorOptionsPages.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtEditorOptionsPages.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtInstPropertiesPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtInstPropertiesPage.h
--rw-r--r--   0 runner    (1001) docker     (127)    88614 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtMainService.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtMainService.h
--rw-r--r--   0 runner    (1001) docker     (127)    32548 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPCellParametersPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPCellParametersPage.h
--rw-r--r--   0 runner    (1001) docker     (127)   101661 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPartialService.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPartialService.h
--rw-r--r--   0 runner    (1001) docker     (127)    27191 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)    27342 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPropertiesPageUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPropertiesPageUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPropertiesPages.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtPropertiesPages.h
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtRecentConfigurationPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtRecentConfigurationPage.h
--rw-r--r--   0 runner    (1001) docker     (127)    56070 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtService.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtService.h
--rw-r--r--   0 runner    (1001) docker     (127)    56804 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtServiceImpl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtServiceImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/edtUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-04-01 08:11:15.000000 klayout-0.29.0/src/edt/edt/gsiDeclEdt.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/gsi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.914328 klayout-0.29.0/src/gsi/gsi/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsi.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsi.h
--rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiCallback.h
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiCallbackVar.h
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiClass.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiClass.h
--rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiClassBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiClassBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDecl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDeclBasic.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDeclBasic.h
--rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDeclInternal.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDeclTl.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiDeclTlPixelBuffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiEnums.h
--rw-r--r--   0 runner    (1001) docker     (127)    28194 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiExpression.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiExpression.h
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiExternalMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiExternalMain.h
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiInspector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiInspector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiInterpreter.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiInterpreter.h
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiIterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiMethods.cc
--rw-r--r--   0 runner    (1001) docker     (127)    66731 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiMethods.h
--rw-r--r--   0 runner    (1001) docker     (127)    63912 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiMethodsVar.h
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiObjectHolder.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiObjectHolder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiSerialisation.cc
--rw-r--r--   0 runner    (1001) docker     (127)    55924 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiSerialisation.h
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiSignals.cc
--rw-r--r--   0 runner    (1001) docker     (127)    37277 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiSignals.h
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiTypes.cc
--rw-r--r--   0 runner    (1001) docker     (127)    85918 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiTypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    26550 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiVariantArgs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-01 08:11:15.000000 klayout-0.29.0/src/gsi/gsi/gsiVariantArgs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.918328 klayout-0.29.0/src/img/img/
--rw-r--r--   0 runner    (1001) docker     (127)    57201 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/gsiDeclImg.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgLandmarksDialog.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgLandmarksDialog.h
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgNavigator.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgNavigator.h
--rw-r--r--   0 runner    (1001) docker     (127)    60689 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgPlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)    28049 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgPropertiesPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgPropertiesPage.h
--rw-r--r--   0 runner    (1001) docker     (127)    49601 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgService.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgService.h
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgStream.h
--rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgWidgets.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-01 08:11:15.000000 klayout-0.29.0/src/img/img/imgWidgets.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/laybasic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.950328 klayout-0.29.0/src/laybasic/laybasic/
--rw-r--r--   0 runner    (1001) docker     (127) 11156282 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/fixedFont.h
--rw-r--r--   0 runner    (1001) docker     (127)    56822 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayLayers.cc
--rw-r--r--   0 runner    (1001) docker     (127)   125663 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayLayoutViewBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayMarker.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22093 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayMenu.cc
--rw-r--r--   0 runner    (1001) docker     (127)    52738 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayRdbAdded.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayTlAdded.cc
--rw-r--r--   0 runner    (1001) docker     (127)    53092 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gtf.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gtf.h
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/gtfdummy.cc
--rw-r--r--   0 runner    (1001) docker     (127)    47760 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layAbstractMenu.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26533 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layAbstractMenu.h
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layAnnotationShapes.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layAnnotationShapes.h
--rw-r--r--   0 runner    (1001) docker     (127)    21413 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmap.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmap.h
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmapRenderer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmapRenderer.h
--rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmapsToImage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBitmapsToImage.h
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBookmarkList.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layBookmarkList.h
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCanvasPlane.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCanvasPlane.h
--rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCellView.cc
--rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCellView.h
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layColorPalette.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layColorPalette.h
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layConverters.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layConverters.h
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCursor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layCursor.h
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDispatcher.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDispatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDisplayState.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDisplayState.h
--rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDitherPattern.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDitherPattern.h
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDragDropData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDragDropData.h
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDrawing.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layDrawing.h
--rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layEditable.cc
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layEditable.h
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layEditorServiceBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layEditorServiceBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    29779 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layFinder.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layFinder.h
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layFixedFont.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layFixedFont.h
--rw-r--r--   0 runner    (1001) docker     (127)    59139 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayerProperties.cc
--rw-r--r--   0 runner    (1001) docker     (127)    49544 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayerProperties.h
--rw-r--r--   0 runner    (1001) docker     (127)    30362 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayoutCanvas.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayoutCanvas.h
--rw-r--r--   0 runner    (1001) docker     (127)   160373 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayoutViewBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)    81866 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayoutViewBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLayoutViewConfig.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLineStylePalette.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLineStylePalette.h
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLineStyles.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layLineStyles.h
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMargin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMargin.h
--rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMarker.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMarker.h
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMouseTracker.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMouseTracker.h
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMove.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layMove.h
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layNativePlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layNativePlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layNetColorizer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layNetColorizer.h
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layObjectInstPath.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layObjectInstPath.h
--rw-r--r--   0 runner    (1001) docker     (127)    41689 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layParsedLayerSource.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layParsedLayerSource.h
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPixelBufferPainter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPixelBufferPainter.h
--rw-r--r--   0 runner    (1001) docker     (127)    15287 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)    26409 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPlugin.h
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPluginConfigPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layPluginConfigPage.h
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layProperties.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layProperties.h
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawLayerInfo.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawLayerInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThread.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThread.h
--rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadCanvas.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadCanvas.h
--rw-r--r--   0 runner    (1001) docker     (127)    79863 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadWorker.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadWorker.h
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRenderer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRenderer.h
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRubberBox.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layRubberBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laySelector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laySelector.h
--rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laySnap.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laySnap.h
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layStipplePalette.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layStipplePalette.h
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layStream.h
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layTextInfo.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layTextInfo.h
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)    35586 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewOp.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewOp.h
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewport.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layViewport.h
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layZoomBox.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/layZoomBox.h
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laybasicCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laybasicConfig.h
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laybasicForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-01 08:11:15.000000 klayout-0.29.0/src/laybasic/laybasic/laybasicForceLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/layview/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.954328 klayout-0.29.0/src/layview/layview/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/gsiDeclLayAdditional.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/gsiDeclLayLayoutView_noqt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/gsiDeclLayLayoutView_qt.cc
--rw-r--r--   0 runner    (1001) docker     (127)    19453 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layGridNet.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layGridNet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layGridNetConfigPage.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layGridNetConfigPage.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layLayoutView.h
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layLayoutView_noqt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layLayoutView_noqt.h
--rw-r--r--   0 runner    (1001) docker     (127)    42468 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layLayoutView_qt.cc
--rw-r--r--   0 runner    (1001) docker     (127)    24045 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layLayoutView_qt.h
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layviewCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layviewForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-01 08:11:15.000000 klayout-0.29.0/src/layview/layview/layviewForceLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.958329 klayout-0.29.0/src/lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasic.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicArc.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicArc.h
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicCircle.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicCircle.h
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicDonut.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicDonut.h
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicEllipse.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicEllipse.h
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicPie.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicPie.h
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicRoundPath.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicRoundPath.h
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicRoundPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicRoundPolygon.h
--rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicStrokedPolygon.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicStrokedPolygon.h
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicText.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libBasicText.h
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lib/lib/libForceLink.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/lym/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.958329 klayout-0.29.0/src/lym/lym/
--rw-r--r--   0 runner    (1001) docker     (127)    32338 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/gsiDeclLymMacro.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    28214 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacro.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacro.h
--rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacroCollection.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacroCollection.h
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacroInterpreter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-01 08:11:15.000000 klayout-0.29.0/src/lym/lym/lymMacroInterpreter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.958329 klayout-0.29.0/src/plugins/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/common/dbPluginCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/common/layPluginCommon.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/cif/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.962329 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIF.h
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFFormat.h
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    15953 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/cif/db_plugin/gsiDeclDbCIF.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/dxf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.962329 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXF.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXF.h
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFFormat.h
--rw-r--r--   0 runner    (1001) docker     (127)    92554 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.h
--rwxr-xr-x   0 runner    (1001) docker     (127)    16271 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/gsiDeclDbDXF.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/gds2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.966328 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.966328 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Text.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.h
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2.h
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Format.h
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.h
--rw-r--r--   0 runner    (1001) docker     (127)    33109 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.h
--rw-r--r--   0 runner    (1001) docker     (127)    27284 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.h
--rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/gsiDeclDbGDS2.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/lefdef/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.966328 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    54398 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.h
--rw-r--r--   0 runner    (1001) docker     (127)    70571 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.cc
--rw-r--r--   0 runner    (1001) docker     (127)    43665 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.h
--rw-r--r--   0 runner    (1001) docker     (127)    19482 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)    30038 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.h
--rw-r--r--   0 runner    (1001) docker     (127)    56804 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/gsiDeclDbLEFDEF.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/magic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.970328 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAG.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAG.h
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGFormat.h
--rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/magic/db_plugin/gsiDeclDbMAG.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/oasis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.970328 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASIS.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASIS.h
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISFormat.h
--rw-r--r--   0 runner    (1001) docker     (127)   102666 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    97148 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/gsiDeclDbOASIS.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/streamers/pcb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.974329 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.h
--rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.h
--rw-r--r--   0 runner    (1001) docker     (127)    31886 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.h
--rw-r--r--   0 runner    (1001) docker     (127)    26606 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.h
--rw-r--r--   0 runner    (1001) docker     (127)    28043 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.814328 klayout-0.29.0/src/plugins/tools/net_tracer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.974329 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    47664 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.h
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.h
--rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerPlugin.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-04-01 08:11:15.000000 klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/gsiDeclDbNetTracer.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.818328 klayout-0.29.0/src/pya/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.978329 klayout-0.29.0/src/pya/pya/
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/gsiDeclPya.cc
--rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pya.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pya.h
--rw-r--r--   0 runner    (1001) docker     (127)   180315 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaCallables.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaCallables.h
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)    18109 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaConvert.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17750 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaConvert.h
--rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaHelpers.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaHelpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaInspector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaInspector.h
--rw-r--r--   0 runner    (1001) docker     (127)    26593 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaInternal.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaInternal.h
--rw-r--r--   0 runner    (1001) docker     (127)    37121 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaMarshal.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaMarshal.h
--rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaModule.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaModule.h
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaObject.h
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaRefs.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaRefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaSignalHandler.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaSignalHandler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaStatusChangedListener.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaStatusChangedListener.h
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pya/pya/pyaUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.978329 klayout-0.29.0/src/pymod/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtCore/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtCore/QtCoreMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtCore/QtCoreMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtCore5Compat/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtCore5Compat/QtCore5CompatMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtCore5Compat/QtCore5CompatMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtDesigner/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtDesigner/QtDesignerMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtDesigner/QtDesignerMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtGui/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtGui/QtGuiMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtGui/QtGuiMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtMultimedia/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtMultimedia/QtMultimediaMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtMultimedia/QtMultimediaMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtNetwork/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtNetwork/QtNetworkMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtNetwork/QtNetworkMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtPrintSupport/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtPrintSupport/QtPrintSupportMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtPrintSupport/QtPrintSupportMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtSql/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtSql/QtSqlMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtSql/QtSqlMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtSvg/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtSvg/QtSvgMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtSvg/QtSvgMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtUiTools/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtUiTools/QtUiToolsMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtUiTools/QtUiToolsMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.982329 klayout-0.29.0/src/pymod/QtWidgets/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtWidgets/QtWidgetsMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtWidgets/QtWidgetsMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.986328 klayout-0.29.0/src/pymod/QtXml/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtXml/QtXmlMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtXml/QtXmlMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.986328 klayout-0.29.0/src/pymod/QtXmlPatterns/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtXmlPatterns/QtXmlPatternsMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/QtXmlPatterns/QtXmlPatternsMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.986328 klayout-0.29.0/src/pymod/ant/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/ant/antMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/ant/antMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.986328 klayout-0.29.0/src/pymod/bridge_sample/
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/bridge_sample/bridge_sample.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.986328 klayout-0.29.0/src/pymod/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/db/dbMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/db/dbMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.818328 klayout-0.29.0/src/pymod/distutils_src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.990329 klayout-0.29.0/src/pymod/distutils_src/klayout/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.990329 klayout-0.29.0/src/pymod/distutils_src/klayout/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/db/pcell_declaration_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)  2687692 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/dbcore.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.990329 klayout-0.29.0/src/pymod/distutils_src/klayout/lay/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/lay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   422246 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/laycore.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.990329 klayout-0.29.0/src/pymod/distutils_src/klayout/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/libcore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/distutils_src/klayout/pya/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/pya/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/distutils_src/klayout/rdb/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/rdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71888 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/rdbcore.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/distutils_src/klayout/tl/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/tl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   119798 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/klayout/tlcore.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:21.022328 klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 08:11:20.000000 klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32235 2024-04-01 08:11:20.000000 klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:11:20.000000 klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 08:11:20.000000 klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/distutils_src/pya/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/distutils_src/pya/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/edt/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/edt/edtMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/edt/edtMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/img/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/img/imgMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/img/imgMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/lay/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lay/layMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lay/layMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lib/libMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lib/libMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/lym/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lym/lymMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/lym/lymMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/pya/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/pya/pyaMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/pymodHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/rdb/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/rdb/rdbMain.cc
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/rdb/rdbMain.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/tl/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/tl/tlMain.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/pymod/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-01 08:11:15.000000 klayout-0.29.0/src/pymod/unit_tests/pymod_tests.cc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.994329 klayout-0.29.0/src/rbastub/
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rbastub/rba.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rbastub/rba.h
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rbastub/rbaCommon.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.822328 klayout-0.29.0/src/rdb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.998329 klayout-0.29.0/src/rdb/rdb/
--rw-r--r--   0 runner    (1001) docker     (127)    73206 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/gsiDeclRdb.cc
--rw-r--r--   0 runner    (1001) docker     (127)    43514 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdb.cc
--rw-r--r--   0 runner    (1001) docker     (127)    50963 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdb.h
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbFile.cc
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbForceLink.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbForceLink.h
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbRVEReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbReader.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbReader.h
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbTiledRdbOutputReceiver.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbTiledRdbOutputReceiver.h
--rw-r--r--   0 runner    (1001) docker     (127)    16217 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-01 08:11:15.000000 klayout-0.29.0/src/rdb/rdb/rdbUtils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:20.822328 klayout-0.29.0/src/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:21.022328 klayout-0.29.0/src/tl/tl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:21.022328 klayout-0.29.0/src/tl/tl/atomic/
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/atomic/atomic.h
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/atomic/atomic_msvc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/atomic/spinlock.h
--rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlAlgorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlArch.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlArch.h
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlAssert.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlAssert.h
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlBase64.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlBase64.h
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlClassRegistry.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlClassRegistry.h
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlColor.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlColor.h
--rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCommandLineParser.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCommandLineParser.h
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCommon.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCopyOnWrite.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCopyOnWrite.h
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlCpp.h
--rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDataMapping.cc
--rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDataMapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeferredExecution.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeferredExecution.h
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeferredExecutionQt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeferredExecutionQt.h
--rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeflate.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDeflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlDefs.h
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEnv.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEnv.h
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEquivalenceClusters.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEquivalenceClusters.h
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEvents.cc
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEvents.h
--rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlEventsVar.h
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlException.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlException.h
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlExceptions.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlExceptions.h
--rw-r--r--   0 runner    (1001) docker     (127)   106291 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlExpression.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlExpression.h
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlFileSystemWatcher.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlFileSystemWatcher.h
--rw-r--r--   0 runner    (1001) docker     (127)    26717 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlFileUtils.cc
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlFileUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlFixedVector.h
--rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlGit.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlGit.h
--rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlGlobPattern.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlGlobPattern.h
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHeap.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStream.h
--rw-r--r--   0 runner    (1001) docker     (127)    34199 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStreamCurl.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStreamCurl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStreamNoQt.cc
--rw-r--r--   0 runner    (1001) docker     (127)    14889 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStreamQt.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlHttpStreamQt.h
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInclude.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInclude.h
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInt128Support.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInt128Support.h
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInternational.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlInternational.h
--rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlIntervalMap.h
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlIntervalSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlIteratorUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    14640 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlKDTree.h
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlList.cc
--rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlList.h
--rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlLog.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlLog.h
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlLongInt.cc
--rw-r--r--   0 runner    (1001) docker     (127)    27167 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlLongInt.h
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlMath.h
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlObject.cc
--rw-r--r--   0 runner    (1001) docker     (127)    10080 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlObject.h
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlObjectCollection.h
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlOptional.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlOptional.h
--rw-r--r--   0 runner    (1001) docker     (127)    24246 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlPixelBuffer.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlPixelBuffer.h
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlProgress.cc
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlProgress.h
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlRecipe.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlRecipe.h
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlResources.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlResources.h
--rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlReuseVector.h
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlSList.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlSList.h
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlScriptError.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlScriptError.h
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlSelect.h
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlSleep.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlSleep.h
--rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStableVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStaticObjects.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStaticObjects.h
--rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStream.cc
--rw-r--r--   0 runner    (1001) docker     (127)    31139 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStream.h
--rw-r--r--   0 runner    (1001) docker     (127)    40394 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlString.cc
--rw-r--r--   0 runner    (1001) docker     (127)    28075 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlString.h
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlStringEx.h
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlThreadedWorkers.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlThreadedWorkers.h
--rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlThreads.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlThreads.h
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlTimer.cc
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlTimer.h
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlTypeTraits.h
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUniqueId.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUniqueId.h
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUniqueName.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUniqueName.h
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUnitTest.cc
--rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUnitTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUri.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUri.h
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlUtils.h
--rw-r--r--   0 runner    (1001) docker     (127)    76537 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlVariant.cc
--rw-r--r--   0 runner    (1001) docker     (127)    43587 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlVariant.h
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlVariantUserClasses.h
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlVector.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlWebDAV.cc
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlWebDAV.h
--rw-r--r--   0 runner    (1001) docker     (127)    23993 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlXMLParser.cc
--rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlXMLParser.h
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlXMLWriter.cc
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/tlXMLWriter.h
--rw-r--r--   0 runner    (1001) docker     (127)   213994 2024-04-01 08:11:15.000000 klayout-0.29.0/src/tl/tl/utf_casefolding.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:11:21.022328 klayout-0.29.0/src/version/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-01 08:11:15.000000 klayout-0.29.0/src/version/version.h
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-01 08:11:16.000000 klayout-0.29.0/version.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.580468 klayout-0.29.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-04 16:37:17.000000 klayout-0.29.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-04 16:37:17.000000 klayout-0.29.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 16:37:22.580468 klayout-0.29.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-04 16:37:17.000000 klayout-0.29.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-04 16:37:18.000000 klayout-0.29.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:37:22.580468 klayout-0.29.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    36792 2024-05-04 16:37:18.000000 klayout-0.29.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.372466 klayout-0.29.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/ant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.376466 klayout-0.29.1/src/ant/ant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antConfig.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14004 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antConfigPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antConfigPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23487 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19423 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antPlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16650 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antPropertiesPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antPropertiesPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    83683 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15991 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antService.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antTemplate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/antTemplate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56210 2024-05-04 16:37:18.000000 klayout-0.29.1/src/ant/ant/gsiDeclAnt.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/db/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.448467 klayout-0.29.1/src/db/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbArray.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    78404 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbArray.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31463 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8511 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59769 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbAsIfFlatTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBox.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    34694 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBoxConvert.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16406 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBoxConvert.h
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBoxScanner.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    37098 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBoxScanner.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57744 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbBoxTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29399 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCell.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCell.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellGraphUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellGraphUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellHullGenerator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellHullGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellInst.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellInst.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11602 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellMapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellVariants.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12139 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCellVariants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29563 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCircuit.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCircuit.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22620 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClip.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClip.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClipboard.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClipboard.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClipboardData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbClipboardData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbColdProxy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbColdProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCommonReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCommonReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCompoundOperation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   104566 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbCompoundOperation.h
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbConverters.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbConverters.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15785 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59720 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)    83561 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    43430 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepShapeStore.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28569 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepShapeStore.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22077 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeepTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDevice.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDevice.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeviceAbstract.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeviceAbstract.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeviceClass.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23269 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbDeviceClass.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdge.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    39777 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdge.h
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgeBoolean.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16847 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgeBoolean.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePair.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePair.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairFilters.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairFilters.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14247 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairRelations.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairRelations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16225 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairsDelegate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgePairsDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    80400 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgeProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    37357 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgeProcessor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    45249 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesDelegate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11849 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesLocalOperations.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesLocalOperations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesToContours.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesToContours.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13332 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEdgesUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10378 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbEmptyTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16149 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFillTool.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFillTool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13294 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFlatTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFuzzyCellMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbFuzzyCellMapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbGenericShapeIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15368 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbGenericShapeIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbGlyphs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbGlyphs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17209 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHershey.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHershey.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHersheyFont.h
+-rw-r--r--   0 runner    (1001) docker     (127)   107885 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierNetworkProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    48327 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierNetworkProcessor.h
+-rw-r--r--   0 runner    (1001) docker     (127)   105181 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18383 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierProcessor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33168 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierarchyBuilder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18902 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbHierarchyBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInit.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInit.h
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInstElement.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInstElement.h
+-rw-r--r--   0 runner    (1001) docker     (127)    55675 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInstances.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    59367 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbInstances.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13637 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayerMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayerMapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayerProperties.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayerProperties.h
+-rw-r--r--   0 runner    (1001) docker     (127)    87383 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayout.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    67229 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayout.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutContextHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutContextHandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59320 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutDiff.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10045 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutDiff.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutLayers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutLayers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    93559 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutQuery.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutQuery.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutStateModel.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutStateModel.h
+-rw-r--r--   0 runner    (1001) docker     (127)    75266 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlist.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    46904 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistEnums.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistFormatDefs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistFormatDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35362 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistSoftConnections.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistSoftConnections.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31028 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutToNetlistWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24155 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematic.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicFormatDefs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicFormatDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLayoutVsSchematicWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibrary.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibrary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibraryManager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibraryManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibraryProxy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLibraryProxy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLoadLayoutOptions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLoadLayoutOptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLocalOperation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLocalOperation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLocalOperationUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLocalOperationUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLog.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbManager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbManager.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27854 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28996 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMemStatistics.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMemStatistics.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMetaInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbMutableTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNamedLayerReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNamedLayerReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetShape.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30142 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlist.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlist.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70642 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompare.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14759 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompare.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57796 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareCore.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareCore.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20738 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareGraph.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11928 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareGraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCompareUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20426 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCrossReference.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11915 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistCrossReference.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceClasses.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceClasses.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24177 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceExtractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceExtractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35073 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceExtractorClasses.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13975 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistDeviceExtractorClasses.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistExtractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistExtractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34044 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21100 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReaderDelegate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReaderDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReaderExpressionParser.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceReaderExpressionParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistSpiceWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbNetlistWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbObjectTag.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbObjectWithProperties.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerEdgePairs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerEdges.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12357 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbOriginalLayerTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellDeclaration.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21064 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellDeclaration.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellHeader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellHeader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellVariant.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPCellVariant.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19796 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    29202 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPin.h
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPoint.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15642 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    97025 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29218 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygonGenerators.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygonGenerators.h
+-rw-r--r--   0 runner    (1001) docker     (127)    84353 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygonTools.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26980 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPolygonTools.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPropertiesRepository.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPropertiesRepository.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbPropertyConstraint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19122 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRecursiveInstanceIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21248 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRecursiveInstanceIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30225 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRecursiveShapeIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    33107 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRecursiveShapeIterator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20718 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    62283 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegion.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19768 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionCheckUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionCheckUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionDelegate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (127)    73054 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionLocalOperations.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionLocalOperations.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionProcessors.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15144 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionProcessors.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12693 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbRegionUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbSaveLayoutOptions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12424 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbSaveLayoutOptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27601 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShape.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    88056 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShape.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeCollection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeCollection.h
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeCollectionUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeCollectionUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeFlags.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeFlags.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29509 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15853 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31002 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeProcessor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11428 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapeRepository.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60032 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    64769 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40124 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapes2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapes2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47851 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbShapes3.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStatic.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStatic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7754 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStreamLayers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbStreamLayers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbSubCircuit.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbSubCircuit.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13800 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTechnology.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21358 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTechnology.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTestSupport.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTestSupport.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbText.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbText.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15866 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTexts.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextsDelegate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextsDelegate.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextsUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTextsUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27699 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTilingProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTilingProcessor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTrans.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    62716 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTrans.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTriangle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTriangle.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47748 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTriangles.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11567 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTriangles.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbUserObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbUserObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9696 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8546 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbVariableWidthPath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbVariableWidthPath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbVector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbWriterTools.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/dbWriterTools.h
+-rw-r--r--   0 runner    (1001) docker     (127)   325050 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/fonts.cc_gen
+-rw-r--r--   0 runner    (1001) docker     (127)   184001 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/glyphs.cc_gen
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbBox.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   206678 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbCell.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24674 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbCellMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbCommonStreamOptions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    61961 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbCompoundOperation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18336 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbContainerHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13786 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbDeepShapeStore.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27090 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbEdge.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbEdgePair.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    58648 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbEdgePairs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31684 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbEdgeProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   116738 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbEdges.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbGlyphs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbHierNetworkProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbInstElement.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayerMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   131530 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayout.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    37095 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayoutDiff.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayoutQuery.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    55810 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayoutToNetlist.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayoutUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLayoutVsSchematic.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    42937 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLibrary.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbLog.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbManager.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbMatrix.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbMetaInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbMetaInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)   141898 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbNetlist.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    34214 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbNetlistCompare.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22473 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbNetlistCrossReference.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbNetlistDeviceClasses.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbNetlistDeviceExtractor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17652 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbPath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbPoint.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    80774 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    29328 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbRecursiveInstanceIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    39585 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbRecursiveShapeIterator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   216123 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbRegion.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    79509 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbShape.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbShapeCollection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24866 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbShapeProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    69049 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbShapes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbTechnologies.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18118 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbText.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31749 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbTexts.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    40313 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbTilingProcessor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    65198 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbTrans.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-05-04 16:37:18.000000 klayout-0.29.1/src/db/db/gsiDeclDbVector.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/edt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.456467 klayout-0.29.1/src/edt/edt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtConfig.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20396 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtDialogs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtDialogs.h
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtDistribute.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtDistribute.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtEditorHooks.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtEditorHooks.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29492 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtEditorOptionsPages.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtEditorOptionsPages.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34028 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtInstPropertiesPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtInstPropertiesPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    88614 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtMainService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtMainService.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtMoveTrackerService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtMoveTrackerService.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32548 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPCellParametersPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPCellParametersPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)   107225 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPartialService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPartialService.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27705 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27342 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPropertiesPageUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPropertiesPageUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41126 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPropertiesPages.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtPropertiesPages.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtRecentConfigurationPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtRecentConfigurationPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56070 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18756 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtService.h
+-rw-r--r--   0 runner    (1001) docker     (127)    62057 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtServiceImpl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtServiceImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/edtUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/gsiDeclEdt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-05-04 16:37:18.000000 klayout-0.29.1/src/edt/edt/gsiDeclEdtEditorHooks.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/gsi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.464467 klayout-0.29.1/src/gsi/gsi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsi.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiCallback.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiCallbackVar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiClass.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21744 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiClass.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28804 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiClassBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17462 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiClassBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDecl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDeclBasic.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDeclBasic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12510 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDeclInternal.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27525 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDeclTl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiDeclTlPixelBuffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18009 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiEnums.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28194 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiExpression.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiExpression.h
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiExternalMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiExternalMain.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiInspector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiInspector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiInterpreter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiInterpreter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiIterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiMethods.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    66731 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiMethods.h
+-rw-r--r--   0 runner    (1001) docker     (127)    63912 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiMethodsVar.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiObjectHolder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiObjectHolder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiSerialisation.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    55924 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiSerialisation.h
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiSignals.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    37277 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiSignals.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiTypes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    85918 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiTypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26550 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiVariantArgs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-04 16:37:18.000000 klayout-0.29.1/src/gsi/gsi/gsiVariantArgs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/img/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.468467 klayout-0.29.1/src/img/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    57201 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/gsiDeclImg.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgLandmarksDialog.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgLandmarksDialog.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgNavigator.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgNavigator.h
+-rw-r--r--   0 runner    (1001) docker     (127)    60689 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgPlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28049 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgPropertiesPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgPropertiesPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)    49601 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgService.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13742 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgService.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13158 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgWidgets.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-04 16:37:18.000000 klayout-0.29.1/src/img/img/imgWidgets.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/laybasic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.504467 klayout-0.29.1/src/laybasic/laybasic/
+-rw-r--r--   0 runner    (1001) docker     (127) 11156282 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/fixedFont.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56822 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayLayers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   125663 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayLayoutViewBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayMarker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22093 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayMenu.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    52738 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayRdbAdded.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayTlAdded.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    53092 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gtf.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gtf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/gtfdummy.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    47760 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layAbstractMenu.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26533 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layAbstractMenu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layAnnotationShapes.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9552 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layAnnotationShapes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21413 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8448 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmapRenderer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12648 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmapRenderer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29934 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmapsToImage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBitmapsToImage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBookmarkList.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layBookmarkList.h
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCanvasPlane.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCanvasPlane.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCellView.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCellView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layColorPalette.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layColorPalette.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layConverters.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layConverters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCursor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layCursor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDispatcher.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDispatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDisplayState.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDisplayState.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDitherPattern.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDitherPattern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDragDropData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDragDropData.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDrawing.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layDrawing.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17558 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layEditable.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layEditable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layEditorServiceBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layEditorServiceBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29779 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layFinder.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layFinder.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layFixedFont.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layFixedFont.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59139 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayerProperties.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    49544 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayerProperties.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30362 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayoutCanvas.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11551 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayoutCanvas.h
+-rw-r--r--   0 runner    (1001) docker     (127)   160373 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayoutViewBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    81866 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayoutViewBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLayoutViewConfig.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLineStylePalette.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLineStylePalette.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLineStyles.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layLineStyles.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMargin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMargin.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35685 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMarker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21239 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMarker.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMouseTracker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMouseTracker.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMove.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layMove.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layNativePlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layNativePlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layNetColorizer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layNetColorizer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layObjectInstPath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layObjectInstPath.h
+-rw-r--r--   0 runner    (1001) docker     (127)    41689 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layParsedLayerSource.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21724 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layParsedLayerSource.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPixelBufferPainter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPixelBufferPainter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15287 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    26409 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPlugin.h
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPluginConfigPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layPluginConfigPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layProperties.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layProperties.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawLayerInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawLayerInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThread.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThread.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadCanvas.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadCanvas.h
+-rw-r--r--   0 runner    (1001) docker     (127)    79863 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadWorker.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadWorker.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRenderer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRenderer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRubberBox.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layRubberBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laySelector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laySelector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laySnap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laySnap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layStipplePalette.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layStipplePalette.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layTextInfo.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layTextInfo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    35586 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewOp.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewOp.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewport.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layViewport.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layZoomBox.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/layZoomBox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laybasicCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laybasicConfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laybasicForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-04 16:37:18.000000 klayout-0.29.1/src/laybasic/laybasic/laybasicForceLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/layview/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.508467 klayout-0.29.1/src/layview/layview/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/gsiDeclLayAdditional.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/gsiDeclLayLayoutView_noqt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/gsiDeclLayLayoutView_qt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    19453 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layGridNet.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layGridNet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layGridNetConfigPage.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layGridNetConfigPage.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layLayoutView.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layLayoutView_noqt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layLayoutView_noqt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    42468 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layLayoutView_qt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24045 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layLayoutView_qt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layviewCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layviewForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-04 16:37:18.000000 klayout-0.29.1/src/layview/layview/layviewForceLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.512467 klayout-0.29.1/src/lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasic.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicArc.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicArc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicCircle.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicCircle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicDonut.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicDonut.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicEllipse.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicEllipse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicPie.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicPie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicRoundPath.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicRoundPath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicRoundPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicRoundPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicStrokedPolygon.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicStrokedPolygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicText.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libBasicText.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lib/lib/libForceLink.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.364466 klayout-0.29.1/src/lym/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.512467 klayout-0.29.1/src/lym/lym/
+-rw-r--r--   0 runner    (1001) docker     (127)    32338 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/gsiDeclLymMacro.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28214 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacro.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacro.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25237 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacroCollection.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacroCollection.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacroInterpreter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-04 16:37:18.000000 klayout-0.29.1/src/lym/lym/lymMacroInterpreter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.512467 klayout-0.29.1/src/plugins/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/common/dbPluginCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/common/layPluginCommon.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/cif/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.512467 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFFormat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15953 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/cif/db_plugin/gsiDeclDbCIF.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/dxf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.516467 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXF.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXF.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFFormat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    92554 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.h
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16271 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/gsiDeclDbDXF.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/gds2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.516467 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.520467 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Text.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Format.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33109 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27284 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15133 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/gsiDeclDbGDS2.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/lefdef/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.520467 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    54398 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70571 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    43665 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19482 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    30038 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56804 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/gsiDeclDbLEFDEF.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/magic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.520467 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAG.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAG.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGFormat.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18082 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/magic/db_plugin/gsiDeclDbMAG.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/oasis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.524468 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASIS.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASIS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISFormat.h
+-rw-r--r--   0 runner    (1001) docker     (127)   102666 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    97148 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9787 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12270 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/gsiDeclDbOASIS.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/streamers/pcb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.524468 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16896 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31886 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23739 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26606 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28043 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/plugins/tools/net_tracer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.528468 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    47664 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    21333 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerPlugin.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    22637 2024-05-04 16:37:18.000000 klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/gsiDeclDbNetTracer.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.368466 klayout-0.29.1/src/pya/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.532467 klayout-0.29.1/src/pya/pya/
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/gsiDeclPya.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    24129 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pya.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pya.h
+-rw-r--r--   0 runner    (1001) docker     (127)   180315 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaCallables.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaCallables.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18109 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaConvert.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17750 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaConvert.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18501 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaHelpers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaHelpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaInspector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaInspector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26593 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaInternal.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaInternal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37121 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaMarshal.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaMarshal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24705 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaModule.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaModule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaRefs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaRefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaSignalHandler.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaSignalHandler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaStatusChangedListener.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaStatusChangedListener.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pya/pya/pyaUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.532467 klayout-0.29.1/src/pymod/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.532467 klayout-0.29.1/src/pymod/QtCore/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtCore/QtCoreMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtCore/QtCoreMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.532467 klayout-0.29.1/src/pymod/QtCore5Compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtCore5Compat/QtCore5CompatMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtCore5Compat/QtCore5CompatMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.532467 klayout-0.29.1/src/pymod/QtDesigner/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtDesigner/QtDesignerMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtDesigner/QtDesignerMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtGui/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtGui/QtGuiMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtGui/QtGuiMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtMultimedia/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtMultimedia/QtMultimediaMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtMultimedia/QtMultimediaMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtNetwork/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtNetwork/QtNetworkMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtNetwork/QtNetworkMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtPrintSupport/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtPrintSupport/QtPrintSupportMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtPrintSupport/QtPrintSupportMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtSql/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtSql/QtSqlMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtSql/QtSqlMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtSvg/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtSvg/QtSvgMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtSvg/QtSvgMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtUiTools/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtUiTools/QtUiToolsMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtUiTools/QtUiToolsMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtWidgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtWidgets/QtWidgetsMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtWidgets/QtWidgetsMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtXml/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtXml/QtXmlMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtXml/QtXmlMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/QtXmlPatterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtXmlPatterns/QtXmlPatternsMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/QtXmlPatterns/QtXmlPatternsMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/ant/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/ant/antMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/ant/antMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.536468 klayout-0.29.1/src/pymod/bridge_sample/
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/bridge_sample/bridge_sample.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.540468 klayout-0.29.1/src/pymod/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/db/dbMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/db/dbMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.372466 klayout-0.29.1/src/pymod/distutils_src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/db/pcell_declaration_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2703403 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/dbcore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/lay/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/lay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   432376 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/laycore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/libcore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/pya/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/pya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/rdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/rdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80422 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/rdbcore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/klayout/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/tl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119798 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/klayout/tlcore.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.580468 klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-04 16:37:22.000000 klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32404 2024-05-04 16:37:22.000000 klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:37:22.000000 klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 16:37:22.000000 klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.544468 klayout-0.29.1/src/pymod/distutils_src/pya/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/distutils_src/pya/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/edt/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/edt/edtMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/edt/edtMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/img/imgMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/img/imgMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/lay/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lay/layMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lay/layMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lib/libMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lib/libMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/lym/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lym/lymMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/lym/lymMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/pya/
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/pya/pyaMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/pymodHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/rdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/rdb/rdbMain.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/rdb/rdbMain.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/tl/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/tl/tlMain.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/pymod/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-04 16:37:18.000000 klayout-0.29.1/src/pymod/unit_tests/pymod_tests.cc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.548468 klayout-0.29.1/src/rbastub/
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rbastub/rba.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rbastub/rba.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rbastub/rbaCommon.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.372466 klayout-0.29.1/src/rdb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.552468 klayout-0.29.1/src/rdb/rdb/
+-rw-r--r--   0 runner    (1001) docker     (127)    76206 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/gsiDeclRdb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    51983 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdb.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    53204 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdb.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8240 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbFile.cc
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbForceLink.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbForceLink.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbRVEReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbReader.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbReader.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbTiledRdbOutputReceiver.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbTiledRdbOutputReceiver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-05-04 16:37:18.000000 klayout-0.29.1/src/rdb/rdb/rdbUtils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.372466 klayout-0.29.1/src/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.576468 klayout-0.29.1/src/tl/tl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.576468 klayout-0.29.1/src/tl/tl/atomic/
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/atomic/atomic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/atomic/atomic_msvc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/atomic/spinlock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19875 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlAlgorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlArch.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlArch.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlAssert.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlAssert.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlBase64.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlBase64.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlClassRegistry.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlClassRegistry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlColor.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlColor.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCommandLineParser.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCommandLineParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCommon.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCopyOnWrite.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCopyOnWrite.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlCpp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11955 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDataMapping.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     9596 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDataMapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeferredExecution.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeferredExecution.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeferredExecutionQt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeferredExecutionQt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14361 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeflate.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDeflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlDefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEnv.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEnv.h
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEquivalenceClusters.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEquivalenceClusters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEvents.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEvents.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10899 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlEventsVar.h
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlException.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlExceptions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlExceptions.h
+-rw-r--r--   0 runner    (1001) docker     (127)   107571 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlExpression.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15243 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlExpression.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlFileSystemWatcher.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlFileSystemWatcher.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26717 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlFileUtils.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlFileUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlFixedVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12332 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlGit.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlGit.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlGlobPattern.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlGlobPattern.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHeap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34199 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStreamCurl.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStreamCurl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStreamNoQt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15072 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStreamQt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlHttpStreamQt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInclude.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInclude.h
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInt128Support.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInt128Support.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInternational.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlInternational.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9680 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlIntervalMap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlIntervalSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlIteratorUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14640 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlKDTree.h
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlList.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    11402 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9027 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlLog.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlLog.h
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlLongInt.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    27167 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlLongInt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlMath.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlObject.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    10080 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlObject.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlObjectCollection.h
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlOptional.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlOptional.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24246 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlPixelBuffer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlPixelBuffer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlProgress.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlProgress.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlRecipe.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlRecipe.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlResources.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlResources.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlReuseVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlSList.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlSList.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlScriptError.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlScriptError.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlSelect.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlSleep.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlSleep.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16140 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStableVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStaticObjects.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStaticObjects.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStream.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31139 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    40394 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlString.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    28075 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlString.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlStringEx.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlThreadedWorkers.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlThreadedWorkers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlThreads.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlThreads.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlTimer.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlTimer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlTypeTraits.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUniqueId.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUniqueId.h
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUniqueName.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUniqueName.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUnitTest.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    15666 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUnitTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUri.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUri.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlUtils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    76537 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlVariant.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    43587 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlVariant.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlVariantUserClasses.h
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlVector.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlWebDAV.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlWebDAV.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23993 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlXMLParser.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    60989 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlXMLParser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlXMLWriter.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/tlXMLWriter.h
+-rw-r--r--   0 runner    (1001) docker     (127)   213994 2024-05-04 16:37:18.000000 klayout-0.29.1/src/tl/tl/utf_casefolding.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:37:22.576468 klayout-0.29.1/src/version/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-04 16:37:18.000000 klayout-0.29.1/src/version/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-04 16:37:18.000000 klayout-0.29.1/version.sh
```

### Comparing `klayout-0.29.0/LICENSE` & `klayout-0.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/MANIFEST.in` & `klayout-0.29.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/PKG-INFO` & `klayout-0.29.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klayout
-Version: 0.29.0
+Version: 0.29.1
 Summary: KLayout standalone Python package
 Home-page: https://github.com/klayout/klayout
 Author: Matthias Koefferlein
 Author-email: matthias@klayout.de
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klayout-0.29.0/README.md` & `klayout-0.29.1/README.md`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/pyproject.toml` & `klayout-0.29.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,37 +7,22 @@
   "python {package}/testdata/pymod/import_lib.py",
   "python {package}/testdata/pymod/import_lay.py",
   "TESTSRC={package} python {package}/testdata/pymod/pya_tests.py"
 ]
 # Disable building PyPy wheels on all platforms
 skip = "pp*"
 
-# Skip trying to test arm64 builds on Intel Macs
-test-skip = "*-macosx_arm64 *-macosx_universal2:arm64"
-
 [tool.cibuildwheel.linux]
 # beware: the before-all script does not persist environment variables!
 # No point in defining $PATH or $CCACHE_DIR
 before-all = "source {project}/ci-scripts/docker/docker_prepare.sh"
 archs = ["auto64"]
 # Append a directory to the PATH variable (this is expanded in the build environment)
 environment = { PATH="/usr/lib/ccache:/usr/lib64/ccache:/usr/lib/ccache/bin:$PATH" }
 before-build = "ccache -s"
 # Export a variable to docker
 # CCACHE_DIR="/home/runner/work/klayout/klayout/.ccache"
 environment-pass = ["HOST_CCACHE_DIR"]
 
 [tool.cibuildwheel.macos]
-before-all = [
-  "brew install libpng",
-  "brew deps --tree --installed",
-]
-
-# TEMP while Github Actions does not provide an Apple Silicon runner
-# TODO Simply remove it when it's available
-archs = ["x86_64", "arm64"]
-before-build = [
-  "ccache -s",
-  "bash {project}/ci-scripts/macos/libpng-patch.sh",
-]
 # Repair macOS wheels (include libpng with the wheel, for example)
-repair-wheel-command = "delocate-wheel --require-archs {delocate_archs} -w {dest_dir} -v --ignore-missing-dependencies {wheel}"
+repair-wheel-command = "delocate-wheel --require-archs {delocate_archs} -w {dest_dir} -v --ignore-missing-dependencies {wheel}"
```

### Comparing `klayout-0.29.0/setup.py` & `klayout-0.29.1/setup.py`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antCommon.h` & `klayout-0.29.1/src/ant/ant/antCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antConfig.cc` & `klayout-0.29.1/src/ant/ant/antConfig.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antConfig.h` & `klayout-0.29.1/src/ant/ant/antConfig.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antConfigPage.cc` & `klayout-0.29.1/src/ant/ant/antConfigPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antConfigPage.h` & `klayout-0.29.1/src/ant/ant/antConfigPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antForceLink.cc` & `klayout-0.29.1/src/ant/ant/antForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antForceLink.h` & `klayout-0.29.1/src/ant/ant/antForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antObject.cc` & `klayout-0.29.1/src/ant/ant/antObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antObject.h` & `klayout-0.29.1/src/ant/ant/antObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antPlugin.cc` & `klayout-0.29.1/src/ant/ant/antPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antPlugin.h` & `klayout-0.29.1/src/ant/ant/antPlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antPropertiesPage.cc` & `klayout-0.29.1/src/ant/ant/antPropertiesPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antPropertiesPage.h` & `klayout-0.29.1/src/ant/ant/antPropertiesPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antService.cc` & `klayout-0.29.1/src/ant/ant/antService.cc`

 * *Files 1% similar despite different names*

```diff
@@ -2194,21 +2194,35 @@
     for (lay::AnnotationShapes::iterator r = mp_view->annotation_shapes ().begin (); r != mp_view->annotation_shapes ().end (); ++r) {
       const ant::Object *robj = dynamic_cast <const ant::Object *> (r->ptr ());
       if (robj && robj->id () > idmax) {
         idmax = robj->id ();
       }
     }
 
+    std::vector<const db::DUserObject *> new_objects;
+
     for (db::Clipboard::iterator c = db::Clipboard::instance ().begin (); c != db::Clipboard::instance ().end (); ++c) {
       const db::ClipboardValue<ant::Object> *value = dynamic_cast<const db::ClipboardValue<ant::Object> *> (*c);
       if (value) {
         ant::Object *ruler = new ant::Object (value->get ());
         ruler->id (++idmax);
-        mp_view->annotation_shapes ().insert (db::DUserObject (ruler));
+        new_objects.push_back (&mp_view->annotation_shapes ().insert (db::DUserObject (ruler)));
+      }
+    }
+
+    //  make new objects selected
+
+    if (! new_objects.empty ()) {
+
+      for (auto r = new_objects.begin (); r != new_objects.end (); ++r) {
+        m_selected.insert (std::make_pair (mp_view->annotation_shapes ().iterator_from_pointer (*r), 0));
       }
+
+      selection_to_view ();
+
     }
 
   }
 
 }
 
 void
```

### Comparing `klayout-0.29.0/src/ant/ant/antService.h` & `klayout-0.29.1/src/ant/ant/antService.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antTemplate.cc` & `klayout-0.29.1/src/ant/ant/antTemplate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/antTemplate.h` & `klayout-0.29.1/src/ant/ant/antTemplate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/ant/ant/gsiDeclAnt.cc` & `klayout-0.29.1/src/ant/ant/gsiDeclAnt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbArray.cc` & `klayout-0.29.1/src/db/db/dbArray.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbArray.h` & `klayout-0.29.1/src/db/db/dbArray.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbAsIfFlatEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatEdgePairs.h` & `klayout-0.29.1/src/db/db/dbAsIfFlatEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatEdges.cc` & `klayout-0.29.1/src/db/db/dbAsIfFlatEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatEdges.h` & `klayout-0.29.1/src/db/db/dbAsIfFlatEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatRegion.cc` & `klayout-0.29.1/src/db/db/dbAsIfFlatRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatRegion.h` & `klayout-0.29.1/src/db/db/dbAsIfFlatRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatTexts.cc` & `klayout-0.29.1/src/db/db/dbAsIfFlatTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbAsIfFlatTexts.h` & `klayout-0.29.1/src/db/db/dbAsIfFlatTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBox.cc` & `klayout-0.29.1/src/db/db/dbBox.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBox.h` & `klayout-0.29.1/src/db/db/dbBox.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBoxConvert.cc` & `klayout-0.29.1/src/db/db/dbBoxConvert.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBoxConvert.h` & `klayout-0.29.1/src/db/db/dbBoxConvert.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBoxScanner.cc` & `klayout-0.29.1/src/db/db/dbBoxScanner.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBoxScanner.h` & `klayout-0.29.1/src/db/db/dbBoxScanner.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbBoxTree.h` & `klayout-0.29.1/src/db/db/dbBoxTree.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCell.cc` & `klayout-0.29.1/src/db/db/dbCell.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCell.h` & `klayout-0.29.1/src/db/db/dbCell.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellGraphUtils.cc` & `klayout-0.29.1/src/db/db/dbCellGraphUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellGraphUtils.h` & `klayout-0.29.1/src/db/db/dbCellGraphUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellHullGenerator.cc` & `klayout-0.29.1/src/db/db/dbCellHullGenerator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellHullGenerator.h` & `klayout-0.29.1/src/db/db/dbCellHullGenerator.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellInst.cc` & `klayout-0.29.1/src/db/db/dbCellInst.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellInst.h` & `klayout-0.29.1/src/db/db/dbCellInst.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellMapping.cc` & `klayout-0.29.1/src/db/db/dbCellMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellMapping.h` & `klayout-0.29.1/src/db/db/dbCellMapping.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCellVariants.cc` & `klayout-0.29.1/src/db/db/dbCellVariants.cc`

 * *Files 2% similar despite different names*

```diff
@@ -284,14 +284,15 @@
 
   //  create new cells for the variants
 
   std::map<db::cell_index_type, std::map<db::ICplxTrans, db::cell_index_type> > var_table_intern;
   if (! var_table) {
     var_table = &var_table_intern;
   }
+  tl_assert (var_table->empty ());
 
   for (db::Layout::bottom_up_const_iterator c = mp_layout->begin_bottom_up (); c != mp_layout->end_bottom_up (); ++c) {
 
     if (m_called.find (*c) == m_called.end ()) {
       continue;
     }
 
@@ -307,14 +308,17 @@
 
       for (db::Cell::const_iterator i = cell.begin (); ! i.at_end (); ++i) {
         inst.push_back (db::CellInstArrayWithProperties (i->cell_inst (), i->prop_id ()));
       }
 
       cell.clear_insts ();
 
+      bool original_cell_is_variant = false;
+      db::ICplxTrans original_cell_variant;
+
       int index = 0;
       for (auto v = vc->second.begin (); v != vc->second.end (); ++v, ++index) {
 
         db::cell_index_type ci_var;
 
         if (v != vc->second.begin ()) {
 
@@ -329,28 +333,32 @@
           //  a new entry for the variant
           if (! v->is_unity ()) {
             m_variants [ci_var].insert (*v);
           }
 
         } else {
           ci_var = *c;
+          original_cell_is_variant = true;
+          original_cell_variant = *v;
         }
 
         vt.insert (std::make_pair (*v, ci_var));
         create_var_instances (mp_layout->cell (ci_var), inst, *v, *var_table, mp_red->is_translation_invariant ());
 
       }
 
       //  correct the first (remaining) entry
-      if (! vt.begin ()->first.is_unity ()) {
-        std::set<db::ICplxTrans> &tv = m_variants [*c];
-        tv.clear ();
-        tv.insert (vt.begin ()->first);
-      } else {
-        m_variants.erase (*c);
+      if (original_cell_is_variant) {
+        if (! original_cell_variant.is_unity ()) {
+          std::set<db::ICplxTrans> &tv = m_variants [*c];
+          tv.clear ();
+          tv.insert (original_cell_variant);
+        } else {
+          m_variants.erase (*c);
+        }
       }
 
     } else {
 
       //  if the children of this cell are separated, map the instances to the new variants
       bool needs_update = false;
       for (db::Cell::child_cell_iterator cc = cell.begin_child_cells (); ! cc.at_end () && ! needs_update; ++cc) {
```

### Comparing `klayout-0.29.0/src/db/db/dbCellVariants.h` & `klayout-0.29.1/src/db/db/dbCellVariants.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCircuit.cc` & `klayout-0.29.1/src/db/db/dbCircuit.cc`

 * *Files 2% similar despite different names*

```diff
@@ -640,14 +640,19 @@
 {
   if (m_pin_refs.size () < pin_id + 1) {
     m_pin_refs.resize (pin_id + 1, Net::pin_iterator ());
   }
   m_pin_refs [pin_id] = iter;
 }
 
+bool Circuit::is_empty () const
+{
+  return m_nets.empty () && m_pins.empty () && m_devices.empty () && m_subcircuits.empty ();
+}
+
 void Circuit::blank ()
 {
   tl_assert (netlist () != 0);
 
   std::set<db::Circuit *> cs;
   for (subcircuit_iterator i = m_subcircuits.begin (); i != m_subcircuits.end (); ++i) {
     cs.insert (i->circuit_ref ());
```

### Comparing `klayout-0.29.0/src/db/db/dbCircuit.h` & `klayout-0.29.1/src/db/db/dbCircuit.h`

 * *Files 0% similar despite different names*

```diff
@@ -756,14 +756,19 @@
    *  and circuits which will itself are not longer be called after this.
    *  This operation will eventually leave a blackbox model of the circuit
    *  containing only pins.
    */
   void blank ();
 
   /**
+   *  @brief Gets a value indicating whether the circuit is empty
+   */
+  bool is_empty () const;
+
+  /**
    *  @brief Generate memory statistics
    */
   void mem_stat (MemStatistics *stat, MemStatistics::purpose_t purpose, int cat, bool no_self = false, void *parent = 0) const
   {
     if (! no_self) {
       stat->add (typeid (*this), (void *) this, sizeof (*this), sizeof (*this), parent, purpose, cat);
     }
```

### Comparing `klayout-0.29.0/src/db/db/dbClip.cc` & `klayout-0.29.1/src/db/db/dbClip.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbClip.h` & `klayout-0.29.1/src/db/db/dbClip.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbClipboard.cc` & `klayout-0.29.1/src/db/db/dbClipboard.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbClipboard.h` & `klayout-0.29.1/src/db/db/dbClipboard.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbClipboardData.cc` & `klayout-0.29.1/src/db/db/dbClipboardData.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbClipboardData.h` & `klayout-0.29.1/src/db/db/dbClipboardData.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbColdProxy.cc` & `klayout-0.29.1/src/db/db/dbColdProxy.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbColdProxy.h` & `klayout-0.29.1/src/db/db/dbColdProxy.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCommon.h` & `klayout-0.29.1/src/db/db/dbCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCommonReader.cc` & `klayout-0.29.1/src/db/db/dbCommonReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCommonReader.h` & `klayout-0.29.1/src/db/db/dbCommonReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCompoundOperation.cc` & `klayout-0.29.1/src/db/db/dbCompoundOperation.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbCompoundOperation.h` & `klayout-0.29.1/src/db/db/dbCompoundOperation.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbConverters.cc` & `klayout-0.29.1/src/db/db/dbConverters.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbConverters.h` & `klayout-0.29.1/src/db/db/dbConverters.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbDeepEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepEdgePairs.h` & `klayout-0.29.1/src/db/db/dbDeepEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepEdges.cc` & `klayout-0.29.1/src/db/db/dbDeepEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepEdges.h` & `klayout-0.29.1/src/db/db/dbDeepEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepRegion.cc` & `klayout-0.29.1/src/db/db/dbDeepRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepRegion.h` & `klayout-0.29.1/src/db/db/dbDeepRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepShapeStore.cc` & `klayout-0.29.1/src/db/db/dbDeepShapeStore.cc`

 * *Files 2% similar despite different names*

```diff
@@ -294,36 +294,65 @@
   };
 
   class VariantsCreatedListener
     : public tl::Object
   {
   public:
     VariantsCreatedListener (DeepShapeStore::LayoutHolder *lh, db::Layout *ly)
-      : mp_lh (lh)
+      : mp_lh (lh), m_dbu (ly->dbu ())
     {
       ly->variants_created_event.add (this, &VariantsCreatedListener::variants_created);
     }
 
   private:
+    std::string var_desc (const db::ICplxTrans &t)
+    {
+      std::string s;
+      if (t.is_mirror ()) {
+        s += "m";
+        s += tl::to_string (t.angle () * 0.5);
+      } else {
+        s += "r";
+        s += tl::to_string (t.angle ());
+      }
+      if (t.is_mag ()) {
+        s += tl::sprintf ("*%.9g", t.mag ());
+      }
+      if (t.disp () != db::Vector ()) {
+        s += tl::sprintf ("(%.12g,%.12g)", t.disp ().x () * m_dbu, t.disp ().y () * m_dbu);
+      }
+      return s;
+    }
+
     void variants_created (const std::map<db::cell_index_type, std::map<db::ICplxTrans, db::cell_index_type> > *var_map)
     {
       for (std::map<db::cell_index_type, std::map<db::ICplxTrans, db::cell_index_type> >::const_iterator i = var_map->begin (); i != var_map->end (); ++i) {
         for (std::map<db::ICplxTrans, db::cell_index_type>::const_iterator j = i->second.begin (); j != i->second.end (); ++j) {
-          mp_lh->builder.register_variant (i->first, j->second);
+          if (i->first != j->second) {
+            mp_lh->builder.register_variant (i->first, j->second, var_desc (j->first));
+          }
+        }
+        //  NOTE: variant conversion events are registered after variant formation events, so we can
+        //  base the formed variants (first pass) on the originals.
+        for (std::map<db::ICplxTrans, db::cell_index_type>::const_iterator j = i->second.begin (); j != i->second.end (); ++j) {
+          if (i->first == j->second) {
+            mp_lh->builder.register_variant (i->first, j->second, var_desc (j->first));
+          }
         }
       }
     }
 
     DeepShapeStore::LayoutHolder *mp_lh;
+    double m_dbu;
   };
 
   LayoutHolder (const db::ICplxTrans &trans)
     : refs (0), layout (false), builder (&layout, trans), variants_created (this, &layout)
   {
-    //  .. nothing yet ..
+    layout.set_hierarchy_builder (&builder);
   }
 
   void add_layer_ref (unsigned int layer)
   {
     layer_refs [layer] += 1;
   }
```

### Comparing `klayout-0.29.0/src/db/db/dbDeepShapeStore.h` & `klayout-0.29.1/src/db/db/dbDeepShapeStore.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepTexts.cc` & `klayout-0.29.1/src/db/db/dbDeepTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeepTexts.h` & `klayout-0.29.1/src/db/db/dbDeepTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDevice.cc` & `klayout-0.29.1/src/db/db/dbDevice.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDevice.h` & `klayout-0.29.1/src/db/db/dbDevice.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeviceAbstract.cc` & `klayout-0.29.1/src/db/db/dbDeviceAbstract.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeviceAbstract.h` & `klayout-0.29.1/src/db/db/dbDeviceAbstract.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeviceClass.cc` & `klayout-0.29.1/src/db/db/dbDeviceClass.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbDeviceClass.h` & `klayout-0.29.1/src/db/db/dbDeviceClass.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdge.cc` & `klayout-0.29.1/src/db/db/dbEdge.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdge.h` & `klayout-0.29.1/src/db/db/dbEdge.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgeBoolean.cc` & `klayout-0.29.1/src/db/db/dbEdgeBoolean.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgeBoolean.h` & `klayout-0.29.1/src/db/db/dbEdgeBoolean.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePair.cc` & `klayout-0.29.1/src/db/db/dbEdgePair.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePair.h` & `klayout-0.29.1/src/db/db/dbEdgePair.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairFilters.cc` & `klayout-0.29.1/src/db/db/dbEdgePairFilters.cc`

 * *Files 3% similar despite different names*

```diff
@@ -94,21 +94,21 @@
   return m_inverted ? !sel : sel;
 }
 
 // ---------------------------------------------------------------------------------------------------
 //  EdgePairFilterByArea implementation
 
 InternalAngleEdgePairFilter::InternalAngleEdgePairFilter (double a, bool inverted)
-  : m_inverted (inverted), m_checker (a, true, a, true)
+  : m_checker (a, true, a, true, inverted, false)
 {
   //  .. nothing yet ..
 }
 
 InternalAngleEdgePairFilter::InternalAngleEdgePairFilter (double amin, bool include_amin, double amax, bool include_amax, bool inverted)
-  : m_inverted (inverted), m_checker (amin, include_amin, amax, include_amax)
+  : m_checker (amin, include_amin, amax, include_amax, inverted, false)
 {
   //  .. nothing yet ..
 }
 
 bool
 InternalAngleEdgePairFilter::selected (const db::EdgePair &edge_pair) const
 {
@@ -118,11 +118,11 @@
   if (db::sprod_sign (d1, d2) < 0) {
     d1 = -d1;
   }
   if (db::vprod_sign (d1, d2) < 0) {
     std::swap (d1, d2);
   }
 
-  return m_checker (d1, d2) != m_inverted;
+  return m_checker (d1, d2);
 }
 
 }
```

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairFilters.h` & `klayout-0.29.1/src/db/db/dbEdgePairFilters.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairRelations.cc` & `klayout-0.29.1/src/db/db/dbEdgePairRelations.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairRelations.h` & `klayout-0.29.1/src/db/db/dbEdgePairRelations.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairs.h` & `klayout-0.29.1/src/db/db/dbEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairsDelegate.cc` & `klayout-0.29.1/src/db/db/dbEdgePairsDelegate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgePairsDelegate.h` & `klayout-0.29.1/src/db/db/dbEdgePairsDelegate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgeProcessor.cc` & `klayout-0.29.1/src/db/db/dbEdgeProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgeProcessor.h` & `klayout-0.29.1/src/db/db/dbEdgeProcessor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdges.cc` & `klayout-0.29.1/src/db/db/dbEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdges.h` & `klayout-0.29.1/src/db/db/dbEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesDelegate.cc` & `klayout-0.29.1/src/db/db/dbEdgesDelegate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesDelegate.h` & `klayout-0.29.1/src/db/db/dbEdgesDelegate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesLocalOperations.cc` & `klayout-0.29.1/src/db/db/dbEdgesLocalOperations.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesLocalOperations.h` & `klayout-0.29.1/src/db/db/dbEdgesLocalOperations.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesToContours.cc` & `klayout-0.29.1/src/db/db/dbEdgesToContours.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesToContours.h` & `klayout-0.29.1/src/db/db/dbEdgesToContours.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEdgesUtils.cc` & `klayout-0.29.1/src/db/db/dbEdgesUtils.cc`

 * *Files 2% similar despite different names*

```diff
@@ -211,24 +211,32 @@
 
   }
 }
 
 // -------------------------------------------------------------------------------------------------------------
 //  EdgeAngleChecker implementation
 
-EdgeAngleChecker::EdgeAngleChecker (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
+EdgeAngleChecker::EdgeAngleChecker (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
 {
+  if (absolute && angle_start < -db::epsilon) {
+    angle_start = 0.0;
+    include_angle_start = true;
+  }
+
   m_t_start = db::CplxTrans(1.0, angle_start, false, db::DVector ());
   m_t_end = db::CplxTrans(1.0, angle_end, false, db::DVector ());
 
   m_include_start = include_angle_start;
   m_include_end = include_angle_end;
 
   m_big_angle = (angle_end - angle_start + db::epsilon) > 180.0;
   m_all = (angle_end - angle_start - db::epsilon) > 360.0;
+
+  m_absolute = absolute;
+  m_inverse = inverse;
 }
 
 bool
 EdgeAngleChecker::check (const db::Vector &a, const db::Vector &b) const
 {
   db::DVector vout (b);
 
@@ -251,62 +259,62 @@
     return false;
   }
 }
 
 // -------------------------------------------------------------------------------------------------------------
 //  EdgeOrientationFilter implementation
 
-EdgeOrientationFilter::EdgeOrientationFilter (double amin, bool include_amin, double amax, bool include_amax, bool inverse)
-  : m_inverse (inverse), m_checker (amin, include_amin, amax, include_amax)
+EdgeOrientationFilter::EdgeOrientationFilter (double amin, bool include_amin, double amax, bool include_amax, bool inverse, bool absolute)
+  : m_checker (amin, include_amin, amax, include_amax, inverse, absolute)
 {
   //  .. nothing yet ..
 }
 
-EdgeOrientationFilter::EdgeOrientationFilter (double a, bool inverse)
-  : m_inverse (inverse), m_checker (a, true, a, true)
+EdgeOrientationFilter::EdgeOrientationFilter (double a, bool inverse, bool absolute)
+  : m_checker (a, true, a, true, inverse, absolute)
 {
   //  .. nothing yet ..
 }
 
 bool
 EdgeOrientationFilter::selected (const db::Edge &edge) const
 {
   //  NOTE: this edge normalization confines the angle to a range between (-90 .. 90] (-90 excluded).
   //  A horizontal edge has 0 degree, a vertical one has 90 degree.
   if (edge.dx () < 0 || (edge.dx () == 0 && edge.dy () < 0)) {
-    return m_checker (db::Vector (edge.ortho_length (), 0), -edge.d ()) != m_inverse;
+    return m_checker (db::Vector (edge.ortho_length (), 0), -edge.d ());
   } else {
-    return m_checker (db::Vector (edge.ortho_length (), 0), edge.d ()) != m_inverse;
+    return m_checker (db::Vector (edge.ortho_length (), 0), edge.d ());
   }
 }
 
 // -------------------------------------------------------------------------------------------------------------
 //  SpecialEdgeOrientationFilter implementation
 
 SpecialEdgeOrientationFilter::SpecialEdgeOrientationFilter (FilterType type, bool inverse)
   : m_type (type), m_inverse (inverse)
 {
   //  .. nothing yet ..
 }
 
 static EdgeAngleChecker s_ortho_checkers [] = {
-  EdgeAngleChecker (0.0, true, 0.0, true),
-  EdgeAngleChecker (90.0, true, 90.0, true)
+  EdgeAngleChecker (0.0, true, 0.0, true, false, false),
+  EdgeAngleChecker (90.0, true, 90.0, true, false, false)
 };
 
 static EdgeAngleChecker s_diagonal_checkers [] = {
-  EdgeAngleChecker (-45.0, true, -45.0, true),
-  EdgeAngleChecker (45.0, true, 45.0, true)
+  EdgeAngleChecker (-45.0, true, -45.0, true, false, false),
+  EdgeAngleChecker (45.0, true, 45.0, true, false, false)
 };
 
 static EdgeAngleChecker s_orthodiagonal_checkers [] = {
-  EdgeAngleChecker (-45.0, true, -45.0, true),
-  EdgeAngleChecker (0.0, true, 0.0, true),
-  EdgeAngleChecker (45.0, true, 45.0, true),
-  EdgeAngleChecker (90.0, true, 90.0, true)
+  EdgeAngleChecker (-45.0, true, -45.0, true, false, false),
+  EdgeAngleChecker (0.0, true, 0.0, true, false, false),
+  EdgeAngleChecker (45.0, true, 45.0, true, false, false),
+  EdgeAngleChecker (90.0, true, 90.0, true, false, false)
 };
 
 bool
 SpecialEdgeOrientationFilter::selected (const db::Edge &edge) const
 {
   const EdgeAngleChecker *eb, *ee;
```

### Comparing `klayout-0.29.0/src/db/db/dbEdgesUtils.h` & `klayout-0.29.1/src/db/db/dbEdgesUtils.h`

 * *Files 2% similar despite different names*

```diff
@@ -138,30 +138,31 @@
  *  The constraint can be given in terms of a minimum and maximum angle. "include" specifies whether the
  *  angle value itself is included. The operator() will return true, if the angle between the given
  *  edges a and b in matching the constraint.
  */
 class DB_PUBLIC EdgeAngleChecker
 {
 public:
-  EdgeAngleChecker (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end);
+  EdgeAngleChecker (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute);
 
   bool operator() (const db::Edge &a, const db::Edge &b) const
   {
-    return m_all || check (a.d (), b.d ());
+    return (m_all || check (a.d (), b.d ()) || (m_absolute && check (b.d (), a.d ()))) != m_inverse;
   }
 
   bool operator() (const db::Vector &a, const db::Vector &b) const
   {
-    return m_all || check (a, b);
+    return (m_all || check (a, b) || (m_absolute && check (b, a))) != m_inverse;
   }
 
 private:
   db::CplxTrans m_t_start, m_t_end;
   bool m_include_start, m_include_end;
   bool m_big_angle, m_all;
+  bool m_inverse, m_absolute;
 
   bool check (const db::Vector &a, const db::Vector &b) const;
 };
 
 /**
  *  @brief An edge orientation filter for use with Edges::filter or Edges::filtered
  *
@@ -177,30 +178,32 @@
 {
   /**
    *  @brief Constructor
    *
    *  @param amin The minimum angle (measured against the x axis)
    *  @param amax The maximum angle (measured against the x axis)
    *  @param inverse If set to true, only edges not matching this criterion will be filtered
+   *  @param absolute Angles are always positive
    *
    *  This filter will filter out all edges whose angle against x axis
    *  is larger or equal to amin and less than amax.
    */
-  EdgeOrientationFilter (double amin, bool include_amin, double amax, bool include_amax, bool inverse);
+  EdgeOrientationFilter (double amin, bool include_amin, double amax, bool include_amax, bool inverse, bool absolute);
 
   /**
    *  @brief Constructor
    *
    *  @param a The angle (measured against the x axis)
    *  @param inverse If set to true, only edges not matching this criterion will be filtered
+   *  @param absolute Angles are always positive
    *
    *  This filter will filter out all edges whose angle against x axis
    *  is equal to a.
    */
-  EdgeOrientationFilter (double a, bool inverse);
+  EdgeOrientationFilter (double a, bool inverse, bool absolute);
 
   /**
    *  @brief Returns true if the edge orientation matches the criterion
    */
   virtual bool selected (const db::Edge &edge) const;
 
   /**
```

### Comparing `klayout-0.29.0/src/db/db/dbEmptyEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbEmptyEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyEdgePairs.h` & `klayout-0.29.1/src/db/db/dbEmptyEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyEdges.cc` & `klayout-0.29.1/src/db/db/dbEmptyEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyEdges.h` & `klayout-0.29.1/src/db/db/dbEmptyEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyRegion.cc` & `klayout-0.29.1/src/db/db/dbEmptyRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyRegion.h` & `klayout-0.29.1/src/db/db/dbEmptyRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyTexts.cc` & `klayout-0.29.1/src/db/db/dbEmptyTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbEmptyTexts.h` & `klayout-0.29.1/src/db/db/dbEmptyTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFillTool.cc` & `klayout-0.29.1/src/db/db/dbFillTool.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFillTool.h` & `klayout-0.29.1/src/db/db/dbFillTool.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbFlatEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatEdgePairs.h` & `klayout-0.29.1/src/db/db/dbFlatEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatEdges.cc` & `klayout-0.29.1/src/db/db/dbFlatEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatEdges.h` & `klayout-0.29.1/src/db/db/dbFlatEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatRegion.cc` & `klayout-0.29.1/src/db/db/dbFlatRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatRegion.h` & `klayout-0.29.1/src/db/db/dbFlatRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatTexts.cc` & `klayout-0.29.1/src/db/db/dbFlatTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFlatTexts.h` & `klayout-0.29.1/src/db/db/dbFlatTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbForceLink.cc` & `klayout-0.29.1/src/db/db/dbForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbForceLink.h` & `klayout-0.29.1/src/db/db/dbForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFuzzyCellMapping.cc` & `klayout-0.29.1/src/db/db/dbFuzzyCellMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbFuzzyCellMapping.h` & `klayout-0.29.1/src/db/db/dbFuzzyCellMapping.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbGenericShapeIterator.cc` & `klayout-0.29.1/src/db/db/dbGenericShapeIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbGenericShapeIterator.h` & `klayout-0.29.1/src/db/db/dbGenericShapeIterator.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbGlyphs.cc` & `klayout-0.29.1/src/db/db/dbGlyphs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbGlyphs.h` & `klayout-0.29.1/src/db/db/dbGlyphs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHash.h` & `klayout-0.29.1/src/db/db/dbHash.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHershey.cc` & `klayout-0.29.1/src/db/db/dbHershey.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHershey.h` & `klayout-0.29.1/src/db/db/dbHershey.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHersheyFont.h` & `klayout-0.29.1/src/db/db/dbHersheyFont.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHierNetworkProcessor.cc` & `klayout-0.29.1/src/db/db/dbHierNetworkProcessor.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1212,19 +1212,21 @@
     }
 
     //  consider connections to global nets
 
     db::Connectivity::global_nets_iterator ge = mp_conn->end_global_connections (p.first);
     for (db::Connectivity::global_nets_iterator g = mp_conn->begin_global_connections (p.first); g != ge; ++g) {
 
+      bool soft = (g->second != 0);
+
       typename std::map<size_t, typename std::list<cluster_value>::iterator>::iterator icg = m_global_to_clusters.find (g->first);
 
       if (icg == m_global_to_clusters.end ()) {
 
-        if (g->second != 0) {
+        if (soft) {
 
           //  soft connection to a new global cluster
           m_clusters.push_back (cluster_value ());
           typename std::list<cluster_value>::iterator cg = --m_clusters.end ();
 
           cg->second.insert (g->first);
           m_global_to_clusters.insert (std::make_pair (g->first, cg));
@@ -1236,15 +1238,15 @@
           ic->second->second.insert (g->first);
           m_global_to_clusters.insert (std::make_pair (g->first, ic->second));
 
         }
 
       } else if (ic->second != icg->second) {
 
-        if (g->second != 0) {
+        if (soft) {
 
           register_soft_connection (ic->second, icg->second, g->second);
 
         } else {
 
           //  join clusters
           if (ic->second->first.size () < icg->second->first.size ()) {
```

### Comparing `klayout-0.29.0/src/db/db/dbHierNetworkProcessor.h` & `klayout-0.29.1/src/db/db/dbHierNetworkProcessor.h`

 * *Files 0% similar despite different names*

```diff
@@ -509,14 +509,15 @@
 public:
   typedef typename local_cluster<T>::id_type id_type;
   typedef typename local_cluster<T>::box_type box_type;
   typedef typename local_cluster<T>::attr_id attr_id;
   typedef db::box_tree<box_type, local_cluster<T>, local_cluster_box_convert<T> > tree_type;
   typedef typename tree_type::touching_iterator touching_iterator;
   typedef typename tree_type::const_iterator const_iterator;
+  typedef typename tree_type::iterator iterator;
 
   /**
    *  @brief Creates an empty collection
    */
   local_clusters ();
 
   /**
@@ -563,14 +564,30 @@
    */
   const_iterator end () const
   {
     return m_clusters.end ();
   }
 
   /**
+   *  @brief Gets the clusters (begin iterator)
+   */
+  iterator begin ()
+  {
+    return m_clusters.begin ();
+  }
+
+  /**
+   *  @brief Gets the clusters (end iterator)
+   */
+  iterator end ()
+  {
+    return m_clusters.end ();
+  }
+
+  /**
    *  @brief Gets a value indicating whether the cluster set is empty
    */
   bool empty () const
   {
     return m_clusters.empty ();
   }
```

### Comparing `klayout-0.29.0/src/db/db/dbHierProcessor.cc` & `klayout-0.29.1/src/db/db/dbHierProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHierProcessor.h` & `klayout-0.29.1/src/db/db/dbHierProcessor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbHierarchyBuilder.cc` & `klayout-0.29.1/src/db/db/dbHierarchyBuilder.cc`

 * *Files 3% similar despite different names*

```diff
@@ -178,36 +178,58 @@
 HierarchyBuilder::reset ()
 {
   m_initial_pass = true;
   mp_initial_cell = 0;
 
   m_cells_to_be_filled.clear ();
   m_cell_map.clear ();
+  m_variants_of_sources_map.clear ();
   m_cells_seen.clear ();
   m_cell_stack.clear ();
   m_cm_entry = null_iterator;
   m_cm_new_entry = false;
 }
 
+const std::pair<db::cell_index_type, std::string> &
+HierarchyBuilder::variant_of_source (db::cell_index_type target) const
+{
+  static std::pair<db::cell_index_type, std::string> def (std::numeric_limits<db::cell_index_type>::max (), std::string ());
+
+  auto vs = m_variants_of_sources_map.find (target);
+  return vs != m_variants_of_sources_map.end () ? vs->second : def;
+}
+
 void
-HierarchyBuilder::register_variant (db::cell_index_type non_var, db::cell_index_type var)
+HierarchyBuilder::register_variant (db::cell_index_type non_var, db::cell_index_type var, const std::string &description)
 {
   //  non_var (despite its name) may be a variant created previously.
   variant_to_original_target_map_type::const_iterator v = m_variants_to_original_target_map.find (non_var);
   if (v != m_variants_to_original_target_map.end ()) {
     non_var = v->second;
   }
 
   m_original_targets_to_variants_map [non_var].push_back (var);
   m_variants_to_original_target_map.insert (std::make_pair (var, non_var));
+
+  auto vs = m_variants_of_sources_map.find (non_var);
+  if (vs != m_variants_of_sources_map.end ()) {
+    std::string new_description = vs->second.second;
+    if (! new_description.empty ()) {
+      new_description += ";";
+    }
+    new_description += description;
+    m_variants_of_sources_map [var] = std::make_pair (vs->second.first, new_description);
+  }
 }
 
 void
 HierarchyBuilder::unregister_variant (db::cell_index_type var)
 {
+  m_variants_of_sources_map.erase (var);
+
   variant_to_original_target_map_type::iterator v = m_variants_to_original_target_map.find (var);
   if (v == m_variants_to_original_target_map.end ()) {
     return;
   }
 
   original_target_to_variants_map_type::iterator rv = m_original_targets_to_variants_map.find (v->second);
   tl_assert (rv != m_original_targets_to_variants_map.end ());
@@ -253,14 +275,15 @@
 
   CellMapKey key (iter->top_cell ()->cell_index (), false, std::set<db::Box> ());
   m_cm_entry = m_cell_map.find (key);
 
   if (m_cm_entry == m_cell_map.end ()) {
     db::cell_index_type new_top_index = mp_target->add_cell (iter->layout ()->cell_name (key.original_cell));
     m_cm_entry = m_cell_map.insert (std::make_pair (key, new_top_index)).first;
+    m_variants_of_sources_map.insert (std::make_pair (new_top_index, std::make_pair (key.original_cell, std::string ())));
   }
 
   db::Cell &new_top = mp_target->cell (m_cm_entry->second);
   m_cells_seen.insert (key);
 
   //  NOTE: we consider the top cell "new" if it does not have instances.
   //  We can do so as the recursive shape iterator will always deliver all instances
@@ -320,25 +343,42 @@
   m_cm_new_entry = false;
 
   db::cell_index_type new_cell;
 
   if (m_cm_entry == m_cell_map.end ()) {
 
     std::string cn = cell_name;
+    std::string description;
     if (! key.clip_region.empty ()) {
       cn += "$CLIP_VAR";
+      description += "CLIP";
+
     }
     if (key.inactive) {
       cn += "$DIS";
+      if (! description.empty ()) {
+        description += "/";
+      }
+      description += "DISABLED";
     }
+
     new_cell = mp_target->add_cell (cn.c_str ());
+
+    std::string new_name = mp_target->cell_name (new_cell);
+    if (new_name.size () > cn.size ()) {
+      //  use cell name extension to uniquify the description
+      description += new_name.c_str () + cn.size ();
+    }
+
     m_cm_entry = m_cell_map.insert (std::make_pair (key, new_cell)).first;
     m_cm_new_entry = true;
     m_cells_to_be_filled.insert (new_cell);
 
+    m_variants_of_sources_map.insert (std::make_pair (new_cell, std::make_pair (key.original_cell, description)));
+
   } else {
     new_cell = m_cm_entry->second;
   }
 
   return new_cell;
 }
```

### Comparing `klayout-0.29.0/src/db/db/dbHierarchyBuilder.h` & `klayout-0.29.1/src/db/db/dbHierarchyBuilder.h`

 * *Files 3% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 
   /**
    *  @brief Marks a cell as a variant of another
    *
    *  The first cell is either the original, non-variant target cell or itself a variant.
    *  The second cell will be registered as a variant of the first one.
    */
-  void register_variant (db::cell_index_type non_var, db::cell_index_type var);
+  void register_variant (db::cell_index_type non_var, db::cell_index_type var, const std::string &description);
 
   /**
    *  @brief Unregisters a cell as a variant
    */
   void unregister_variant (db::cell_index_type var);
 
   /**
@@ -401,28 +401,44 @@
    */
   bool is_variant (db::cell_index_type ci) const
   {
     return m_variants_to_original_target_map.find (ci) != m_variants_to_original_target_map.end ();
   }
 
   /**
+   *  @brief Gets the information about the target/source + variant relationship
+   *
+   *  For a target cell, returns a pointer to a pair with the cell index of the source cell and
+   *  a string describing the variant this cell forms of the source cell.
+   *
+   *  The description string is empty if the cell is not a variant.
+   */
+  const std::pair<db::cell_index_type, std::string> &variant_of_source (db::cell_index_type target) const;
+
+  /**
    *  @brief Gets the original target for a variant cell
+   *
+   *  The original cell is the first-generation target-space cell that variants have been created for.
+   *  This still can mean that the original cell is a clip variant of a source cell.
+   *
+   *  Target-to-source variants can be derived with "variant_of_source".
    */
   db::cell_index_type original_target_for_variant (db::cell_index_type ci) const;
 
 private:
   db::cell_index_type make_cell_variant (const HierarchyBuilder::CellMapKey &key, const std::string &cell_name);
 
   tl::weak_ptr<db::Layout> mp_target;
   HierarchyBuilderShapeReceiver *mp_pipe;
   bool m_initial_pass;
   db::RecursiveShapeIterator m_source;
   cell_map_type m_cell_map;
   original_target_to_variants_map_type m_original_targets_to_variants_map;
   variant_to_original_target_map_type m_variants_to_original_target_map;
+  std::map<db::cell_index_type, std::pair<db::cell_index_type, std::string> > m_variants_of_sources_map;
 
   std::set<cell_map_type::key_type> m_cells_seen;
   std::set<db::cell_index_type> m_cells_to_be_filled;
   cell_map_type::const_iterator m_cm_entry;
   bool m_cm_new_entry;
   unsigned int m_target_layer;
   bool m_wants_all_cells;
```

### Comparing `klayout-0.29.0/src/db/db/dbInit.cc` & `klayout-0.29.1/src/db/db/dbInit.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbInit.h` & `klayout-0.29.1/src/db/db/dbInit.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbInstElement.cc` & `klayout-0.29.1/src/db/db/dbInstElement.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbInstElement.h` & `klayout-0.29.1/src/db/db/dbInstElement.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbInstances.cc` & `klayout-0.29.1/src/db/db/dbInstances.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbInstances.h` & `klayout-0.29.1/src/db/db/dbInstances.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayer.h` & `klayout-0.29.1/src/db/db/dbLayer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayerMapping.cc` & `klayout-0.29.1/src/db/db/dbLayerMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayerMapping.h` & `klayout-0.29.1/src/db/db/dbLayerMapping.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayerProperties.cc` & `klayout-0.29.1/src/db/db/dbLayerProperties.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayerProperties.h` & `klayout-0.29.1/src/db/db/dbLayerProperties.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayout.cc` & `klayout-0.29.1/src/db/db/dbLayout.cc`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,15 @@
 
 // -----------------------------------------------------------------
 //  Implementation of the Layout class
 
 Layout::Layout (db::Manager *manager)
   : db::Object (manager),
     mp_library (0),
+    mp_builder (0),
     m_cells_size (0),
     m_invalid (0),
     m_top_cells (0),
     m_dbu (0.001),
     m_prop_id (0),
     m_properties_repository (this),
     m_do_cleanup (false),
@@ -450,14 +451,15 @@
 {
   // .. nothing yet ..
 }
 
 Layout::Layout (bool editable, db::Manager *manager)
   : db::Object (manager),
     mp_library (0),
+    mp_builder (0),
     m_cells_size (0),
     m_invalid (0),
     m_top_cells (0),
     m_dbu (0.001),
     m_prop_id (0),
     m_properties_repository (this),
     m_do_cleanup (false),
@@ -469,14 +471,15 @@
 Layout::Layout (const db::Layout &layout)
   : db::Object (layout),
     db::LayoutStateModel (),
     gsi::ObjectBase (),
     tl::Object (),
     tl::UniqueId (),
     mp_library (0),
+    mp_builder (0),
     m_cells_size (0),
     m_invalid (0),
     m_top_cells (0),
     m_dbu (0.001),
     m_prop_id (0),
     m_properties_repository (this),
     m_do_cleanup (false),
```

### Comparing `klayout-0.29.0/src/db/db/dbLayout.h` & `klayout-0.29.1/src/db/db/dbLayout.h`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 class Edges;
 class EdgePairs;
 class Texts;
 class Technology;
 class CellMapping;
 class LayerMapping;
 class VariantsCollectorBase;
+class HierarchyBuilder;
 
 template <class Coord> class generic_repository;
 typedef generic_repository<db::Coord> GenericRepository;
 
 /**
  *  @brief The cell iterator
  *
@@ -2110,14 +2111,32 @@
   /**
    *  @brief Gets the meta info value for a meta info object with the given name ID for the given cell
    *  If no object with that name exists, an empty string is returned
    */
   const MetaInfo &meta_info (db::cell_index_type ci, meta_info_name_id_type name_id) const;
 
   /**
+   *  @brief Sets the hierarchy builder reference
+   *  Used internally
+   */
+  void set_hierarchy_builder (db::HierarchyBuilder *builder)
+  {
+    mp_builder = builder;
+  }
+
+  /**
+   *  @brief Gets the hierarchy builder
+   *  Used internally
+   */
+  db::HierarchyBuilder *builder () const
+  {
+    return mp_builder;
+  }
+
+  /**
    *  @brief This event is triggered when the technology changes
    */
   tl::Event technology_changed_event;
 
   /**
    *  @brief This event is raised when cell variants are built
    *  It will specify a list of cells with their new variants.
@@ -2134,14 +2153,15 @@
    *  This will guarantee mainly that region queries can be performed
    *  on all levels of the graph.
    */
   virtual void do_update ();
 
 private:
   db::Library *mp_library;
+  db::HierarchyBuilder *mp_builder;
   cell_list m_cells;
   size_t m_cells_size;
   cell_ptr_vector m_cell_ptrs;
   cell_index_vector m_free_cell_indices;
   mutable unsigned int m_invalid;
   cell_index_vector m_top_down_list;
   size_t m_top_cells;
```

### Comparing `klayout-0.29.0/src/db/db/dbLayoutContextHandler.cc` & `klayout-0.29.1/src/db/db/dbLayoutContextHandler.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutContextHandler.h` & `klayout-0.29.1/src/db/db/dbLayoutContextHandler.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutDiff.cc` & `klayout-0.29.1/src/db/db/dbLayoutDiff.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutDiff.h` & `klayout-0.29.1/src/db/db/dbLayoutDiff.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutLayers.cc` & `klayout-0.29.1/src/db/db/dbLayoutLayers.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutLayers.h` & `klayout-0.29.1/src/db/db/dbLayoutLayers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutQuery.cc` & `klayout-0.29.1/src/db/db/dbLayoutQuery.cc`

 * *Files 1% similar despite different names*

```diff
@@ -659,15 +659,35 @@
           objectives ().request_cell (c->cell_index ());
         }
       }
 
     }
   }
 
-  virtual void reset (FilterStateBase *previous) 
+  db::Instance instance () const
+  {
+    return mp_parent->sorted_inst_ptr (std::distance (mp_parent->begin_sorted_insts (), m_inst));
+  }
+
+  void validate_instance ()
+  {
+    //  during modification or delete, instances may vanish while iterating,
+    //  hence we need to check during iteration
+    while (m_inst != m_inst_end && !mp_parent->is_valid (instance ())) {
+      ++m_inst;
+    }
+  }
+
+  void next_valid_instance ()
+  {
+    ++m_inst;
+    validate_instance ();
+  }
+
+  virtual void reset (FilterStateBase *previous)
   {
     FilterStateBase::reset (previous);
 
     m_pattern.reset ();
     m_ignored.clear ();
 
     //  Get the parent cell by asking the previous states 
@@ -703,24 +723,26 @@
         } 
 
       } else {
 
         m_inst = mp_parent->begin_sorted_insts ();
         m_inst_end = mp_parent->end_sorted_insts ();
 
+        validate_instance ();
+
         while (m_inst != m_inst_end) {
 
           db::cell_index_type cid = (*m_inst)->object ().cell_index ();
           if (layout ()->is_valid_cell_index (cid) && cell_matches (cid)) {
             break;
           }
 
-          ++m_inst;
+          next_valid_instance ();
           while (m_inst != m_inst_end && (*m_inst)->object ().cell_index () == cid) {
-            ++m_inst;
+            next_valid_instance ();
           }
 
         }
 
         if (m_inst != m_inst_end && !m_reading) {
           m_i = mp_parent->sorted_inst_ptr (std::distance (mp_parent->begin_sorted_insts (), m_inst));
         }
@@ -756,43 +778,43 @@
 
         if (m_instance_mode == ExplodedInstances) {
           ++m_array_iter;
         }
 
         if (m_instance_mode != ExplodedInstances || m_array_iter.at_end ()) {
 
-          if (! m_reading && m_i != mp_parent->sorted_inst_ptr (std::distance (mp_parent->begin_sorted_insts (), m_inst))) {
+          if (! m_reading && m_i != instance ()) {
             m_ignored.insert (m_i);
           }
 
           do {
 
             db::cell_index_type cid = (*m_inst)->object ().cell_index ();
-            ++m_inst;
+            next_valid_instance ();
 
             if (m_inst != m_inst_end && (*m_inst)->object ().cell_index () != cid) {
 
               while (m_inst != m_inst_end) {
 
                 cid = (*m_inst)->object ().cell_index ();
                 if (layout ()->is_valid_cell_index (cid) && cell_matches (cid)) {
                   break;
                 }
 
-                ++m_inst;
+                next_valid_instance ();
                 while (m_inst != m_inst_end && (*m_inst)->object ().cell_index () == cid) {
-                  ++m_inst;
+                  next_valid_instance ();
                 }
 
               }
 
             }
 
             if (! m_reading && m_inst != m_inst_end) {
-              m_i = mp_parent->sorted_inst_ptr (std::distance (mp_parent->begin_sorted_insts (), m_inst));
+              m_i = instance ();
             } else {
               break;
             }
 
           } while (m_ignored.find (m_i) != m_ignored.end ());
 
           if (m_inst != m_inst_end) {
```

### Comparing `klayout-0.29.0/src/db/db/dbLayoutQuery.h` & `klayout-0.29.1/src/db/db/dbLayoutQuery.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutStateModel.cc` & `klayout-0.29.1/src/db/db/dbLayoutStateModel.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutStateModel.h` & `klayout-0.29.1/src/db/db/dbLayoutStateModel.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlist.cc` & `klayout-0.29.1/src/db/db/dbLayoutToNetlist.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlist.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlist.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistEnums.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistEnums.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistFormatDefs.cc` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistFormatDefs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistFormatDefs.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistFormatDefs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistReader.cc` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistReader.cc`

 * *Files 1% similar despite different names*

```diff
@@ -391,20 +391,26 @@
       read_word_or_quoted (class_name);
       read_word_or_quoted (templ_name);
 
       if (netlist->device_class_by_name (class_name) != 0) {
         throw tl::Exception (tl::to_string (tr ("Duplicate definition of device class: ")) + class_name);
       }
 
-      db::DeviceClassTemplateBase *dct = db::DeviceClassTemplateBase::template_by_name (templ_name);
-      if (! dct) {
-        throw tl::Exception (tl::to_string (tr ("Invalid device class template: ")) + templ_name);
+      db::DeviceClass *dc;
+      if (templ_name.empty ()) {
+        //  generic device class (issue #1696)
+        dc = new db::DeviceClass ();
+      } else {
+        db::DeviceClassTemplateBase *dct = db::DeviceClassTemplateBase::template_by_name (templ_name);
+        if (! dct) {
+          throw tl::Exception (tl::to_string (tr ("Invalid device class template: ")) + templ_name);
+        }
+        dc = dct->create ();
       }
 
-      db::DeviceClass *dc = dct->create ();
       dc->set_name (class_name);
       netlist->add_device_class (dc);
 
       while (br) {
 
         if (test (skeys::terminal_key) || test (lkeys::terminal_key)) {
```

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistReader.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistSoftConnections.cc` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistSoftConnections.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistSoftConnections.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistSoftConnections.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistWriter.cc` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutToNetlistWriter.h` & `klayout-0.29.1/src/db/db/dbLayoutToNetlistWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutUtils.cc` & `klayout-0.29.1/src/db/db/dbLayoutUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutUtils.h` & `klayout-0.29.1/src/db/db/dbLayoutUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematic.cc` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematic.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematic.h` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematic.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicFormatDefs.cc` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicFormatDefs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicFormatDefs.h` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicFormatDefs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicReader.cc` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicReader.h` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicWriter.cc` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLayoutVsSchematicWriter.h` & `klayout-0.29.1/src/db/db/dbLayoutVsSchematicWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibrary.cc` & `klayout-0.29.1/src/db/db/dbLibrary.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibrary.h` & `klayout-0.29.1/src/db/db/dbLibrary.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibraryManager.cc` & `klayout-0.29.1/src/db/db/dbLibraryManager.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibraryManager.h` & `klayout-0.29.1/src/db/db/dbLibraryManager.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibraryProxy.cc` & `klayout-0.29.1/src/db/db/dbLibraryProxy.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLibraryProxy.h` & `klayout-0.29.1/src/db/db/dbLibraryProxy.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLoadLayoutOptions.cc` & `klayout-0.29.1/src/db/db/dbLoadLayoutOptions.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLoadLayoutOptions.h` & `klayout-0.29.1/src/db/db/dbLoadLayoutOptions.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLocalOperation.cc` & `klayout-0.29.1/src/db/db/dbLocalOperation.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLocalOperation.h` & `klayout-0.29.1/src/db/db/dbLocalOperation.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLocalOperationUtils.cc` & `klayout-0.29.1/src/db/db/dbLocalOperationUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLocalOperationUtils.h` & `klayout-0.29.1/src/db/db/dbLocalOperationUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLog.cc` & `klayout-0.29.1/src/db/db/dbLog.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbLog.h` & `klayout-0.29.1/src/db/db/dbLog.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbManager.cc` & `klayout-0.29.1/src/db/db/dbManager.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbManager.h` & `klayout-0.29.1/src/db/db/dbManager.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMatrix.cc` & `klayout-0.29.1/src/db/db/dbMatrix.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMatrix.h` & `klayout-0.29.1/src/db/db/dbMatrix.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMemStatistics.cc` & `klayout-0.29.1/src/db/db/dbMemStatistics.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMemStatistics.h` & `klayout-0.29.1/src/db/db/dbMemStatistics.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMetaInfo.h` & `klayout-0.29.1/src/db/db/dbMetaInfo.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbMutableEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableEdgePairs.h` & `klayout-0.29.1/src/db/db/dbMutableEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableEdges.cc` & `klayout-0.29.1/src/db/db/dbMutableEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableEdges.h` & `klayout-0.29.1/src/db/db/dbMutableEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableRegion.cc` & `klayout-0.29.1/src/db/db/dbMutableRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableRegion.h` & `klayout-0.29.1/src/db/db/dbMutableRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableTexts.cc` & `klayout-0.29.1/src/db/db/dbMutableTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbMutableTexts.h` & `klayout-0.29.1/src/db/db/dbMutableTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNamedLayerReader.cc` & `klayout-0.29.1/src/db/db/dbNamedLayerReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNamedLayerReader.h` & `klayout-0.29.1/src/db/db/dbNamedLayerReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNet.cc` & `klayout-0.29.1/src/db/db/dbNet.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNet.h` & `klayout-0.29.1/src/db/db/dbNet.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetShape.cc` & `klayout-0.29.1/src/db/db/dbNetShape.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetShape.h` & `klayout-0.29.1/src/db/db/dbNetShape.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlist.cc` & `klayout-0.29.1/src/db/db/dbNetlist.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlist.h` & `klayout-0.29.1/src/db/db/dbNetlist.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompare.cc` & `klayout-0.29.1/src/db/db/dbNetlistCompare.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompare.h` & `klayout-0.29.1/src/db/db/dbNetlistCompare.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareCore.cc` & `klayout-0.29.1/src/db/db/dbNetlistCompareCore.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareCore.h` & `klayout-0.29.1/src/db/db/dbNetlistCompareCore.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareGraph.cc` & `klayout-0.29.1/src/db/db/dbNetlistCompareGraph.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareGraph.h` & `klayout-0.29.1/src/db/db/dbNetlistCompareGraph.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareUtils.cc` & `klayout-0.29.1/src/db/db/dbNetlistCompareUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCompareUtils.h` & `klayout-0.29.1/src/db/db/dbNetlistCompareUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCrossReference.cc` & `klayout-0.29.1/src/db/db/dbNetlistCrossReference.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistCrossReference.h` & `klayout-0.29.1/src/db/db/dbNetlistCrossReference.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceClasses.cc` & `klayout-0.29.1/src/db/db/dbNetlistDeviceClasses.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceClasses.h` & `klayout-0.29.1/src/db/db/dbNetlistDeviceClasses.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceExtractor.cc` & `klayout-0.29.1/src/db/db/dbNetlistDeviceExtractor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceExtractor.h` & `klayout-0.29.1/src/db/db/dbNetlistDeviceExtractor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceExtractorClasses.cc` & `klayout-0.29.1/src/db/db/dbNetlistDeviceExtractorClasses.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistDeviceExtractorClasses.h` & `klayout-0.29.1/src/db/db/dbNetlistDeviceExtractorClasses.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistExtractor.cc` & `klayout-0.29.1/src/db/db/dbNetlistExtractor.cc`

 * *Files 2% similar despite different names*

```diff
@@ -224,16 +224,16 @@
   }
 
   std::map<db::cell_index_type, std::map<size_t, size_t> > pins_per_cluster_per_cell;
   for (db::Layout::bottom_up_const_iterator cid = mp_layout->begin_bottom_up (); cid != mp_layout->end_bottom_up (); ++cid) {
 
     const db::Cell &cell = mp_layout->cell (*cid);
 
-    const connected_clusters_type &clusters = mp_clusters->clusters_per_cell (*cid);
-    if (clusters.empty ()) {
+    connected_clusters_type &per_cell_clusters = mp_clusters->clusters_per_cell (*cid);
+    if (per_cell_clusters.empty ()) {
 
       bool any_good = false;
 
       //  in case of "include floating subcircuits" check whether we have a child cell which has a circuit attached in this case
       if (include_floating_subcircuits ()) {
         for (db::Cell::child_cell_iterator cc = cell.begin_child_cells (); ! any_good && ! cc.at_end (); ++cc) {
           any_good = (circuits.find (*cc) != circuits.end ());
@@ -247,15 +247,15 @@
 
     }
 
     db::DeviceAbstract *dm = nl.device_abstract_by_cell_index (*cid);
     if (dm) {
       //  This is a device abstract cell:
       //  make the terminal to cluster ID connections for the device abstract from the device cells
-      make_device_abstract_connections (dm, clusters);
+      make_device_abstract_connections (dm, per_cell_clusters);
       continue;
     }
 
     //  a cell makes a new circuit (or uses an existing one)
 
     db::Circuit *circuit = 0;
 
@@ -280,68 +280,68 @@
         for (db::CellInstArray::iterator ii = inst->begin (); ! ii.at_end (); ++ii) {
           make_subcircuit (circuit, inst->cell_index (), inst->complex_trans (*ii), subcircuits, circuits);
         }
       }
 
     }
 
-    for (connected_clusters_type::all_iterator c = clusters.begin_all (); ! c.at_end (); ++c) {
+    for (connected_clusters_type::all_iterator c = per_cell_clusters.begin_all (); ! c.at_end (); ++c) {
 
-      const db::local_cluster<db::NetShape> &lc = clusters.cluster_by_id (*c);
-      const connected_clusters_type::connections_type &cc = clusters.connections_for_cluster (*c);
-      const std::set<size_t> &sc_up = clusters.upward_soft_connections (*c);
-      const std::set<size_t> &sc_down = clusters.downward_soft_connections (*c);
+      const db::local_cluster<db::NetShape> &lc = per_cell_clusters.cluster_by_id (*c);
+      const connected_clusters_type::connections_type &cc = per_cell_clusters.connections_for_cluster (*c);
+      const std::set<size_t> &sc_up = per_cell_clusters.upward_soft_connections (*c);
+      const std::set<size_t> &sc_down = per_cell_clusters.downward_soft_connections (*c);
       if (cc.empty () && sc_up.empty () && sc_down.empty () && lc.empty ()) {
         //  this is an entirely empty cluster so we skip it.
         //  Such clusters are left over when joining clusters.
         continue;
       }
 
       db::Net *net = new db::Net ();
       net->set_cluster_id (*c);
       circuit->add_net (net);
 
       //  make subcircuit connections (also make the subcircuits if required) from the connections of the clusters
-      make_and_connect_subcircuits (circuit, clusters, *c, net, subcircuits, circuits, pins_per_cluster_per_cell);
+      make_and_connect_subcircuits (circuit, per_cell_clusters, *c, net, subcircuits, circuits, pins_per_cluster_per_cell);
 
       //  connect devices
-      connect_devices (circuit, clusters, *c, net);
+      connect_devices (circuit, per_cell_clusters, *c, net);
 
       //  collect labels to net names
       std::set<std::string> net_names;
-      collect_labels (clusters, *c, net_names);
+      collect_labels (per_cell_clusters, *c, net_names);
 
       //  add the global names as second priority
       if (net_names.empty ()) {
         const db::local_cluster<db::NetShape>::global_nets &gn = lc.get_global_nets ();
         for (db::local_cluster<db::NetShape>::global_nets::const_iterator g = gn.begin (); g != gn.end (); ++g) {
           net_names.insert (conn.global_net_name (*g));
         }
       }
 
 #if 0
       //  This code will pull net names from subcircuits into their parents if those nets are dummy connections
       //  made to satisfy the subcircuit's pin, but not to make a physical connection.
       //  Don't know whether this is a good idea, so this code is disabled for now.
 
-      if (net_names.empty () && clusters.is_dummy (*c) && net->subcircuit_pin_count () == 1) {
+      if (net_names.empty () && per_cell_clusters.is_dummy (*c) && net->subcircuit_pin_count () == 1) {
         //  in the case of a dummy connection (partially connected subcircuits) create a
         //  new name indicating the subcircuit and the subcircuit net name - this makes subcircuit
         //  net names available (the net is pseudo-root inside in the subcircuit)
         const db::NetSubcircuitPinRef &sc_pin = *net->begin_subcircuit_pins ();
         const db::Net *sc_net = sc_pin.subcircuit ()->circuit_ref ()->net_for_pin (sc_pin.pin_id ());
         if (sc_net && ! sc_net->name ().empty ()) {
           net_names.insert (sc_pin.subcircuit ()->expanded_name () + ":" + sc_net->name ());
         }
       }
 #endif
 
       assign_net_names (net, net_names);
 
-      if (! clusters.is_root (*c)) {
+      if (! per_cell_clusters.is_root (*c)) {
         //  a non-root cluster makes a pin
         size_t pin_id = make_pin (circuit, net);
         c2p.insert (std::make_pair (*c, pin_id));
       }
 
     }
 
@@ -360,36 +360,81 @@
       nn += *n;
     }
   }
 
   net->set_name (nn);
 }
 
+static void
+collect_soft_connected_clusters (size_t from_id, const NetlistExtractor::connected_clusters_type &clusters, std::set<size_t> &ids)
+{
+  if (ids.find (from_id) != ids.end ()) {
+    return;
+  }
+
+  ids.insert (from_id);
+
+  auto upward = clusters.upward_soft_connections (from_id);
+  for (auto i = upward.begin (); i != upward.end (); ++i) {
+    collect_soft_connected_clusters (*i, clusters, ids);
+  }
+
+  auto downward = clusters.downward_soft_connections (from_id);
+  for (auto i = downward.begin (); i != downward.end (); ++i) {
+    collect_soft_connected_clusters (*i, clusters, ids);
+  }
+}
+
 void
-NetlistExtractor::make_device_abstract_connections (db::DeviceAbstract *dm, const connected_clusters_type &clusters)
+NetlistExtractor::make_device_abstract_connections (db::DeviceAbstract *dm, connected_clusters_type &clusters)
 {
   //  make the terminal to cluster ID connections for the device abstract from the device cells
 
   if (m_terminal_annot_name_id.first) {
 
-    for (connected_clusters_type::const_iterator dc = clusters.begin (); dc != clusters.end (); ++dc) {
+    for (connected_clusters_type::iterator dc = clusters.begin (); dc != clusters.end (); ++dc) {
 
-      for (local_cluster_type::attr_iterator a = dc->begin_attr (); a != dc->end_attr (); ++a) {
+      std::set<size_t> ids;
+      collect_soft_connected_clusters (dc->id (), clusters, ids);
 
-        if (! db::is_prop_id_attr (*a)) {
-          continue;
-        }
+      for (auto id = ids.begin (); id != ids.end (); ++id) {
+
+        const local_cluster_type &lc = clusters.cluster_by_id (*id);
+        bool join = false;
 
-        db::properties_id_type pi = db::prop_id_from_attr (*a);
+        for (local_cluster_type::attr_iterator a = lc.begin_attr (); a != lc.end_attr (); ++a) {
 
-        const db::PropertiesRepository::properties_set &ps = mp_layout->properties_repository ().properties (pi);
-        for (db::PropertiesRepository::properties_set::const_iterator j = ps.begin (); j != ps.end (); ++j) {
-          if (j->first == m_terminal_annot_name_id.second) {
-            dm->set_cluster_id_for_terminal (j->second.to<size_t> (), dc->id ());
+          if (! db::is_prop_id_attr (*a)) {
+            continue;
           }
+
+          db::properties_id_type pi = db::prop_id_from_attr (*a);
+
+          const db::PropertiesRepository::properties_set &ps = mp_layout->properties_repository ().properties (pi);
+          for (db::PropertiesRepository::properties_set::const_iterator j = ps.begin (); j != ps.end (); ++j) {
+
+            if (j->first == m_terminal_annot_name_id.second) {
+
+              size_t terminal_id = j->second.to<size_t> ();
+              if (*id != dc->id ()) {
+                tl::warn << tl::sprintf (tl::to_string (tr ("Ignoring soft connection at device terminal %s for device %s")), dm->device_class ()->terminal_definition (terminal_id)->name (), dm->device_class ()->name ());
+                join = true;
+              }
+
+              dm->set_cluster_id_for_terminal (terminal_id, dc->id ());
+
+            }
+
+          }
+
+        }
+
+        if (join) {
+          //  copy the terminal attributes and shapes so we attach the terminal here in the device connection step
+          clusters.join_cluster_with (dc->id (), *id);
         }
 
       }
 
     }
 
   }
```

### Comparing `klayout-0.29.0/src/db/db/dbNetlistExtractor.h` & `klayout-0.29.1/src/db/db/dbNetlistExtractor.h`

 * *Files 0% similar despite different names*

```diff
@@ -229,14 +229,14 @@
   void collect_labels (const connected_clusters_type &clusters,
                        size_t cid,
                        std::set<std::string> &net_names);
 
   /**
    *  @brief Makes the terminal to cluster ID connections of the device abstract
    */
-  void make_device_abstract_connections (db::DeviceAbstract *dm, const connected_clusters_type &clusters);
+  void make_device_abstract_connections (db::DeviceAbstract *dm, connected_clusters_type &clusters);
 
 };
 
 }
 
 #endif
```

### Comparing `klayout-0.29.0/src/db/db/dbNetlistObject.cc` & `klayout-0.29.1/src/db/db/dbNetlistObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistObject.h` & `klayout-0.29.1/src/db/db/dbNetlistObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistReader.cc` & `klayout-0.29.1/src/db/db/dbNetlistReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistReader.h` & `klayout-0.29.1/src/db/db/dbNetlistReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReader.cc` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReader.cc`

 * *Files 1% similar despite different names*

```diff
@@ -629,14 +629,21 @@
           m_in_lib.push_back (libname);
           ex.expect_end ();
 
         }
 
       } else if (ex.test_without_case (".endl")) {
 
+        std::string name;
+        if (ex.try_read_name (name)) {
+          if (! m_in_lib.empty () && mp_netlist->normalize_name (name) != m_in_lib.back ()) {
+            warn (tl::sprintf (tl::to_string (tr (".endl has wrong name: %s given, %s expected")), mp_netlist->normalize_name (name), m_in_lib.back ()));
+          }
+        }
+
         if (! m_in_lib.empty ()) {
           m_in_lib.pop_back ();
         } else {
           warn (tl::to_string (tr ("Ignoring .endl without .lib")));
         }
 
         ex.expect_end ();
@@ -932,14 +939,20 @@
   if (c == m_circuits.end ()) {
     return 0;
   }
   auto cp = c->second.find (pv);
   if (cp == c->second.end ()) {
     return 0;
   }
+
+  //  a null pointer indicates that we are currently defining this circuit
+  if (cp->second == 0) {
+    error (tl::sprintf (tl::to_string (tr ("Subcircuit '%s' called recursively")), cc->name ()));
+  }
+
   return cp->second;
 }
 
 void
 SpiceNetlistBuilder::register_circuit_for (const SpiceCachedCircuit *cc, const parameters_type &pv, db::Circuit *circuit, bool anonymous_top_level)
 {
   m_circuits [cc][pv] = circuit;
@@ -1044,15 +1057,16 @@
   mp_netlist->add_circuit (c);
   if (pv.empty ()) {
     c->set_name (cc->name ());
   } else {
     c->set_name (make_circuit_name (cc->name (), pv));
   }
 
-  register_circuit_for (cc, pv, c, anonymous_top_level);
+  //  pre-register the circuit - allows detecting recursive calls
+  register_circuit_for (cc, pv, 0, false);
 
   std::unique_ptr<std::map<std::string, db::Net *> > n2n (mp_nets_by_name.release ());
   mp_nets_by_name.reset (0);
 
   NetlistSpiceReader::parameters_type vars = cc->parameters ();
   for (auto p = pv.begin (); p != pv.end (); ++p) {
     vars [p->first] = p->second;
@@ -1084,14 +1098,22 @@
   mp_current_card = 0;
   mp_nets_by_name.reset (n2n.release ());
 
   std::swap (cc, mp_circuit);
   std::swap (c, mp_netlist_circuit);
   std::swap (vars, m_variables);
 
+  //  final registration if required
+  if (! anonymous_top_level || ! c->is_empty ()) {
+    register_circuit_for (cc, pv, c, anonymous_top_level);
+  } else {
+    mp_netlist->remove_circuit (c);
+    c = 0;
+  }
+
   return c;
 }
 
 db::Net *
 SpiceNetlistBuilder::make_net (const std::string &name)
 {
   if (! mp_nets_by_name.get ()) {
@@ -1192,30 +1214,33 @@
       if (m_strict) {
         error (tl::sprintf (tl::to_string (tr ("Subcircuit '%s' not found in netlist")), model));
       } else {
         db::SpiceCachedCircuit *cc_nc = mp_dict->create_cached_circuit (model);
         cc_nc->set_anonymous (true);
         cc = cc_nc;
         std::vector<std::string> pins;
-        pins.resize (nn.size ());
+        pins.reserve (nn.size ());
+        for (size_t i = 0; i < nn.size (); ++i) {
+          pins.push_back (tl::to_string (i + 1));
+        }
         cc_nc->set_pins (pins);
       }
     }
 
     if (! cc->is_anonymous ()) {
       //  issue warnings on unknown parameters which are skipped otherwise
       for (auto p = pv.begin (); p != pv.end (); ++p) {
         if (cc->parameters ().find (p->first) == cc->parameters ().end ()) {
           warn (tl::sprintf (tl::to_string (tr ("Not a known parameter for circuit '%s': '%s'")), cc->name (), p->first));
         }
       }
     }
 
     if (cc->pin_count () != nn.size ()) {
-      error (tl::sprintf (tl::to_string (tr ("Pin count mismatch between circuit definition and circuit call: %d expected, got %d")), int (cc->pin_count ()), int (nets.size ())));
+      error (tl::sprintf (tl::to_string (tr ("Pin count mismatch between circuit definition and circuit call: %d expected, got %d (definition maybe implicit somewhere before)")), int (cc->pin_count ()), int (nets.size ())));
     }
 
     db::Circuit *c = build_circuit (cc, pv);
 
     db::SubCircuit *sc = new db::SubCircuit (c, name);
     mp_netlist_circuit->add_subcircuit (sc);
```

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReader.h` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReaderDelegate.cc` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReaderDelegate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReaderDelegate.h` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReaderDelegate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReaderExpressionParser.cc` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReaderExpressionParser.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceReaderExpressionParser.h` & `klayout-0.29.1/src/db/db/dbNetlistSpiceReaderExpressionParser.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceWriter.cc` & `klayout-0.29.1/src/db/db/dbNetlistSpiceWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistSpiceWriter.h` & `klayout-0.29.1/src/db/db/dbNetlistSpiceWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistUtils.h` & `klayout-0.29.1/src/db/db/dbNetlistUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistWriter.cc` & `klayout-0.29.1/src/db/db/dbNetlistWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbNetlistWriter.h` & `klayout-0.29.1/src/db/db/dbNetlistWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbObject.cc` & `klayout-0.29.1/src/db/db/dbObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbObject.h` & `klayout-0.29.1/src/db/db/dbObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbObjectTag.h` & `klayout-0.29.1/src/db/db/dbObjectTag.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbObjectWithProperties.h` & `klayout-0.29.1/src/db/db/dbObjectWithProperties.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerEdgePairs.cc` & `klayout-0.29.1/src/db/db/dbOriginalLayerEdgePairs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerEdgePairs.h` & `klayout-0.29.1/src/db/db/dbOriginalLayerEdgePairs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerEdges.cc` & `klayout-0.29.1/src/db/db/dbOriginalLayerEdges.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerEdges.h` & `klayout-0.29.1/src/db/db/dbOriginalLayerEdges.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerRegion.cc` & `klayout-0.29.1/src/db/db/dbOriginalLayerRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerRegion.h` & `klayout-0.29.1/src/db/db/dbOriginalLayerRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerTexts.cc` & `klayout-0.29.1/src/db/db/dbOriginalLayerTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbOriginalLayerTexts.h` & `klayout-0.29.1/src/db/db/dbOriginalLayerTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellDeclaration.cc` & `klayout-0.29.1/src/db/db/dbPCellDeclaration.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellDeclaration.h` & `klayout-0.29.1/src/db/db/dbPCellDeclaration.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellHeader.cc` & `klayout-0.29.1/src/db/db/dbPCellHeader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellHeader.h` & `klayout-0.29.1/src/db/db/dbPCellHeader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellVariant.cc` & `klayout-0.29.1/src/db/db/dbPCellVariant.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPCellVariant.h` & `klayout-0.29.1/src/db/db/dbPCellVariant.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPath.cc` & `klayout-0.29.1/src/db/db/dbPath.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPath.h` & `klayout-0.29.1/src/db/db/dbPath.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPin.cc` & `klayout-0.29.1/src/db/db/dbPin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPin.h` & `klayout-0.29.1/src/db/db/dbPin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPlugin.cc` & `klayout-0.29.1/src/db/db/dbPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPlugin.h` & `klayout-0.29.1/src/db/db/dbPlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPoint.cc` & `klayout-0.29.1/src/db/db/dbPoint.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPoint.h` & `klayout-0.29.1/src/db/db/dbPoint.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygon.cc` & `klayout-0.29.1/src/db/db/dbPolygon.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygon.h` & `klayout-0.29.1/src/db/db/dbPolygon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygonGenerators.cc` & `klayout-0.29.1/src/db/db/dbPolygonGenerators.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygonGenerators.h` & `klayout-0.29.1/src/db/db/dbPolygonGenerators.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygonTools.cc` & `klayout-0.29.1/src/db/db/dbPolygonTools.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPolygonTools.h` & `klayout-0.29.1/src/db/db/dbPolygonTools.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPropertiesRepository.cc` & `klayout-0.29.1/src/db/db/dbPropertiesRepository.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPropertiesRepository.h` & `klayout-0.29.1/src/db/db/dbPropertiesRepository.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbPropertyConstraint.h` & `klayout-0.29.1/src/db/db/dbPropertyConstraint.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbReader.cc` & `klayout-0.29.1/src/db/db/dbReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbReader.h` & `klayout-0.29.1/src/db/db/dbReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRecursiveInstanceIterator.cc` & `klayout-0.29.1/src/db/db/dbRecursiveInstanceIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRecursiveInstanceIterator.h` & `klayout-0.29.1/src/db/db/dbRecursiveInstanceIterator.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRecursiveShapeIterator.cc` & `klayout-0.29.1/src/db/db/dbRecursiveShapeIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRecursiveShapeIterator.h` & `klayout-0.29.1/src/db/db/dbRecursiveShapeIterator.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegion.cc` & `klayout-0.29.1/src/db/db/dbRegion.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegion.h` & `klayout-0.29.1/src/db/db/dbRegion.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionCheckUtils.cc` & `klayout-0.29.1/src/db/db/dbRegionCheckUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionCheckUtils.h` & `klayout-0.29.1/src/db/db/dbRegionCheckUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionDelegate.cc` & `klayout-0.29.1/src/db/db/dbRegionDelegate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionDelegate.h` & `klayout-0.29.1/src/db/db/dbRegionDelegate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionLocalOperations.cc` & `klayout-0.29.1/src/db/db/dbRegionLocalOperations.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionLocalOperations.h` & `klayout-0.29.1/src/db/db/dbRegionLocalOperations.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionProcessors.cc` & `klayout-0.29.1/src/db/db/dbRegionProcessors.cc`

 * *Files 17% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 namespace db
 {
 
 // -----------------------------------------------------------------------------------
 //  CornerDetectorCore implementation
 
-CornerDetectorCore::CornerDetectorCore (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
-  : m_checker (angle_start, include_angle_start, angle_end, include_angle_end)
+CornerDetectorCore::CornerDetectorCore (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
+  : m_checker (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute)
 {
   //  .. nothing yet ..
 }
 
 void CornerDetectorCore::detect_corners (const db::Polygon &poly, const CornerPointDelivery &delivery) const
 {
   size_t n = poly.holes () + 1;
@@ -342,8 +342,162 @@
       pts [i] = trans_inv * *t->vertex (i);
     }
     result.push_back (db::Polygon ());
     result.back ().assign_hull (pts + 0, pts + 3);
   }
 }
 
+// -----------------------------------------------------------------------------------
+//  DRCHullProcessor implementation
+
+DRCHullProcessor::DRCHullProcessor (db::Coord d, db::metrics_type metrics, size_t n_circle)
+  : m_d (d), m_metrics (metrics), m_n_circle (n_circle)
+{
+  //  .. nothing yet ..
+}
+
+static void create_edge_segment_euclidian (std::vector<db::Point> &points, const db::Edge &e, const db::Edge &ee, db::Coord dist, size_t n_circle)
+{
+  db::Vector d (e.d ());
+  db::Vector n (-d.y (), d.x ());
+
+  db::Vector dd (ee.d ());
+  db::Vector nn (-dd.y (), dd.x ());
+
+  if ((d.x () == 0 && d.y () == 0) || (dd.x () == 0 && dd.y () == 0)) {
+    //  should not happen
+    return;
+  }
+
+  double f = dist / n.double_length ();
+  double ff = dist / nn.double_length ();
+
+  points.push_back (e.p1 () + db::Vector (n * f));
+  points.push_back (e.p2 () + db::Vector (n * f));
+
+  if (db::vprod_sign (nn, n) < 0) {
+
+    //  concave corner
+    points.push_back (e.p2 ());
+    points.push_back (e.p2 () + db::Vector (nn * ff));
+
+  } else {
+
+    db::DVector dnn (nn);
+    db::DVector dn (n);
+    double amax;
+    if (db::vprod_sign (dnn, dn) == 0) {
+      amax = db::sprod_sign (dnn, dn) < 0 ? M_PI : 0.0;
+    } else {
+      amax = atan2 (db::vprod (dnn, dn), db::sprod (dnn, dn));
+    }
+
+    double da = M_PI * 2.0 / n_circle;
+    double f2 = f / cos (0.5 * da);
+
+    int na = int (floor (amax / da + db::epsilon));
+    double a0 = 0.5 * (amax - da * (na - 1));
+
+    for (int i = 0; i < na; ++i) {
+      double a = i * da + a0;
+      points.push_back (e.p2 () + db::Vector (d * (f2 * sin (a)) + n * (f2 * cos (a))));
+    }
+
+  }
+}
+
+static void create_edge_segment_square (std::vector<db::Point> &points, const db::Edge &e, db::Coord dist)
+{
+  db::Vector d (e.d ());
+  db::Vector n (-d.y (), d.x ());
+
+  if (d.x () == 0 && d.y () == 0) {
+    return;
+  }
+
+  double f = dist / n.double_length ();
+
+  points.push_back (e.p1 ());
+  points.push_back (e.p1 () + db::Vector (d * -f));
+  points.push_back (e.p1 () + db::Vector (d * -f + n * f));
+  points.push_back (e.p2 () + db::Vector (d * f + n * f));
+  points.push_back (e.p2 () + db::Vector (d * f));
+}
+
+static void create_edge_segment_projection (std::vector<db::Point> &points, const db::Edge &e, db::Coord dist)
+{
+  db::Vector d (e.d ());
+  db::Vector n (-d.y (), d.x ());
+
+  if (d.x () == 0 && d.y () == 0) {
+    return;
+  }
+
+  double f = dist / n.double_length ();
+
+  points.push_back (e.p1 ());
+  points.push_back (e.p1 () + db::Vector (n * f));
+  points.push_back (e.p2 () + db::Vector (n * f));
+}
+
+static void create_edge_segment (std::vector<db::Point> &points, db::metrics_type metrics, const db::Edge &e, const db::Edge &ee, db::Coord d, size_t n_circle)
+{
+  if (metrics == db::Euclidian) {
+    create_edge_segment_euclidian (points, e, ee, d, n_circle);
+  } else if (metrics == db::Square) {
+    create_edge_segment_square (points, e, d);
+  } else if (metrics == db::Projection) {
+    create_edge_segment_projection (points, e, d);
+  }
+}
+
+void
+DRCHullProcessor::process (const db::Polygon &poly, std::vector<db::Polygon> &result) const
+{
+  db::EdgeProcessor ep;
+  std::vector<db::Point> points;
+
+  for (unsigned int i = 0; i < poly.holes () + 1; ++i) {
+
+    points.clear ();
+
+    auto c = poly.contour (i);
+    if (c.size () < 2) {
+      continue;
+    }
+
+    for (auto p = c.begin (); p != c.end (); ++p) {
+
+      auto pp = p;
+      if (++pp == c.end ()) {
+        pp = c.begin ();
+      }
+
+      auto ppp = pp;
+      if (++ppp == c.end ()) {
+        ppp = c.begin ();
+      }
+
+      create_edge_segment (points, m_metrics, db::Edge (*p, *pp), db::Edge (*pp, *ppp), m_d, m_n_circle);
+
+    }
+
+    for (auto p = points.begin (); p != points.end (); ++p) {
+
+      auto pp = p;
+      if (++ pp == points.end ()) {
+        pp = points.begin ();
+      }
+
+      ep.insert (db::Edge (*p, *pp));
+
+    }
+
+  }
+
+  db::SimpleMerge op;
+  db::PolygonContainer psink (result);
+  db::PolygonGenerator pg (psink, false);
+  ep.process (pg, op);
+}
+
 }
```

### Comparing `klayout-0.29.0/src/db/db/dbRegionProcessors.h` & `klayout-0.29.1/src/db/db/dbRegionProcessors.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 #define HDR_dbRegionProcessors
 
 #include "dbCommon.h"
 #include "dbRegionDelegate.h"
 #include "dbPolygonTools.h"
 #include "dbEdgesUtils.h"
 #include "dbTriangles.h"
+#include "dbEdgePairRelations.h"
 
 namespace db
 {
 
 // -----------------------------------------------------------------------------------
 //  Corner detection
 
@@ -109,15 +110,15 @@
 
 /**
  *  @brief A helper class implementing the core corner detection algorithm
  */
 class DB_PUBLIC CornerDetectorCore
 {
 public:
-  CornerDetectorCore (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end);
+  CornerDetectorCore (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute);
   virtual ~CornerDetectorCore () { }
 
   void detect_corners (const db::Polygon &poly, const CornerPointDelivery &delivery) const;
 
 private:
   db::EdgeAngleChecker m_checker;
 };
@@ -125,16 +126,16 @@
 /**
  *  @brief A corner detector delivering small retangles (2*dim x 2*dim) per detected corner
  */
 class DB_PUBLIC CornersAsRectangles
   : public db::PolygonProcessorBase, private CornerDetectorCore
 {
 public:
-  CornersAsRectangles (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, db::Coord dim = 1)
-    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end), m_dim (dim)
+  CornersAsRectangles (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute, db::Coord dim = 1)
+    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute), m_dim (dim)
   {
     //  .. nothing yet ..
   }
 
   void process (const db::Polygon &poly, std::vector<db::Polygon> &result) const
   {
     detect_corners (poly, CornerRectDelivery (m_dim, result));
@@ -154,16 +155,16 @@
 /**
  *  @brief A corner detector delivering degenerated edges (dots) for the corners
  */
 class DB_PUBLIC CornersAsDots
   : public db::PolygonToEdgeProcessorBase, private CornerDetectorCore
 {
 public:
-  CornersAsDots (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
-    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end)
+  CornersAsDots (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
+    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute)
   {
     //  .. nothing yet ..
   }
 
   void process (const db::Polygon &poly, std::vector<db::Edge> &result) const
   {
     detect_corners (poly, CornerDotDelivery (result));
@@ -179,16 +180,16 @@
 /**
  *  @brief A corner detector delivering edge pairs for the corners
  */
 class DB_PUBLIC CornersAsEdgePairs
   : public db::PolygonToEdgePairProcessorBase, private CornerDetectorCore
 {
 public:
-  CornersAsEdgePairs (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
-    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end)
+  CornersAsEdgePairs (double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
+    : CornerDetectorCore (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute)
   {
     //  .. nothing yet ..
   }
 
   void process (const db::Polygon &poly, std::vector<db::EdgePair> &result) const
   {
     detect_corners (poly, CornerEdgePairDelivery (result));
@@ -460,10 +461,28 @@
   virtual bool wants_variants () const { return true; }
 
 private:
   K m_q;
   db::MagnificationAndOrientationReducer m_vars;
 };
 
+/**
+ *  @brief Computes DRC hulls for DRC space visualization
+ */
+class DB_PUBLIC_TEMPLATE DRCHullProcessor
+  : public db::PolygonProcessorBase
+{
+public:
+  DRCHullProcessor (db::Coord d, db::metrics_type metrics, size_t n_circle = 64);
+
+  void process (const db::Polygon &poly, std::vector<db::Polygon> &result) const;
+
+private:
+  db::Coord m_d;
+  db::metrics_type m_metrics;
+  size_t m_n_circle;
+};
+
+
 }
 
 #endif
```

### Comparing `klayout-0.29.0/src/db/db/dbRegionUtils.cc` & `klayout-0.29.1/src/db/db/dbRegionUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbRegionUtils.h` & `klayout-0.29.1/src/db/db/dbRegionUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbSaveLayoutOptions.cc` & `klayout-0.29.1/src/db/db/dbSaveLayoutOptions.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbSaveLayoutOptions.h` & `klayout-0.29.1/src/db/db/dbSaveLayoutOptions.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShape.cc` & `klayout-0.29.1/src/db/db/dbShape.cc`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 */
 
 
 #include "dbShape.h"
 #include "dbBoxConvert.h"
 #include "dbPolygonTools.h"
+#include "dbHash.h"
 #include "tlCpp.h"
 
 namespace db
 {
 
 static NO_RETURN void raise_no_path ()
 {
@@ -858,14 +859,32 @@
   default:
     break;
   }
 
   return box_type ();
 }
 
+size_t
+Shape::hash_value () const
+{
+  size_t h = size_t (m_type);
+  h = std::hcombine (h, std::hfunc (m_trans));
+
+  if (m_stable) {
+    //  Use the bytes of the iterator binary pattern (see operator<)
+    for (unsigned int i = 0; i < sizeof (tl::reuse_vector<box_type>::const_iterator); ++i) {
+      h = std::hcombine (h, size_t (m_generic.iter[i]));
+    }
+  } else {
+    h = std::hcombine (h, size_t (m_generic.any));
+  }
+
+  return h;
+}
+
 std::string
 Shape::to_string () const
 {
   std::string r; 
 
   switch (m_type) {
   case Null:
```

### Comparing `klayout-0.29.0/src/db/db/dbShape.h` & `klayout-0.29.1/src/db/db/dbShape.h`

 * *Files 0% similar despite different names*

```diff
@@ -2765,14 +2765,19 @@
       if (m_generic.any != d.m_generic.any) {
         return m_generic.any < d.m_generic.any;
       }
     }
     return m_trans < d.m_trans;
   }
 
+  /**
+   *  @brief Hash value
+   */
+  size_t hash_value () const;
+
   /** 
    *  @brief Convert to a string
    */
   std::string to_string () const;
 
 public:
   friend class db::Shapes;
@@ -2833,10 +2838,25 @@
   trans_type m_trans;
   bool m_with_props : 8;
   bool m_stable : 8;
   object_type m_type : 16;
 };
 
 }  // namespace db
+
+namespace std
+{
+
+  //  provide a template specialization for std::hash<T>
+  template <>
+  struct hash <db::Shape>
+  {
+    size_t operator() (const db::Shape &s) const
+    {
+      return s.hash_value ();
+    }
+  };
+
+}  // namespace std
   
 #endif
```

### Comparing `klayout-0.29.0/src/db/db/dbShapeCollection.cc` & `klayout-0.29.1/src/db/db/dbShapeCollection.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeCollection.h` & `klayout-0.29.1/src/db/db/dbShapeCollection.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeCollectionUtils.cc` & `klayout-0.29.1/src/db/db/dbShapeCollectionUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeCollectionUtils.h` & `klayout-0.29.1/src/db/db/dbShapeCollectionUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeFlags.cc` & `klayout-0.29.1/src/db/db/dbShapeFlags.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeFlags.h` & `klayout-0.29.1/src/db/db/dbShapeFlags.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeIterator.cc` & `klayout-0.29.1/src/db/db/dbShapeIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeProcessor.cc` & `klayout-0.29.1/src/db/db/dbShapeProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeProcessor.h` & `klayout-0.29.1/src/db/db/dbShapeProcessor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapeRepository.h` & `klayout-0.29.1/src/db/db/dbShapeRepository.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapes.cc` & `klayout-0.29.1/src/db/db/dbShapes.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapes.h` & `klayout-0.29.1/src/db/db/dbShapes.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapes2.cc` & `klayout-0.29.1/src/db/db/dbShapes2.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapes2.h` & `klayout-0.29.1/src/db/db/dbShapes2.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbShapes3.cc` & `klayout-0.29.1/src/db/db/dbShapes3.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStatic.cc` & `klayout-0.29.1/src/db/db/dbStatic.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStatic.h` & `klayout-0.29.1/src/db/db/dbStatic.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStream.cc` & `klayout-0.29.1/src/db/db/dbStream.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStream.h` & `klayout-0.29.1/src/db/db/dbStream.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStreamLayers.cc` & `klayout-0.29.1/src/db/db/dbStreamLayers.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbStreamLayers.h` & `klayout-0.29.1/src/db/db/dbStreamLayers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbSubCircuit.cc` & `klayout-0.29.1/src/db/db/dbSubCircuit.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbSubCircuit.h` & `klayout-0.29.1/src/db/db/dbSubCircuit.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTechnology.cc` & `klayout-0.29.1/src/db/db/dbTechnology.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTechnology.h` & `klayout-0.29.1/src/db/db/dbTechnology.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTestSupport.cc` & `klayout-0.29.1/src/db/db/dbTestSupport.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTestSupport.h` & `klayout-0.29.1/src/db/db/dbTestSupport.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbText.cc` & `klayout-0.29.1/src/db/db/dbText.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbText.h` & `klayout-0.29.1/src/db/db/dbText.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextWriter.cc` & `klayout-0.29.1/src/db/db/dbTextWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextWriter.h` & `klayout-0.29.1/src/db/db/dbTextWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTexts.cc` & `klayout-0.29.1/src/db/db/dbTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTexts.h` & `klayout-0.29.1/src/db/db/dbTexts.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextsDelegate.cc` & `klayout-0.29.1/src/db/db/dbTextsDelegate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextsDelegate.h` & `klayout-0.29.1/src/db/db/dbTextsDelegate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextsUtils.cc` & `klayout-0.29.1/src/db/db/dbTextsUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTextsUtils.h` & `klayout-0.29.1/src/db/db/dbTextsUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTilingProcessor.cc` & `klayout-0.29.1/src/db/db/dbTilingProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTilingProcessor.h` & `klayout-0.29.1/src/db/db/dbTilingProcessor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTrans.cc` & `klayout-0.29.1/src/db/db/dbTrans.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTrans.h` & `klayout-0.29.1/src/db/db/dbTrans.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTriangle.cc` & `klayout-0.29.1/src/db/db/dbTriangle.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTriangle.h` & `klayout-0.29.1/src/db/db/dbTriangle.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTriangles.cc` & `klayout-0.29.1/src/db/db/dbTriangles.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTriangles.h` & `klayout-0.29.1/src/db/db/dbTriangles.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbTypes.h` & `klayout-0.29.1/src/db/db/dbTypes.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbUserObject.cc` & `klayout-0.29.1/src/db/db/dbUserObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbUserObject.h` & `klayout-0.29.1/src/db/db/dbUserObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbUtils.cc` & `klayout-0.29.1/src/db/db/dbUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbUtils.h` & `klayout-0.29.1/src/db/db/dbUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbVariableWidthPath.cc` & `klayout-0.29.1/src/db/db/dbVariableWidthPath.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbVariableWidthPath.h` & `klayout-0.29.1/src/db/db/dbVariableWidthPath.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbVector.cc` & `klayout-0.29.1/src/db/db/dbVector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbVector.h` & `klayout-0.29.1/src/db/db/dbVector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbWriter.cc` & `klayout-0.29.1/src/db/db/dbWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbWriter.h` & `klayout-0.29.1/src/db/db/dbWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbWriterTools.cc` & `klayout-0.29.1/src/db/db/dbWriterTools.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/dbWriterTools.h` & `klayout-0.29.1/src/db/db/dbWriterTools.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/fonts.cc_gen` & `klayout-0.29.1/src/db/db/fonts.cc_gen`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/glyphs.cc_gen` & `klayout-0.29.1/src/db/db/glyphs.cc_gen`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbBox.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbBox.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbCell.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbCell.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbCellMapping.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbCellMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbCommonStreamOptions.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbCommonStreamOptions.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbCompoundOperation.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbCompoundOperation.cc`

 * *Files 2% similar despite different names*

```diff
@@ -210,30 +210,30 @@
 }
 
 static db::CompoundRegionOperationNode *new_count_filter (db::CompoundRegionOperationNode *input, bool invert, size_t min_count, size_t max_count)
 {
   return new db::CompoundRegionCountFilterNode (input, invert, min_count, max_count);
 }
 
-static db::CompoundRegionOperationNode *new_corners_as_rectangles (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, db::Coord dim = 1)
+static db::CompoundRegionOperationNode *new_corners_as_rectangles (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, db::Coord dim, bool inverse, bool absolute)
 {
   check_non_null (input, "input");
-  return new db::CompoundRegionProcessingOperationNode (new db::CornersAsRectangles (angle_start, include_angle_start, angle_end, include_angle_end, dim), input, true /*processor is owned*/, dim /*dist adder*/);
+  return new db::CompoundRegionProcessingOperationNode (new db::CornersAsRectangles (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute, dim), input, true /*processor is owned*/, dim /*dist adder*/);
 }
 
-static db::CompoundRegionOperationNode *new_corners_as_dots (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
+static db::CompoundRegionOperationNode *new_corners_as_dots (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
 {
   check_non_null (input, "input");
-  return new db::CompoundRegionToEdgeProcessingOperationNode (new db::CornersAsDots (angle_start, include_angle_start, angle_end, include_angle_end), input, true /*processor is owned*/);
+  return new db::CompoundRegionToEdgeProcessingOperationNode (new db::CornersAsDots (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute), input, true /*processor is owned*/);
 }
 
-static db::CompoundRegionOperationNode *new_corners_as_edge_pairs (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end)
+static db::CompoundRegionOperationNode *new_corners_as_edge_pairs (db::CompoundRegionOperationNode *input, double angle_start, bool include_angle_start, double angle_end, bool include_angle_end, bool inverse, bool absolute)
 {
   check_non_null (input, "input");
-  return new db::CompoundRegionToEdgePairProcessingOperationNode (new db::CornersAsEdgePairs (angle_start, include_angle_start, angle_end, include_angle_end), input, true /*processor is owned*/);
+  return new db::CompoundRegionToEdgePairProcessingOperationNode (new db::CornersAsEdgePairs (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute), input, true /*processor is owned*/);
 }
 
 static db::CompoundRegionOperationNode *new_extents (db::CompoundRegionOperationNode *input, db::Coord e)
 {
   check_non_null (input, "input");
   if (input->result_type () == db::CompoundRegionOperationNode::EdgePairs) {
     return new db::CompoundRegionEdgePairToPolygonProcessingOperationNode (new db::extents_processor<db::EdgePair> (e, e), input, true /*processor is owned*/);
@@ -337,18 +337,18 @@
 
 static db::CompoundRegionOperationNode *new_edge_length_sum_filter (db::CompoundRegionOperationNode *input, bool inverse, db::Edge::distance_type lmin, db::Edge::distance_type lmax)
 {
   check_non_null (input, "input");
   return new db::CompoundRegionEdgeFilterOperationNode (new db::EdgeLengthFilter (lmin, lmax, inverse), input, true /*processor is owned*/, true /*sum*/);
 }
 
-static db::CompoundRegionOperationNode *new_edge_orientation_filter (db::CompoundRegionOperationNode *input, bool inverse, double amin, bool include_amin, double amax, bool include_amax)
+static db::CompoundRegionOperationNode *new_edge_orientation_filter (db::CompoundRegionOperationNode *input, bool inverse, double amin, bool include_amin, double amax, bool include_amax, bool absolute_angle)
 {
   check_non_null (input, "input");
-  return new db::CompoundRegionEdgeFilterOperationNode (new db::EdgeOrientationFilter (amin, include_amin, amax, include_amax, inverse), input, true /*processor is owned*/);
+  return new db::CompoundRegionEdgeFilterOperationNode (new db::EdgeOrientationFilter (amin, include_amin, amax, include_amax, inverse, absolute_angle), input, true /*processor is owned*/);
 }
 
 static db::CompoundRegionOperationNode *new_polygons (db::CompoundRegionOperationNode *input, db::Coord e)
 {
   check_non_null (input, "input");
   if (input->result_type () == db::CompoundRegionOperationNode::EdgePairs) {
     return new db::CompoundRegionEdgePairToPolygonProcessingOperationNode (new db::EdgePairToPolygonProcessor (e), input, true /*processor is owned*/);
@@ -613,25 +613,29 @@
     "element is taken as the default result. The implementation will evaluate c1 and if not empty, will render r1. Otherwise, c2 will be evaluated and r2 "
     "rendered if c2 isn't empty etc. If none of the conditions renders a non-empty set and a default result is present, the default will be "
     "returned. Otherwise, the result is empty."
   ) +
   gsi::constructor ("new_count_filter", &new_count_filter, gsi::arg ("inputs"), gsi::arg ("invert", false), gsi::arg ("min_count", size_t (0)), gsi::arg ("max_count", std::numeric_limits<size_t>::max ()),
     "@brief Creates a node selecting results but their shape count.\n"
   ) +
-  gsi::constructor ("new_corners_as_rectangles", &new_corners_as_rectangles, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"), gsi::arg ("dim"),
+  gsi::constructor ("new_corners_as_rectangles", &new_corners_as_rectangles, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"), gsi::arg ("dim"), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief Creates a node turning corners into rectangles.\n"
+    "\n"
+    "'absolute' and 'inverse' arguments have been added in version 0.29.1.\n"
   ) +
-  gsi::constructor ("new_corners_as_dots", &new_corners_as_dots, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"),
+  gsi::constructor ("new_corners_as_dots", &new_corners_as_dots, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief Creates a node turning corners into dots (single-point edges).\n"
+    "\n"
+    "'absolute' and 'inverse' arguments have been added in version 0.29.1.\n"
   ) +
-  gsi::constructor ("new_corners_as_edge_pairs", &new_corners_as_edge_pairs, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"),
+  gsi::constructor ("new_corners_as_edge_pairs", &new_corners_as_edge_pairs, gsi::arg ("input"), gsi::arg ("angle_min"), gsi::arg ("include_angle_min"), gsi::arg ("angle_max"), gsi::arg ("include_angle_max"), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief Creates a node turning corners into edge pairs containing the two edges adjacent to the corner.\n"
     "The first edge will be the incoming edge and the second one the outgoing edge.\n"
     "\n"
-    "This feature has been introduced in version 0.27.1.\n"
+    "This feature has been introduced in version 0.27.1. 'absolute' and 'inverse' arguments have been added in version 0.29.1.\n"
   ) +
   gsi::constructor ("new_extents", &new_extents, gsi::arg ("input"), gsi::arg ("e", 0),
     "@brief Creates a node returning the extents of the objects.\n"
     "The 'e' parameter provides a generic enlargement which is applied to the boxes. This is helpful to cover dot-like edges or edge pairs in the input."
   ) +
   gsi::constructor ("new_relative_extents", &new_relative_extents, gsi::arg ("input"), gsi::arg ("fx1"), gsi::arg ("fy1"), gsi::arg ("fx2"), gsi::arg ("fy2"), gsi::arg ("dx"), gsi::arg ("dy"),
     "@brief Creates a node returning markers at specified locations of the extent (e.g. at the center).\n"
@@ -755,16 +759,18 @@
   ) +
   gsi::constructor ("new_edge_length_filter", &new_edge_length_filter, gsi::arg ("input"), gsi::arg ("inverse", false), gsi::arg ("lmin", 0), gsi::arg ("lmax", std::numeric_limits<db::Edge::distance_type>::max (), "max"),
     "@brief Creates a node filtering edges by their length.\n"
   ) +
   gsi::constructor ("new_edge_length_sum_filter", &new_edge_length_sum_filter, gsi::arg ("input"), gsi::arg ("inverse", false), gsi::arg ("lmin", 0), gsi::arg ("lmax", std::numeric_limits<db::Edge::distance_type>::max (), "max"),
     "@brief Creates a node filtering edges by their length sum (over the local set).\n"
   ) +
-  gsi::constructor ("new_edge_orientation_filter", &new_edge_orientation_filter, gsi::arg ("input"), gsi::arg ("inverse"), gsi::arg ("amin"), gsi::arg ("include_amin"), gsi::arg ("amax"), gsi::arg ("include_amax"),
+  gsi::constructor ("new_edge_orientation_filter", &new_edge_orientation_filter, gsi::arg ("input"), gsi::arg ("inverse"), gsi::arg ("amin"), gsi::arg ("include_amin"), gsi::arg ("amax"), gsi::arg ("include_amax"), gsi::arg ("absolute_angle", false),
     "@brief Creates a node filtering edges by their orientation.\n"
+    "\n"
+    "'absolute_angle' has been introduced in version 0.29.1."
   ) +
   gsi::constructor ("new_polygons", &new_polygons, gsi::arg ("input"), gsi::arg ("e", 0),
     "@brief Creates a node converting the input to polygons.\n"
     "@param e The enlargement parameter when converting edges or edge pairs to polygons.\n"
   ) +
   gsi::constructor ("new_edge_pair_to_first_edges", &new_edge_pair_to_first_edges, gsi::arg ("input"),
     "@brief Creates a node delivering the first edge of each edges pair.\n"
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbContainerHelpers.h` & `klayout-0.29.1/src/db/db/gsiDeclDbContainerHelpers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbDeepShapeStore.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbDeepShapeStore.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbEdge.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbEdge.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbEdgePair.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbEdgePair.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbEdgePairs.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbEdgePairs.cc`

 * *Files 2% similar despite different names*

```diff
@@ -428,43 +428,71 @@
   db::EdgeLengthFilter f (min.is_nil () ? db::Edges::distance_type (0) : min.to<db::Edges::distance_type> (), max.is_nil () ? std::numeric_limits <db::Edges::distance_type>::max () : max.to<db::Edges::distance_type> (), inverse);
   db::EdgeFilterBasedEdgePairFilter ef (&f, false /*both must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle1 (const db::EdgePairs *r, double a, bool inverse)
 {
-  db::EdgeOrientationFilter f (a, inverse);
+  db::EdgeOrientationFilter f (a, inverse, false);
   db::EdgeFilterBasedEdgePairFilter ef (&f, true /*one must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle2 (const db::EdgePairs *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
 {
-  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse);
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, false);
+  db::EdgeFilterBasedEdgePairFilter ef (&f, true /*one must match*/);
+  return r->filtered (ef);
+}
+
+static db::EdgePairs with_abs_angle1 (const db::EdgePairs *r, double a, bool inverse)
+{
+  db::EdgeOrientationFilter f (a, inverse, true);
+  db::EdgeFilterBasedEdgePairFilter ef (&f, true /*one must match*/);
+  return r->filtered (ef);
+}
+
+static db::EdgePairs with_abs_angle2 (const db::EdgePairs *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
+{
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, true);
   db::EdgeFilterBasedEdgePairFilter ef (&f, true /*one must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle3 (const db::EdgePairs *r, db::SpecialEdgeOrientationFilter::FilterType type, bool inverse)
 {
   db::SpecialEdgeOrientationFilter f (type, inverse);
   db::EdgeFilterBasedEdgePairFilter ef (&f, true /*one must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle_both1 (const db::EdgePairs *r, double a, bool inverse)
 {
-  db::EdgeOrientationFilter f (a, inverse);
+  db::EdgeOrientationFilter f (a, inverse, false);
   db::EdgeFilterBasedEdgePairFilter ef (&f, false /*both must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle_both2 (const db::EdgePairs *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
 {
-  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse);
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, false);
+  db::EdgeFilterBasedEdgePairFilter ef (&f, false /*both must match*/);
+  return r->filtered (ef);
+}
+
+static db::EdgePairs with_abs_angle_both1 (const db::EdgePairs *r, double a, bool inverse)
+{
+  db::EdgeOrientationFilter f (a, inverse, true);
+  db::EdgeFilterBasedEdgePairFilter ef (&f, false /*both must match*/);
+  return r->filtered (ef);
+}
+
+static db::EdgePairs with_abs_angle_both2 (const db::EdgePairs *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
+{
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, true);
   db::EdgeFilterBasedEdgePairFilter ef (&f, false /*both must match*/);
   return r->filtered (ef);
 }
 
 static db::EdgePairs with_angle_both3 (const db::EdgePairs *r, db::SpecialEdgeOrientationFilter::FilterType type, bool inverse)
 {
   db::SpecialEdgeOrientationFilter f (type, inverse);
@@ -963,14 +991,30 @@
     "@code\n"
     "result = edge_pairs.with_angle(0, 45, false)\n"
     "others = edge_pairs.with_angle_both(0, 45, true)\n"
     "@/code\n"
     "\n"
     "This method has been added in version 0.27.1.\n"
   ) +
+  method_ext ("with_abs_angle", with_abs_angle1, gsi::arg ("angle"), gsi::arg ("inverse"),
+    "@brief Filter the edge pairs by orientation of their edges\n"
+    "\n"
+    "This method behaves like \\with_angle, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
+  ) +
+  method_ext ("with_abs_angle", with_abs_angle2, gsi::arg ("min_angle"), gsi::arg ("max_angle"), gsi::arg ("inverse"), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", false),
+    "@brief Filter the edge pairs by orientation of their edges\n"
+    "\n"
+    "This method behaves like \\with_angle, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
+  ) +
   method_ext ("with_angle", with_angle3, gsi::arg ("type"), gsi::arg ("inverse"),
     "@brief Filter the edge pairs by orientation of their edges\n"
     "Filters the edge pairs in the edge pair collection by orientation. If \"inverse\" is false, only "
     "edge pairs with at least one edge having an angle of the given type are returned. If \"inverse\" is true, "
     "edge pairs not fulfilling this criterion are returned.\n"
     "\n"
     "This version allows specifying an edge type instead of an angle. Edge types include multiple distinct orientations "
@@ -1023,14 +1067,29 @@
     "@code\n"
     "result = edge_pairs.with_angle_both(0, 45, false)\n"
     "others = edge_pairs.with_angle(0, 45, true)\n"
     "@/code\n"
     "\n"
     "This method has been added in version 0.27.1.\n"
   ) +
+  method_ext ("with_abs_angle_both", with_abs_angle_both1, gsi::arg ("angle"), gsi::arg ("inverse"),
+    "@brief Filter the edge pairs by orientation of both of their edges\n"
+    "\n"
+    "This method behaves like \\with_angle_both, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
+  ) +
+  method_ext ("with_abs_angle_both", with_abs_angle_both2, gsi::arg ("min_angle"), gsi::arg ("max_angle"), gsi::arg ("inverse"), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", false),
+    "\n"
+    "This method behaves like \\with_angle_both, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
+  ) +
   method_ext ("with_angle_both", with_angle_both3, gsi::arg ("type"), gsi::arg ("inverse"),
     "@brief Filter the edge pairs by orientation of their edges\n"
     "Filters the edge pairs in the edge pair collection by orientation. If \"inverse\" is false, only "
     "edge pairs with both edges having an angle of the given type are returned. If \"inverse\" is true, "
     "edge pairs not fulfilling this criterion for both edges are returned.\n"
     "\n"
     "This version allows specifying an edge type instead of an angle. Edge types include multiple distinct orientations "
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbEdgeProcessor.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbEdgeProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbEdges.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbEdges.cc`

 * *Files 1% similar despite different names*

```diff
@@ -436,21 +436,33 @@
 {
   db::EdgeLengthFilter f (min.is_nil () ? db::Edges::distance_type (0) : min.to<db::Edges::distance_type> (), max.is_nil () ? std::numeric_limits <db::Edges::distance_type>::max () : max.to<db::Edges::distance_type> (), inverse);
   return r->filtered (f);
 }
 
 static db::Edges with_angle1 (const db::Edges *r, double a, bool inverse)
 {
-  db::EdgeOrientationFilter f (a, inverse);
+  db::EdgeOrientationFilter f (a, inverse, false);
   return r->filtered (f);
 }
 
 static db::Edges with_angle2 (const db::Edges *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
 {
-  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse);
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, false);
+  return r->filtered (f);
+}
+
+static db::Edges with_abs_angle1 (const db::Edges *r, double a, bool inverse)
+{
+  db::EdgeOrientationFilter f (a, inverse, true);
+  return r->filtered (f);
+}
+
+static db::Edges with_abs_angle2 (const db::Edges *r, double amin, double amax, bool inverse, bool include_amin, bool include_amax)
+{
+  db::EdgeOrientationFilter f (amin, include_amin, amax, include_amax, inverse, true);
   return r->filtered (f);
 }
 
 static db::Edges with_angle3 (const db::Edges *r, db::SpecialEdgeOrientationFilter::FilterType type, bool inverse)
 {
   db::SpecialEdgeOrientationFilter f (type, inverse);
   return r->filtered (f);
@@ -919,15 +931,31 @@
     "edges which have an angle to the x-axis larger or equal to \"min_angle\" (depending on \"include_min_angle\") and equal or less than \"max_angle\" (depending on \"include_max_angle\") are "
     "returned. If \"inverse\" is true, "
     "edges which do not conform to this criterion are returned.\n"
     "\n"
     "With \"include_min_angle\" set to true (the default), the minimum angle is included in the criterion while with false, the "
     "minimum angle itself is not included. Same for \"include_max_angle\" where the default is false, meaning the maximum angle is not included in the range.\n"
     "\n"
-    "The two \"include..\" arguments have been added in version 0.27."
+    "The two \"include..\" arguments have been added in version 0.27.\n"
+  ) +
+  method_ext ("with_abs_angle", with_abs_angle1, gsi::arg ("angle"), gsi::arg ("inverse"),
+    "@brief Filter the edges by orientation\n"
+    "\n"
+    "This method behaves like \\with_angle, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
+  ) +
+  method_ext ("with_abs_angle", with_abs_angle2, gsi::arg ("min_angle"), gsi::arg ("max_angle"), gsi::arg ("inverse"), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", false),
+    "@brief Filter the edges by orientation\n"
+    "\n"
+    "This method behaves like \\with_angle, but angles are always positive - i.e. there is no "
+    "differentiation between edges sloping 'down' vs. edges sloping 'up.\n"
+    "\n"
+    "This method has been added in version 0.29.1.\n"
   ) +
   method_ext ("with_angle", with_angle3, gsi::arg ("type"), gsi::arg ("inverse"),
     "@brief Filters the edges by orientation type\n"
     "Filters the edges in the edge collection by orientation. If \"inverse\" is false, only "
     "edges which have an angle of the given type are returned. If \"inverse\" is true, "
     "edges which do not conform to this criterion are returned.\n"
     "\n"
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbGlyphs.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbGlyphs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbHelpers.h` & `klayout-0.29.1/src/db/db/gsiDeclDbHelpers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbHierNetworkProcessor.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbHierNetworkProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbInstElement.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbInstElement.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayerMapping.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayerMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayout.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayout.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayoutDiff.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayoutDiff.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayoutQuery.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayoutQuery.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayoutToNetlist.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayoutToNetlist.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayoutUtils.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayoutUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLayoutVsSchematic.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLayoutVsSchematic.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLibrary.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLibrary.cc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -214,20 +214,20 @@
     "@brief Additionally associates the library with the given technology.\n"
     "See also \\clear_technologies.\n"
     "\n"
     "This method has been introduced in version 0.27"
   ) +
   gsi::method ("is_for_technology", &db::Library::is_for_technology, gsi::arg ("tech"),
     "@brief Returns a value indicating whether the library is associated with the given technology.\n"
+    "The method is equivalent to checking whether the \\technologies list is empty.\n"
+    "\n"
     "This method has been introduced in version 0.27"
   ) +
   gsi::method ("for_technologies", &db::Library::for_technologies,
     "@brief Returns a value indicating whether the library is associated with any technology.\n"
-    "The method is equivalent to checking whether the \\technologies list is empty.\n"
-    "\n"
     "This method has been introduced in version 0.27"
   ) +
   gsi::method ("technologies", &db::Library::get_technologies,
     "@brief Gets the list of technologies this library is associated with.\n"
     "This method has been introduced in version 0.27"
   ) +
   gsi::method ("layout_const", (const db::Layout &(db::Library::*)() const) &db::Library::layout,
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbLog.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbLog.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbManager.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbManager.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbMatrix.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbMatrix.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbMetaInfo.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbMetaInfo.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbMetaInfo.h` & `klayout-0.29.1/src/db/db/gsiDeclDbMetaInfo.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbNetlist.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbNetlist.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbNetlistCompare.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbNetlistCompare.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbNetlistCrossReference.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbNetlistCrossReference.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbNetlistDeviceClasses.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbNetlistDeviceClasses.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbNetlistDeviceExtractor.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbNetlistDeviceExtractor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbPath.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbPath.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbPoint.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbPoint.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbPolygon.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbPolygon.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbReader.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbRecursiveInstanceIterator.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbRecursiveInstanceIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbRecursiveShapeIterator.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbRecursiveShapeIterator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbRegion.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbRegion.cc`

 * *Files 0% similar despite different names*

```diff
@@ -296,27 +296,27 @@
 }
 
 static db::Region *texts_as_boxes2 (const db::Region *r, db::DeepShapeStore &dss, const std::string &pat, bool pattern, db::Coord enl)
 {
   return new db::Region (r->texts_as_boxes (pat, pattern, enl, dss));
 }
 
-static db::Edges corners_to_dots (const db::Region *r, double angle_start, double angle_end, bool include_angle_start, bool include_angle_end)
+static db::Edges corners_to_dots (const db::Region *r, double angle_start, double angle_end, bool include_angle_start, bool include_angle_end, bool inverse, bool absolute)
 {
-  return r->processed (db::CornersAsDots (angle_start, include_angle_start, angle_end, include_angle_end));
+  return r->processed (db::CornersAsDots (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute));
 }
 
-static db::Region corners_to_boxes (const db::Region *r, double angle_start, double angle_end, db::Coord dim, bool include_angle_start, bool include_angle_end)
+static db::Region corners_to_boxes (const db::Region *r, double angle_start, double angle_end, db::Coord dim, bool include_angle_start, bool include_angle_end, bool inverse, bool absolute)
 {
-  return r->processed (db::CornersAsRectangles (angle_start, include_angle_start, angle_end, include_angle_end, dim));
+  return r->processed (db::CornersAsRectangles (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute, dim));
 }
 
-static db::EdgePairs corners_to_edge_pairs (const db::Region *r, double angle_start, double angle_end, bool include_angle_start, bool include_angle_end)
+static db::EdgePairs corners_to_edge_pairs (const db::Region *r, double angle_start, double angle_end, bool include_angle_start, bool include_angle_end, bool inverse, bool absolute)
 {
-  return r->processed (db::CornersAsEdgePairs (angle_start, include_angle_start, angle_end, include_angle_end));
+  return r->processed (db::CornersAsEdgePairs (angle_start, include_angle_start, angle_end, include_angle_end, inverse, absolute));
 }
 
 static db::Region *new_si (const db::RecursiveShapeIterator &si)
 {
   return new db::Region (si);
 }
 
@@ -432,14 +432,19 @@
 {
   db::TriangulationProcessor tri (max_area, min_b);
   db::Region res = r->processed (tri);
   res.set_merged_semantics (false);
   return res;
 }
 
+static db::Region drc_hull (const db::Region *r, db::metrics_type metrics, db::Coord space, size_t n_circle)
+{
+  return r->processed (db::DRCHullProcessor (space, metrics, n_circle));
+}
+
 static db::Region minkowski_sum_pe (const db::Region *r, const db::Edge &e)
 {
   return r->processed (db::minkowski_sum_computation<db::Edge> (e));
 }
 
 static db::Region minkowski_sum_pp (const db::Region *r, const db::Polygon &q)
 {
@@ -1688,46 +1693,52 @@
     "@hide\n"
     "This method is provided for DRC implementation.\n"
   ) +
   method_ext ("extent_refs_edges", &extent_refs_edges,
     "@hide\n"
     "This method is provided for DRC implementation.\n"
   ) +
-  method_ext ("corners", &corners_to_boxes, gsi::arg ("angle_min", -180.0), gsi::arg ("angle_max", 180.0), gsi::arg ("dim", 1), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true),
+  method_ext ("corners", &corners_to_boxes, gsi::arg ("angle_min", -180.0), gsi::arg ("angle_max", 180.0), gsi::arg ("dim", 1), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief This method will select all corners whose attached edges satisfy the angle condition.\n"
     "\n"
     "The angle values specify a range of angles: all corners whose attached edges form an angle "
     "between angle_min and angle_max will be reported boxes with 2*dim x 2*dim dimension. The default dimension is 2x2 DBU.\n"
     "\n"
     "If 'include_angle_min' is true, the angle condition is >= min. angle, otherwise it is > min. angle. "
     "Same for 'include_angle_,ax' and the max. angle.\n"
     "\n"
-    "The angle is measured "
+    "With 'absolute' set to false (the default), the angle is measured "
     "between the incoming and the outcoming edge in mathematical sense: a positive value is a turn left "
     "while a negative value is a turn right. Since polygon contours are oriented clockwise, positive "
     "angles will report concave corners while negative ones report convex ones.\n"
+    "With the 'absolute' option set to true, there is no such distinction and angle values are always positive.\n"
+    "\n"
+    "With 'inverse' set to true, the method will select corners not meeting the angle criterion.\n"
     "\n"
     "A similar function that reports corners as point-like edges is \\corners_dots.\n"
     "\n"
-    "This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27.\n"
+    "This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27. "
+    "'inverse' and 'absolute' have been added in version 0.29.1.\n"
   ) +
-  method_ext ("corners_dots", &corners_to_dots, gsi::arg ("angle_start", -180.0), gsi::arg ("angle_end", 180.0), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true),
+  method_ext ("corners_dots", &corners_to_dots, gsi::arg ("angle_start", -180.0), gsi::arg ("angle_end", 180.0), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief This method will select all corners whose attached edges satisfy the angle condition.\n"
     "\n"
     "This method is similar to \\corners, but delivers an \\Edges collection with dot-like edges for each corner.\n"
     "\n"
-    "This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27.\n"
+    "This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27. "
+    "'inverse' and 'absolute' have been added in version 0.29.1.\n"
   ) +
-  method_ext ("corners_edge_pairs", &corners_to_edge_pairs, gsi::arg ("angle_start", -180.0), gsi::arg ("angle_end", 180.0), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true),
+  method_ext ("corners_edge_pairs", &corners_to_edge_pairs, gsi::arg ("angle_start", -180.0), gsi::arg ("angle_end", 180.0), gsi::arg ("include_min_angle", true), gsi::arg ("include_max_angle", true), gsi::arg ("inverse", false), gsi::arg ("absolute", false),
     "@brief This method will select all corners whose attached edges satisfy the angle condition.\n"
     "\n"
     "This method is similar to \\corners, but delivers an \\EdgePairs collection with an edge pairs for each corner.\n"
     "The first edge is the incoming edge of the corner, the second one the outgoing edge.\n"
     "\n"
-    "This method has been introduced in version 0.27.1.\n"
+    "This method has been introduced in version 0.27.1. "
+    "'inverse' and 'absolute' have been added in version 0.29.1.\n"
   ) +
   method ("merge", (db::Region &(db::Region::*) ()) &db::Region::merge,
     "@brief Merge the region\n"
     "\n"
     "@return The region after is has been merged (self).\n"
     "\n"
     "Merging removes overlaps and joins touching polygons.\n"
@@ -2778,14 +2789,25 @@
     "The Minkowski sum of a region and a contour basically results in the area covered when "
     "\"dragging\" the region along the contour. The effect is similar to drawing the contour "
     "with a pencil that has the shape of the given region.\n"
     "\n"
     "The resulting polygons are not merged. In order to remove overlaps, use the \\merge or \\merged method."
     "Merged semantics applies for the input of this method (see \\merged_semantics= for a description of this concept)\n"
   ) +
+  method_ext ("drc_hull", &drc_hull, gsi::arg ("metrics"), gsi::arg ("space"), gsi::arg ("n_circle", size_t (64)),
+    "@brief Computes a visualization of the forbidden region for a DRC space check\n"
+    "\n"
+    "@param metrics The metrics to apply\n"
+    "@param space The space value to apply\n"
+    "@param n_circle The full-circle number of points for the Euclidian space visualization\n"
+    "\n"
+    "@return The new polygons representing the forbidden region.\n"
+    "\n"
+    "This method has been introduced in version 0.29.1.\n"
+  ) +
   method_ext ("move", &move_p, gsi::arg ("v"),
     "@brief Moves the region\n"
     "\n"
     "Moves the polygon by the given offset and returns the \n"
     "moved region. The region is overwritten.\n"
     "\n"
     "@param v The distance to move the region.\n"
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbShape.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbShape.cc`

 * *Files 1% similar despite different names*

```diff
@@ -2127,14 +2127,29 @@
   ) +
   gsi::method ("==", &db::Shape::operator==, gsi::arg ("other"),
     "@brief Equality operator\n"
     "\n"
     "Equality of shapes is not specified by the identity of the objects but by the\n"
     "identity of the pointers - both shapes must refer to the same object.\n"
   ) +
+  gsi::method ("<", &db::Shape::operator<, gsi::arg ("other"),
+    "@brief Less operator\n"
+    "\n"
+    "The less operator implementation is based on pointers and not strictly reproducible."
+    "However, it is good enough so Shape objects can serve as keys in hashes (see also \\hash).\n"
+    "\n"
+    "This method has been introduced in version 0.29.1."
+  ) +
+  gsi::method ("hash", &db::Shape::hash_value,
+    "@brief Hash function\n"
+    "\n"
+    "The hash function enables Shape objects as keys in hashes.\n"
+    "\n"
+    "This method has been introduced in version 0.29.1."
+  ) +
   gsi::method ("to_s", &db::Shape::to_string,
     "@brief Create a string showing the contents of the reference\n"
     "\n"
     "This method has been introduced with version 0.16."
   ) +
   gsi::method ("TNull|#t_null", &t_null) +
   gsi::method ("TPolygon|#t_polygon", &t_polygon) +
```

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbShapeCollection.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbShapeCollection.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbShapeProcessor.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbShapeProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbShapes.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbShapes.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbTechnologies.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbTechnologies.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbText.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbText.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbTexts.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbTexts.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbTilingProcessor.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbTilingProcessor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbTrans.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbTrans.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbUtils.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/db/db/gsiDeclDbVector.cc` & `klayout-0.29.1/src/db/db/gsiDeclDbVector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtCommon.h` & `klayout-0.29.1/src/edt/edt/edtCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtConfig.cc` & `klayout-0.29.1/src/edt/edt/edtConfig.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtConfig.h` & `klayout-0.29.1/src/edt/edt/edtConfig.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtDialogs.cc` & `klayout-0.29.1/src/edt/edt/edtDialogs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtDialogs.h` & `klayout-0.29.1/src/edt/edt/edtDialogs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtDistribute.cc` & `klayout-0.29.1/src/edt/edt/edtDistribute.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtDistribute.h` & `klayout-0.29.1/src/edt/edt/edtDistribute.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtEditorOptionsPages.cc` & `klayout-0.29.1/src/edt/edt/edtEditorOptionsPages.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtEditorOptionsPages.h` & `klayout-0.29.1/src/edt/edt/edtEditorOptionsPages.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtForceLink.cc` & `klayout-0.29.1/src/edt/edt/edtForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtForceLink.h` & `klayout-0.29.1/src/edt/edt/edtForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtInstPropertiesPage.cc` & `klayout-0.29.1/src/edt/edt/edtInstPropertiesPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtInstPropertiesPage.h` & `klayout-0.29.1/src/edt/edt/edtInstPropertiesPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtMainService.cc` & `klayout-0.29.1/src/edt/edt/edtMainService.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtMainService.h` & `klayout-0.29.1/src/edt/edt/edtMainService.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPCellParametersPage.cc` & `klayout-0.29.1/src/edt/edt/edtPCellParametersPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPCellParametersPage.h` & `klayout-0.29.1/src/edt/edt/edtPCellParametersPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPartialService.cc` & `klayout-0.29.1/src/edt/edt/edtPartialService.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1412,115 +1412,254 @@
   //  just allow displacements
   db::DTrans move_trans (tr.disp ());
   transform_selection (move_trans);
 
   selection_to_view ();
 }
 
-void  
-PartialService::transform_selection (const db::DTrans &move_trans)
+void
+PartialService::open_editor_hooks ()
+{
+  lay::CellViewRef cv_ref (view ()->cellview_ref (view ()->active_cellview_index ()));
+  if (! cv_ref.is_valid ()) {
+    return;
+  }
+
+  std::string technology;
+  if (cv_ref->layout ().technology ()) {
+    technology = cv_ref->layout ().technology ()->name ();
+  }
+
+  m_editor_hooks = edt::EditorHooks::get_editor_hooks (technology);
+  call_editor_hooks<lay::CellViewRef &> (m_editor_hooks, &edt::EditorHooks::begin_edit, (lay::CellViewRef &) cv_ref);
+}
+
+void
+PartialService::close_editor_hooks (bool commit)
+{
+  if (commit) {
+    call_editor_hooks (m_editor_hooks, &edt::EditorHooks::commit_edit);
+  }
+  call_editor_hooks (m_editor_hooks, &edt::EditorHooks::end_edit);
+
+  m_editor_hooks.clear ();
+}
+
+void
+PartialService::issue_editor_hook_calls (const tl::weak_collection<edt::EditorHooks> &hooks)
 {
+  if (hooks.empty ()) {
+    return;
+  }
+
+  //  NOTE: needs to be called during move operations
+  db::DTrans move_trans = db::DTrans (m_current - m_start);
+
   //  build the transformation variants cache
   TransformationVariants tv (view ());
 
+  //  Issue editor hook calls for the shape modification events
+
   //  since a shape reference may become invalid while moving it and
   //  because it creates ambiguities, we treat each shape separately:
   //  collect the valid selected items in a selection-per-shape map.
   std::map <db::Shape, std::vector<partial_objects::iterator> > sel_per_shape;
 
   for (partial_objects::iterator r = m_selection.begin (); r != m_selection.end (); ++r) {
     if (! r->first.is_cell_inst ()) {
       const std::vector<db::DCplxTrans> *tv_list = tv.per_cv_and_layer (r->first.cv_index (), r->first.layer ());
       if (tv_list && ! tv_list->empty ()) {
         sel_per_shape.insert (std::make_pair (r->first.shape (), std::vector<partial_objects::iterator> ())).first->second.push_back (r);
       }
     }
   }
 
+  db::Shapes tmp_shapes;
+
   for (std::map <db::Shape, std::vector<partial_objects::iterator> >::iterator sps = sel_per_shape.begin (); sps != sel_per_shape.end (); ++sps) {
 
-    db::Shape shape = sps->first;
+    db::Shape shape = tmp_shapes.insert (sps->first);
+    for (std::vector<partial_objects::iterator>::const_iterator rr = sps->second.begin (); rr != sps->second.end (); ++rr) {
+
+      std::map <EdgeWithIndex, db::Edge> new_edges;
+      std::map <PointWithIndex, db::Point> new_points;
+
+      shape = modify_shape (tv, shape, (*rr)->first, (*rr)->second, move_trans, new_edges, new_points);
+
+    }
 
     for (std::vector<partial_objects::iterator>::const_iterator rr = sps->second.begin (); rr != sps->second.end (); ++rr) {
 
-      partial_objects::iterator r = *rr;
+      const lay::ObjectInstPath &sel = (*rr)->first;
 
-      const lay::CellView &cv = view ()->cellview (r->first.cv_index ());
+      const lay::CellView &cv = view ()->cellview (sel.cv_index ());
 
-      //  use only the first one of the explicit transformations 
-      //  TODO: clarify how this can be implemented in a more generic form or leave it thus.
+      //  compute the transformation into context cell's micron space
+      double dbu = cv->layout ().dbu ();
+      db::CplxTrans gt = db::CplxTrans (dbu) * cv.context_trans () * sel.trans ();
 
-      db::ICplxTrans gt (cv.context_trans () * r->first.trans ());
-      const std::vector<db::DCplxTrans> *tv_list = tv.per_cv_and_layer (r->first.cv_index (), r->first.layer ());
-      db::CplxTrans tt = (*tv_list) [0] * db::CplxTrans (cv->layout ().dbu ()) * gt;
-      db::Vector move_vector = db::Vector ((tt.inverted () * db::DCplxTrans (move_trans) * tt).disp ());
+      //  get one representative global transformation
+      const std::vector<db::DCplxTrans> *tv_list = tv.per_cv_and_layer (sel.cv_index (), sel.layer ());
+      if (tv_list && ! tv_list->empty ()) {
+        gt = tv_list->front () * gt;
+      }
 
-      std::map <EdgeWithIndex, db::Edge> new_edges;
-      std::map <PointWithIndex, db::Point> new_points;
-      create_shift_sets (shape, r->second, new_points, new_edges, move_vector);
+      call_editor_hooks<const lay::ObjectInstPath &, const db::Shape &, const db::CplxTrans &> (hooks, &edt::EditorHooks::modified, (*rr)->first, shape, gt);
 
-      //  modify the shapes and insert
+    }
 
-      db::Shapes &shapes = cv->layout ().cell (r->first.cell_index ()).shapes (r->first.layer ());
+  }
 
-      if (shape.is_polygon ()) {
+  //  Issue editor hook calls for the instance transformation events
 
-        db::Polygon poly;
-        shape.polygon (poly);
+  //  sort the selected objects (the instances) by the cell they are in
+  //  The key is a pair: cell_index, cv_index
+  std::map <std::pair <db::cell_index_type, unsigned int>, std::vector <partial_objects::const_iterator> > insts_by_cell;
+  for (partial_objects::const_iterator r = m_selection.begin (); r != m_selection.end (); ++r) {
+    if (r->first.is_cell_inst ()) {
+      insts_by_cell.insert (std::make_pair (std::make_pair (r->first.cell_index (), r->first.cv_index ()), std::vector <partial_objects::const_iterator> ())).first->second.push_back (r);
+    }
+  }
 
-        //  warning: poly is modified:
-        modify_polygon (poly, new_points, new_edges, true /*compress*/);
+  for (std::map <std::pair <db::cell_index_type, unsigned int>, std::vector <partial_objects::const_iterator> >::const_iterator ibc = insts_by_cell.begin (); ibc != insts_by_cell.end (); ++ibc) {
 
-        shape = shapes.replace (shape, poly);
+    const lay::CellView &cv = view ()->cellview (ibc->first.second);
+    if (cv.is_valid ()) {
 
-      } else if (shape.is_path ()) {
+      const std::vector<db::DCplxTrans> *tv_list = tv.per_cv (ibc->first.second);
+      db::DCplxTrans tvt;
+      if (tv_list && ! tv_list->empty ()) {
+        tvt = tv_list->front ();
+      }
 
-        db::Path path;
-        shape.path (path);
+      for (auto inst = ibc->second.begin (); inst != ibc->second.end (); ++inst) {
 
-        //  warning: path is modified:
-        modify_path (path, new_points, new_edges, true /*compress*/);
+        db::CplxTrans gt = tvt * db::CplxTrans (cv->layout ().dbu ()) * cv.context_trans () * (*inst)->first.trans ();
+        db::ICplxTrans applied = gt.inverted () * db::DCplxTrans (move_trans) * gt;
 
-        shape = shapes.replace (shape, path);
+        call_editor_hooks<const lay::ObjectInstPath &, const db::ICplxTrans &, const db::CplxTrans &> (hooks, &edt::EditorHooks::transformed, (*inst)->first, applied, gt);
 
-      } else if (shape.is_box ()) {
+      }
 
-        db::Polygon poly;
-        shape.polygon (poly);
+    }
 
-        //  warning: poly is modified:
-        modify_polygon (poly, new_points, new_edges, true /*compress*/);
+  }
+}
 
-        shape = shapes.replace (shape, poly.box ());
+db::Shape
+PartialService::modify_shape (TransformationVariants &tv, const db::Shape &shape_in, const lay::ObjectInstPath &path, const std::set <EdgeWithIndex> &sel, const db::DTrans &move_trans, std::map <EdgeWithIndex, db::Edge> &new_edges, std::map <PointWithIndex, db::Point> &new_points)
+{
+  tl_assert (shape_in.shapes () != 0);
+  db::Shape shape = shape_in;
+  db::Shapes &shapes = *shape_in.shapes ();
 
-      } else if (shape.is_text ()) {
+  const lay::CellView &cv = view ()->cellview (path.cv_index ());
 
-        db::Text t;
-        shape.text (t);
+  //  use only the first one of the explicit transformations
+  //  TODO: clarify how this can be implemented in a more generic form or leave it thus.
 
-        db::Point tp (shape.text_trans () * db::Point ());
-        std::map <PointWithIndex, db::Point>::const_iterator np = new_points.find (PointWithIndex (tp, 0, 0));
+  db::ICplxTrans gt (cv.context_trans () * path.trans ());
+  const std::vector<db::DCplxTrans> *tv_list = tv.per_cv_and_layer (path.cv_index (), path.layer ());
+  db::CplxTrans tt = (*tv_list) [0] * db::CplxTrans (cv->layout ().dbu ()) * gt;
+  db::Vector move_vector = db::Vector ((tt.inverted () * db::DCplxTrans (move_trans) * tt).disp ());
 
-        if (np != new_points.end ()) {
-          t.transform (db::Trans (np->second - tp));
-          shape = shapes.replace (shape, t);
-        }
+  create_shift_sets (shape, sel, new_points, new_edges, move_vector);
 
-      } else if (shape.is_point ()) {
+  //  modify the shapes and insert
 
-        db::Point p;
-        shape.point (p);
+  if (shape.is_polygon ()) {
 
-        std::map <PointWithIndex, db::Point>::const_iterator np = new_points.find (PointWithIndex (p, 0, 0));
+    db::Polygon poly;
+    shape.polygon (poly);
 
-        if (np != new_points.end ()) {
-          shape = shapes.replace (shape, np->second);
-        }
+    //  warning: poly is modified:
+    modify_polygon (poly, new_points, new_edges, true /*compress*/);
+
+    shape = shapes.replace (shape, poly);
+
+  } else if (shape.is_path ()) {
+
+    db::Path path;
+    shape.path (path);
+
+    //  warning: path is modified:
+    modify_path (path, new_points, new_edges, true /*compress*/);
+
+    shape = shapes.replace (shape, path);
+
+  } else if (shape.is_box ()) {
+
+    db::Polygon poly;
+    shape.polygon (poly);
+
+    //  warning: poly is modified:
+    modify_polygon (poly, new_points, new_edges, true /*compress*/);
+
+    shape = shapes.replace (shape, poly.box ());
+
+  } else if (shape.is_text ()) {
+
+    db::Text t;
+    shape.text (t);
+
+    db::Point tp (shape.text_trans () * db::Point ());
+    std::map <PointWithIndex, db::Point>::const_iterator np = new_points.find (PointWithIndex (tp, 0, 0));
 
+    if (np != new_points.end ()) {
+      t.transform (db::Trans (np->second - tp));
+      shape = shapes.replace (shape, t);
+    }
+
+  } else if (shape.is_point ()) {
+
+    db::Point p;
+    shape.point (p);
+
+    std::map <PointWithIndex, db::Point>::const_iterator np = new_points.find (PointWithIndex (p, 0, 0));
+
+    if (np != new_points.end ()) {
+      shape = shapes.replace (shape, np->second);
+    }
+
+  }
+
+  return shape;
+}
+
+void
+PartialService::transform_selection (const db::DTrans &move_trans)
+{
+  //  build the transformation variants cache
+  TransformationVariants tv (view ());
+
+  //  since a shape reference may become invalid while moving it and
+  //  because it creates ambiguities, we treat each shape separately:
+  //  collect the valid selected items in a selection-per-shape map.
+  std::map <db::Shape, std::vector<partial_objects::iterator> > sel_per_shape;
+
+  for (partial_objects::iterator r = m_selection.begin (); r != m_selection.end (); ++r) {
+    if (! r->first.is_cell_inst ()) {
+      const std::vector<db::DCplxTrans> *tv_list = tv.per_cv_and_layer (r->first.cv_index (), r->first.layer ());
+      if (tv_list && ! tv_list->empty ()) {
+        sel_per_shape.insert (std::make_pair (r->first.shape (), std::vector<partial_objects::iterator> ())).first->second.push_back (r);
       }
+    }
+  }
+
+  for (std::map <db::Shape, std::vector<partial_objects::iterator> >::iterator sps = sel_per_shape.begin (); sps != sel_per_shape.end (); ++sps) {
+
+    db::Shape shape = sps->first;
+
+    for (std::vector<partial_objects::iterator>::const_iterator rr = sps->second.begin (); rr != sps->second.end (); ++rr) {
+
+      partial_objects::iterator r = *rr;
+
+      std::map <EdgeWithIndex, db::Edge> new_edges;
+      std::map <PointWithIndex, db::Point> new_points;
+      shape = modify_shape (tv, shape, r->first, r->second, move_trans, new_edges, new_points);
 
       //  transform the selection 
       
       std::set <EdgeWithIndex> new_sel;
       new_sel.swap (r->second);
 
       for (std::set <EdgeWithIndex>::const_iterator s = new_sel.begin (); s != new_sel.end () && m_keep_selection; ++s) {
@@ -1621,14 +1760,16 @@
   if (mp_box) {
     delete mp_box;
     mp_box = 0;
   }
 
   ui ()->ungrab_mouse (this);
 
+  close_editor_hooks (false);
+
   selection_to_view ();
 }
 
 bool 
 PartialService::wheel_event (int /*delta*/, bool /*horizontal*/, const db::DPoint & /*p*/, unsigned int /*buttons*/, bool /*prio*/)
 {
   hover_reset ();
@@ -1667,14 +1808,18 @@
       m_current = m_start + snap_move (p - m_start);
       clear_mouse_cursors ();
 
     }
 
     selection_to_view ();
 
+    call_editor_hooks (m_editor_hooks, &edt::EditorHooks::begin_edits);
+    issue_editor_hook_calls (m_editor_hooks);
+    call_editor_hooks (m_editor_hooks, &edt::EditorHooks::end_edits);
+
     m_alt_ac = lay::AC_Global;
 
   } else if (prio) {
     
     if (mp_box) {
 
       m_alt_ac = ac_from_buttons (buttons);
@@ -1792,14 +1937,16 @@
         m_current = m_start = projected_to_edge (single_selected_edge (), p);
       } else {
         m_current = m_start = p;
       }
 
       ui ()->grab_mouse (this, true);
 
+      open_editor_hooks ();
+
     }
 
     m_alt_ac = lay::AC_Global;
 
     return true;
 
   }
@@ -1854,14 +2001,16 @@
     if (! m_keep_selection) {
       m_selection.clear ();
     }
 
     m_dragging = false;
     selection_to_view ();
 
+    close_editor_hooks (true);
+
     m_alt_ac = lay::AC_Global;
 
     return true;
 
   } else if (ui ()->mouse_event_viewport ().contains (p)) { 
 
     //  clear other selection when this mode gets active
@@ -1987,14 +2136,16 @@
           //  for an edge selection use the point projected to edge as the start location which
           //  allows bringing it to grid
           m_current = m_start = projected_to_edge (single_selected_edge (), p);
         } else {
           m_current = m_start = p;
         }
 
+        open_editor_hooks ();
+
       }
 
       selection_to_view ();
 
     } catch (tl::Exception &ex) {
       show_error (ex);
       //  clear selection
@@ -2019,14 +2170,16 @@
     return false;
   }
 
   if ((buttons & lay::LeftButton) != 0 && prio) {
 
     m_alt_ac = ac_from_buttons (buttons);
 
+    close_editor_hooks (false);
+
     //  stop dragging
     ui ()->ungrab_mouse (this);
     m_dragging = false;
       
     partial_select (db::DBox (p, p), lay::Editable::Replace);
 
     if (! m_selection.empty ()) {
@@ -2349,14 +2502,16 @@
   }
 
   m_dragging = false;
   selection_to_view ();
 
   clear_mouse_cursors ();
 
+  close_editor_hooks (false);
+
   m_alt_ac = lay::AC_Global;
 }
 
 bool
 PartialService::has_selection ()
 {
   return ! m_selection.empty ();
@@ -2526,14 +2681,16 @@
   //  handles guiding shapes, this should be fairly safe.
   handle_guiding_shape_changes ();
 
   m_selection.clear ();
   m_dragging = false;
   selection_to_view ();
 
+  close_editor_hooks (false);
+
   //  clean up the layouts that need to do so.
   for (std::set<db::Layout *>::const_iterator l = needs_cleanup.begin (); l != needs_cleanup.end (); ++l) {
     (*l)->cleanup ();
   }
 }
 
 lay::InstanceMarker *
```

### Comparing `klayout-0.29.0/src/edt/edt/edtPartialService.h` & `klayout-0.29.1/src/edt/edt/edtPartialService.h`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #include "layViewObject.h"
 #include "layRubberBox.h"
 #include "laySnap.h"
 #include "tlAssert.h"
 #include "tlDeferredExecution.h"
 #include "edtUtils.h"
 #include "edtConfig.h"
+#include "edtEditorHooks.h"
 
 #if defined(HAVE_QT)
 #  include <QObject>
 #  include <QTimer>
 #endif
 
 namespace db {
@@ -312,14 +313,19 @@
   virtual void set_colors (tl::Color background, tl::Color text);
 
   /**
    *  @brief Cancel any edit operations (in this case, unselect all & cancel any drag operation)
    */
   virtual void edit_cancel ();
 
+  /**
+   *  @brief Issues editor hook calls ("modified") for the current selection and the given move transformation
+   */
+  void issue_editor_hook_calls (const tl::weak_collection<edt::EditorHooks> &hooks);
+
 #if defined(HAVE_QT)
 public slots:
   void timeout ();
 #endif
 
 protected:
   lay::angle_constraint_type connect_ac () const;
@@ -357,14 +363,16 @@
 #if defined(HAVE_QT)
   QTimer m_timer;
 #endif
   bool m_hover;
   bool m_hover_wait;
   db::DPoint m_hover_point;
 
+  tl::weak_collection<edt::EditorHooks> m_editor_hooks;
+
   //  Deferred method to update the selection
   tl::DeferredMethod<edt::PartialService> dm_selection_to_view;
 
   void hover_reset ();
 
   void clear_partial_transient_selection ();
   bool partial_select (const db::DBox &box, lay::Editable::SelectionMode mode);
@@ -388,13 +396,17 @@
   void resize_inst_markers (size_t n, bool transient);
   bool is_single_point_selection () const;
   bool is_single_edge_selection () const;
   db::DPoint single_selected_point () const;
   db::DEdge single_selected_edge () const;
   bool handle_guiding_shape_changes ();
   void transform_selection (const db::DTrans &move_trans);
+  db::Shape modify_shape (TransformationVariants &tv, const db::Shape &shape_in, const lay::ObjectInstPath &path, const std::set<EdgeWithIndex> &sel, const db::DTrans &move_trans, std::map <EdgeWithIndex, db::Edge> &new_edges, std::map <PointWithIndex, db::Point> &new_points);
+
+  void open_editor_hooks ();
+  void close_editor_hooks (bool commit);
 };
 
 }
 
 #endif
```

### Comparing `klayout-0.29.0/src/edt/edt/edtPlugin.cc` & `klayout-0.29.1/src/edt/edt/edtPlugin.cc`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #include "layLayoutViewBase.h"
 #include "edtPlugin.h"
 #include "edtConfig.h"
 #include "edtService.h"
 #include "edtServiceImpl.h"
 #include "edtMainService.h"
 #include "edtPartialService.h"
+#include "edtMoveTrackerService.h"
 #if defined(HAVE_QT)
 #  include "edtEditorOptionsPages.h"
 #  include "edtRecentConfigurationPage.h"
 #endif
 
 #if defined(HAVE_QT)
 #  include <QApplication>
@@ -561,9 +562,30 @@
 
 static tl::RegisteredClass<lay::PluginDeclaration> config_decl30 (
   new edt::PartialPluginDeclaration (tl::to_string (tr ("Partial shapes")), "partial:edit_mode\t" + tl::to_string (tr ("Partial{Edit points and edges of shapes}")) + "<:partial_24px.png>"),
   4030, 
   "edt::PartialService"
 );
 
+class MoveTrackerPluginDeclaration
+  : public lay::PluginDeclaration
+{
+public:
+  MoveTrackerPluginDeclaration ()
+  {
+    //  .. nothing yet ..
+  }
+
+  virtual lay::Plugin *create_plugin (db::Manager * /*manager*/, lay::Dispatcher * /*root*/, lay::LayoutViewBase *view) const
+  {
+    return new edt::MoveTrackerService (view);
+  }
+};
+
+static tl::RegisteredClass<lay::PluginDeclaration> config_decl40 (
+  new MoveTrackerPluginDeclaration (),
+  4100,
+  "edt::MoveTrackerService"
+);
+
 }
```

### Comparing `klayout-0.29.0/src/edt/edt/edtPlugin.h` & `klayout-0.29.1/src/edt/edt/edtPlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPropertiesPageUtils.cc` & `klayout-0.29.1/src/edt/edt/edtPropertiesPageUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPropertiesPageUtils.h` & `klayout-0.29.1/src/edt/edt/edtPropertiesPageUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPropertiesPages.cc` & `klayout-0.29.1/src/edt/edt/edtPropertiesPages.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtPropertiesPages.h` & `klayout-0.29.1/src/edt/edt/edtPropertiesPages.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtRecentConfigurationPage.cc` & `klayout-0.29.1/src/edt/edt/edtRecentConfigurationPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtRecentConfigurationPage.h` & `klayout-0.29.1/src/edt/edt/edtRecentConfigurationPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtService.cc` & `klayout-0.29.1/src/edt/edt/edtService.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtService.h` & `klayout-0.29.1/src/edt/edt/edtService.h`

 * *Files 2% similar despite different names*

```diff
@@ -377,14 +377,30 @@
   /**
    *  @brief Handle changes in a specific guiding shape, i.e. create new PCell variants if required
    *
    *  @return A pair of bool (indicating that the object path has changed) and the new guiding shape path
    */
   std::pair<bool, lay::ObjectInstPath> handle_guiding_shape_changes (const lay::ObjectInstPath &obj) const;
 
+  /**
+   *  @brief Gets a value indicating whether a move operation is ongoing
+   */
+  bool is_moving () const
+  {
+    return m_moving;
+  }
+
+  /**
+   *  @brief Gets the current move transformation (in DBU space on context cell level)
+   */
+  const db::DTrans &move_trans () const
+  {
+    return m_move_trans;
+  }
+
 protected:
   /**
    *  @brief Update m_markers to reflect the selection
    */
   void selection_to_view ();
 
   /**
```

### Comparing `klayout-0.29.0/src/edt/edt/edtServiceImpl.cc` & `klayout-0.29.1/src/edt/edt/edtServiceImpl.cc`

 * *Files 6% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     }
   }
 
   m_layer = (unsigned int) layer;
   m_cv_index = (unsigned int) cv_index;
   m_trans = (cl->trans ().front () * db::CplxTrans (cv->layout ().dbu ()) * cv.context_trans ()).inverted ();
   mp_layout = &(cv->layout ());
-  mp_cell = &(mp_layout->cell (cv.cell_index ()));
+  mp_cell = cv.cell ();
 
   if (mp_cell->is_proxy ()) {
     throw tl::Exception (tl::to_string (tr ("Cannot put a shape into a PCell or library cell")));
   }
 }
 
 void
@@ -153,15 +153,15 @@
   const lay::CellView &cv = view ()->cellview (cv_index);
   int layer = cl->layer_index ();
 
   if (cv_index < 0 || ! cv.is_valid ()) {
     return;
   }
 
-  if (cv->layout ().cell (cv.cell_index ()).is_proxy ()) {
+  if (cv.cell ()->is_proxy ()) {
     return;
   }
 
 #if defined(HAVE_QT)
   if (! cl->visible (true)) {
     lay::TipDialog td (QApplication::activeWindow (),
                        tl::to_string (tr ("You are now drawing on a hidden layer. The result won't be visible.")),
@@ -194,15 +194,15 @@
 
   }
 
   m_layer = (unsigned int) layer;
   m_cv_index = (unsigned int) cv_index;
   m_trans = (cl->trans ().front () * db::CplxTrans (cv->layout ().dbu ()) * cv.context_trans ()).inverted ();
   mp_layout = &(cv->layout ());
-  mp_cell = &(mp_layout->cell (cv.cell_index ()));
+  mp_cell = cv.cell ();
 
   current_layer_changed ();
 }
 
 void
 ShapeEditService::tap (const db::DPoint &initial)
 {
@@ -396,14 +396,55 @@
     cell ().shapes (layer ()).insert (point);
     if (manager ()) {
       manager ()->commit ();
     }
   }
 }
 
+void
+ShapeEditService::open_editor_hooks ()
+{
+  std::string technology;
+  if (mp_layout && mp_layout->technology ()) {
+    technology = mp_layout->technology ()->name ();
+  }
+
+  m_editor_hooks = edt::EditorHooks::get_editor_hooks (technology);
+
+  lay::CellViewRef cv_ref (view ()->cellview_ref (m_cv_index));
+  call_editor_hooks<lay::CellViewRef &, const lay::LayerProperties &> (m_editor_hooks, &edt::EditorHooks::begin_create_shapes, cv_ref, *view ()->current_layer ());
+}
+
+void
+ShapeEditService::close_editor_hooks (bool with_commit)
+{
+  if (with_commit) {
+    call_editor_hooks (m_editor_hooks, &edt::EditorHooks::commit_shapes);
+  }
+  call_editor_hooks (m_editor_hooks, &edt::EditorHooks::end_create_shapes);
+
+  m_editor_hooks.clear ();
+}
+
+template <class Shape>
+void
+ShapeEditService::deliver_shape_to_hooks (const Shape &shape)
+{
+  db::Shapes tmp (true);
+  db::Shape s = tmp.insert (shape);
+  call_editor_hooks<const db::Shape &, const db::CplxTrans &> (m_editor_hooks, &edt::EditorHooks::create_shape, s, trans ().inverted ());
+}
+
+//  explicit instantiations
+template void ShapeEditService::deliver_shape_to_hooks<db::Polygon> (const db::Polygon &);
+template void ShapeEditService::deliver_shape_to_hooks<db::Path> (const db::Path &);
+template void ShapeEditService::deliver_shape_to_hooks<db::Box> (const db::Box &);
+template void ShapeEditService::deliver_shape_to_hooks<db::Point> (const db::Point &);
+template void ShapeEditService::deliver_shape_to_hooks<db::Text> (const db::Text &);
+
 // -----------------------------------------------------------------------------
 //  PolygonService implementation
 
 PolygonService::PolygonService (db::Manager *manager, lay::LayoutViewBase *view)
   : ShapeEditService (manager, view, db::ShapeIterator::Polygons),
     m_closure_set (false), m_closure ()
 {
@@ -429,14 +470,16 @@
   m_last = pp;
 
   m_points.clear ();
   m_points.push_back (pp);
   m_points.push_back (pp);
   m_closure_set = false;
 
+  open_editor_hooks ();
+
   update_marker ();
 }
 
 void 
 PolygonService::set_last_point (const db::DPoint &p)
 {
   m_points.back () = snap2 (p, m_last);
@@ -499,51 +542,55 @@
   //  do not do a add_closure here - this will not work since we may have two identical points on top.
   return false;
 }
 
 void 
 PolygonService::do_finish_edit ()
 {
-  deliver_shape (get_polygon ());
+  deliver_shape (get_polygon (false));
   commit_recent (view ());
+  close_editor_hooks (true);
 }
 
 db::Polygon
-PolygonService::get_polygon () const
+PolygonService::get_polygon (bool editing) const
 {
   db::Polygon poly;
 
-  if (m_points.size () < 4) {
+  if (! editing && m_points.size () + (m_closure_set ? 1 : 0) < 4) {
     throw tl::Exception (tl::to_string (tr ("A polygon must have at least 3 points")));
   }
 
   std::vector<db::Point> points_dbu;
-  points_dbu.reserve (m_points.size ());
+  points_dbu.reserve (m_points.size () + 1);
 
   //  one point is reserved for the current one
   for (std::vector<db::DPoint>::const_iterator p = m_points.begin (); p + 1 != m_points.end (); ++p) {
     points_dbu.push_back (trans () * *p);
   }
+  if (editing) {
+    points_dbu.push_back (trans () * m_points.back ());
+  }
   if (m_closure_set) {
     points_dbu.push_back (trans () * m_closure);
   }
 
-  poly.assign_hull (points_dbu.begin (), points_dbu.end (), true, true /*remove reflected*/);
+  poly.assign_hull (points_dbu.begin (), points_dbu.end (), !editing /*compress*/, !editing /*remove reflected*/);
 
-  if (poly.hull ().size () < 3) {
+  if (! editing && poly.hull ().size () < 3) {
     throw tl::Exception (tl::to_string (tr ("A polygon must have at least 3 effective points")));
   }
 
   return poly;
 }
 
 void 
 PolygonService::do_cancel_edit ()
 {
-  //  .. nothing yet ..
+  close_editor_hooks (false);
 }
 
 bool 
 PolygonService::selection_applies (const lay::ObjectInstPath &sel) const
 {
   return !sel.is_cell_inst () && sel.shape ().is_polygon ();
 }
@@ -728,14 +775,25 @@
     view ()->message (std::string ("lx: ") +
                       tl::micron_to_string (m_points.back ().x () - m_points.end () [-2].x ()) + 
                       std::string ("  ly: ") +
                       tl::micron_to_string (m_points.back ().y () - m_points.end () [-2].y ()) + 
                       std::string ("  l: ") +
                       tl::micron_to_string (m_points.back ().distance (m_points.end () [-2])));
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_shapes);
+    try {
+      deliver_shape_to_hooks (get_polygon (true));
+    } catch (...) {
+      //  ignore exceptions
+    }
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_shapes);
+  }
 }
 
 // -----------------------------------------------------------------------------
 //  BoxService implementation
 
 BoxService::BoxService (db::Manager *manager, lay::LayoutViewBase *view)
   : ShapeEditService (manager, view, db::ShapeIterator::Boxes)
@@ -757,14 +815,16 @@
 BoxService::do_begin_edit (const db::DPoint &p)
 {
   get_edit_layer ();
 
   db::DPoint pp = snap2 (p);
   m_p1 = m_p2 = pp;
 
+  open_editor_hooks ();
+
   set_edit_marker (new lay::Marker (view (), cv_index ()));
   update_marker ();
 }
 
 db::Box
 BoxService::get_box () const
 {
@@ -781,14 +841,25 @@
 
     view ()->message (std::string ("lx: ") +
                       tl::micron_to_string (m_p2.x () - m_p1.x ()) + 
                       std::string ("  ly: ") +
                       tl::micron_to_string (m_p2.y () - m_p1.y ()));
 
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_shapes);
+    try {
+      deliver_shape_to_hooks (get_box ());
+    } catch (...) {
+      //  ignore exceptions
+    }
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_shapes);
+  }
 }
 
 void
 BoxService::do_mouse_move_inactive (const db::DPoint &p)
 {
   lay::PointSnapToObjectResult snap_details = snap2_details (p);
   mouse_cursor_from_snap_details (snap_details);
@@ -812,20 +883,21 @@
 }
 
 void 
 BoxService::do_finish_edit ()
 {
   deliver_shape (get_box ());
   commit_recent (view ());
+  close_editor_hooks (true);
 }
 
 void 
 BoxService::do_cancel_edit ()
 {
-  //  .. nothing yet ..
+  close_editor_hooks (false);
 }
 
 bool 
 BoxService::selection_applies (const lay::ObjectInstPath &sel) const
 {
   return !sel.is_cell_inst () && sel.shape ().is_box ();
 }
@@ -853,14 +925,16 @@
 PointService::do_begin_edit (const db::DPoint &p)
 {
   get_edit_layer ();
 
   db::DPoint pp = snap2 (p);
   m_p = pp;
 
+  open_editor_hooks ();
+
   set_edit_marker (new lay::Marker (view (), cv_index ()));
   update_marker ();
 }
 
 db::Point
 PointService::get_point () const
 {
@@ -878,14 +952,25 @@
 
     view ()->message (std::string ("x: ") +
                       tl::micron_to_string (m_p.x ()) +
                       std::string ("  y: ") +
                       tl::micron_to_string (m_p.y ()));
 
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_shapes);
+    try {
+      deliver_shape_to_hooks (get_point ());
+    } catch (...) {
+      //  ignore exceptions
+    }
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_shapes);
+  }
 }
 
 void
 PointService::do_mouse_move_inactive (const db::DPoint &p)
 {
   lay::PointSnapToObjectResult snap_details = snap2_details (p);
   mouse_cursor_from_snap_details (snap_details);
@@ -909,20 +994,21 @@
 }
 
 void
 PointService::do_finish_edit ()
 {
   deliver_shape (get_point ());
   commit_recent (view ());
+  close_editor_hooks (true);
 }
 
 void
 PointService::do_cancel_edit ()
 {
-  //  .. nothing yet ..
+  close_editor_hooks (false);
 }
 
 bool
 PointService::selection_applies (const lay::ObjectInstPath &sel) const
 {
   return !sel.is_cell_inst () && sel.shape ().is_point ();
 }
@@ -955,14 +1041,16 @@
 void 
 TextService::do_begin_edit (const db::DPoint &p)
 {
   get_edit_layer ();
 
   m_text.trans (db::DTrans (m_rot, snap2 (p) - db::DPoint ()));
 
+  open_editor_hooks ();
+
   lay::DMarker *marker = new lay::DMarker (view ());
   marker->set_vertex_shape (lay::ViewOp::Cross);
   marker->set_vertex_size (9 /*cross vertex size*/);
   set_edit_marker (marker);
   update_marker ();
 }
 
@@ -981,14 +1069,25 @@
     if (m_text.trans ().rot () != 0) {
       pos += std::string ("  ") + ((const db::DFTrans &) m_text.trans ()).to_string ();
     }
 
     view ()->message (pos);
 
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_shapes);
+    try {
+      deliver_shape_to_hooks (get_text ());
+    } catch (...) {
+      //  ignore exceptions
+    }
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_shapes);
+  }
 }
 
 bool
 TextService::do_activated ()
 {
   m_rot = 0;
 
@@ -1061,20 +1160,22 @@
     td.exec_dialog (button);
     if (button == lay::TipDialog::yes_button) {
       view ()->text_visible (true);
     }
 
   }
 #endif
+
+  close_editor_hooks (true);
 }
 
 void 
 TextService::do_cancel_edit ()
 {
-  //  .. nothing yet ..
+  close_editor_hooks (false);
 }
 
 bool 
 TextService::selection_applies (const lay::ObjectInstPath &sel) const
 {
   return !sel.is_cell_inst () && sel.shape ().is_text ();
 }
@@ -1162,14 +1263,16 @@
   db::DPoint pp = snap2 (p);
   m_last = pp;
 
   m_points.clear ();
   m_points.push_back (pp);
   m_points.push_back (pp);
 
+  open_editor_hooks ();
+
   set_edit_marker (new lay::Marker (view (), cv_index ()));
   update_marker ();
 }
 
 bool
 PathService::do_activated ()
 {
@@ -1246,14 +1349,16 @@
     throw tl::Exception (tl::to_string (tr ("A path must have at least 2 points")));
   }
   m_points.pop_back ();
 
   deliver_shape (get_path ());
 
   commit_recent (view ());
+
+  close_editor_hooks (true);
 }
 
 void
 PathService::update_marker ()
 {
   lay::Marker *marker = dynamic_cast<lay::Marker *> (edit_marker ());
   if (marker) {
@@ -1267,14 +1372,25 @@
                         std::string ("  ly: ") +
                         tl::micron_to_string (m_points.back ().y () - m_points.end () [-2].y ()) + 
                         std::string ("  l: ") +
                         tl::micron_to_string (m_points.back ().distance (m_points.end () [-2])));
     }
 
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_shapes);
+    try {
+      deliver_shape_to_hooks (get_path ());
+    } catch (...) {
+      //  ignore exceptions
+    }
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_shapes);
+  }
 }
 
 db::Path 
 PathService::get_path () const
 {
   db::Path path;
 
@@ -1301,15 +1417,15 @@
 
   return path;
 }
 
 void 
 PathService::do_cancel_edit ()
 {
-  //  .. nothing yet ..
+  close_editor_hooks (false);
 }
 
 bool 
 PathService::selection_applies (const lay::ObjectInstPath &sel) const
 {
   return !sel.is_cell_inst () && sel.shape ().is_path ();
 }
@@ -1578,14 +1694,16 @@
   }
   std::sort (tv.begin (), tv.end ());
   tv.erase (std::unique (tv.begin (), tv.end ()), tv.end ());
   if (! tv.empty ()) {
     m_trans = db::VCplxTrans (1.0 / cv->layout ().dbu ()) * tv [0] * db::CplxTrans (cv->layout ().dbu ()) * cv.context_trans ();
   }
 
+  open_editor_hooks ();
+
   update_marker ();
 }
 
 std::pair<bool, db::cell_index_type> 
 InstService::make_cell (const lay::CellView &cv)
 {
   if (m_has_valid_cell) {
@@ -1752,28 +1870,28 @@
 
       //  check for recursive hierarchy
       const lay::CellView &cv = view ()->cellview (m_cv_index);
       std::set <db::cell_index_type> called, callers;
 
       cv->layout ().cell (inst.object ().cell_index ()).collect_called_cells (called);
       called.insert (inst.object ().cell_index ());
-      cv->layout ().cell (cv.cell_index ()).collect_caller_cells (callers);
+      cv.cell ()->collect_caller_cells (callers);
       callers.insert (cv.cell_index ());
 
       std::vector <db::cell_index_type> intersection;
       std::set_intersection (called.begin (), called.end (), callers.begin (), callers.end (), std::back_inserter (intersection));
       if (! intersection.empty ()) {
         throw tl::Exception (tl::to_string (tr ("Inserting this instance would create a recursive hierarchy")));
       }
 
       if (manager ()) {
         manager ()->transaction (tl::to_string (tr ("Create instance")), m_reference_transaction_id);
       }
       m_reference_transaction_id = 0;
-      db::Instance i = cv->layout ().cell (cv.cell_index ()).insert (inst);
+      db::Instance i = cv.cell ()->insert (inst);
       cv->layout ().cleanup ();
       if (manager ()) {
         manager ()->commit ();
       }
 
       commit_recent (view ());
 
@@ -1788,18 +1906,20 @@
 
       }
 
     }
 
     m_has_valid_cell = false;
     m_in_drag_drop = false;
+    close_editor_hooks (true);
 
   } catch (...) {
     m_has_valid_cell = false;
     m_in_drag_drop = false;
+    close_editor_hooks (false);
     throw;
   }
 }
 
 void 
 InstService::do_cancel_edit ()
 {
@@ -1815,14 +1935,16 @@
   set_edit_marker (0);
 
   //  clean up any proxy cells created so far 
   const lay::CellView &cv = view ()->cellview (m_cv_index);
   if (cv.is_valid ()) {
     cv->layout ().cleanup ();
   }
+
+  close_editor_hooks (false);
 }
 
 void
 InstService::service_configuration_changed ()
 {
   m_needs_update = true;
 }
@@ -2124,14 +2246,43 @@
     } else {
       marker->set ();
     }
 
   } else {
     set_edit_marker (0);
   }
+
+  //  call hooks with new shape
+  if (! editor_hooks ().empty ()) {
+
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::begin_new_instances);
+
+    try {
+
+      const lay::CellView &cv = view ()->cellview (m_cv_index);
+
+      db::CellInstArray inst;
+      if (cv.is_valid () && get_inst (inst)) {
+
+        //  Note: the instance collection is temporary
+        db::Instances instances (cv.cell ());
+        db::Instance i = instances.insert (inst);
+
+        db::CplxTrans view_trans = db::CplxTrans (cv->layout ().dbu ()) * m_trans;
+        call_editor_hooks<const db::Instance &, const db::CplxTrans &> (m_editor_hooks, &edt::EditorHooks::create_instance, i, view_trans);
+
+      }
+
+    } catch (...) {
+      //  ignore exceptions
+    }
+
+    call_editor_hooks (editor_hooks (), &edt::EditorHooks::end_new_instances);
+
+  }
 }
 
 bool
 InstService::get_inst (db::CellInstArray &inst) 
 {
   const lay::CellView &cv = view ()->cellview (m_cv_index);
   if (cv.is_valid ()) {
@@ -2155,10 +2306,40 @@
 
     }
 
   }
   return false;
 }
 
+void
+InstService::open_editor_hooks ()
+{
+  const lay::CellView &cv = view ()->cellview (m_cv_index);
+  if (! cv.is_valid ()) {
+    return;
+  }
+
+  std::string technology;
+  if (cv->layout ().technology ()) {
+    technology = cv->layout ().technology ()->name ();
+  }
+
+  m_editor_hooks = edt::EditorHooks::get_editor_hooks (technology);
+
+  lay::CellViewRef cv_ref (view ()->cellview_ref (m_cv_index));
+  call_editor_hooks<lay::CellViewRef &> (m_editor_hooks, &edt::EditorHooks::begin_create_instances, cv_ref);
+}
+
+void
+InstService::close_editor_hooks (bool with_commit)
+{
+  if (with_commit) {
+    call_editor_hooks (m_editor_hooks, &edt::EditorHooks::commit_instances);
+  }
+  call_editor_hooks (m_editor_hooks, &edt::EditorHooks::end_create_instances);
+
+  m_editor_hooks.clear ();
+}
+
 } // namespace edt
```

### Comparing `klayout-0.29.0/src/edt/edt/edtServiceImpl.h` & `klayout-0.29.1/src/edt/edt/edtServiceImpl.h`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 #ifndef HDR_edtServiceImpl
 #define HDR_edtServiceImpl
 
 #include "edtService.h"
 #include "edtConfig.h"
+#include "edtEditorHooks.h"
 
 #include <memory>
 
 namespace lay
 {
   class CellView;
   class LayoutViewBase;
@@ -64,23 +65,34 @@
 
 protected:
   std::pair <bool, db::DPoint> interpolate (const db::DPoint &m, const db::DPoint &o, const db::DPoint &p) const;
   void deliver_shape (const db::Polygon &poly);
   void deliver_shape (const db::Path &path);
   void deliver_shape (const db::Box &box);
   void deliver_shape (const db::Point &point);
+  void open_editor_hooks ();
+  template <class Shape>
+  void deliver_shape_to_hooks (const Shape &shape);
+  void close_editor_hooks (bool with_commit);
+
+  const tl::weak_collection<edt::EditorHooks> &editor_hooks ()
+  {
+    return m_editor_hooks;
+  }
+
   virtual void current_layer_changed () { }
 
 private:
   db::VCplxTrans m_trans;
   unsigned int m_layer;
   unsigned int m_cv_index;
   db::Cell *mp_cell;
   db::Layout *mp_layout;
   combine_mode_type m_combine_mode;
+  tl::weak_collection<edt::EditorHooks> m_editor_hooks;
 
   void update_edit_layer (const lay::LayerPropertiesConstIterator &iter);
 };
 
 /**
  *  @brief Implementation of edt::Service for polygon editing
  */
@@ -105,15 +117,15 @@
 private:
   std::vector <db::DPoint> m_points;
   bool m_closure_set;
   db::DPoint m_closure;
   db::DPoint m_last;
 
   void update_marker ();
-  db::Polygon get_polygon () const;
+  db::Polygon get_polygon (bool editing) const;
   void add_closure ();
   void set_last_point (const db::DPoint &p);
 };
 
 /**
  *  @brief Implementation of edt::Service for box editing
  */
@@ -294,20 +306,28 @@
   bool m_has_valid_cell;
   bool m_in_drag_drop;
   db::cell_index_type m_current_cell;
   db::Layout *mp_current_layout;
   const db::PCellDeclaration *mp_pcell_decl;
   int m_cv_index;
   db::ICplxTrans m_trans;
+  tl::weak_collection<edt::EditorHooks> m_editor_hooks;
 
   void update_marker ();
   bool get_inst (db::CellInstArray &inst);
   std::pair<bool, db::cell_index_type> make_cell (const lay::CellView &cv);
   tl::Variant get_default_layer_for_pcell ();
   void sync_to_config ();
   void switch_cell_or_pcell (bool switch_parameters);
+  void open_editor_hooks ();
+  void close_editor_hooks (bool with_commit);
+
+  const tl::weak_collection<edt::EditorHooks> &editor_hooks ()
+  {
+    return m_editor_hooks;
+  }
 };
 
 }
 
 #endif
```

### Comparing `klayout-0.29.0/src/edt/edt/edtUtils.cc` & `klayout-0.29.1/src/edt/edt/edtUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/edtUtils.h` & `klayout-0.29.1/src/edt/edt/edtUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/edt/edt/gsiDeclEdt.cc` & `klayout-0.29.1/src/edt/edt/gsiDeclEdt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsi.cc` & `klayout-0.29.1/src/gsi/gsi/gsi.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsi.h` & `klayout-0.29.1/src/gsi/gsi/gsi.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiCallback.h` & `klayout-0.29.1/src/gsi/gsi/gsiCallback.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiCallbackVar.h` & `klayout-0.29.1/src/gsi/gsi/gsiCallbackVar.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiClass.cc` & `klayout-0.29.1/src/gsi/gsi/gsiClass.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiClass.h` & `klayout-0.29.1/src/gsi/gsi/gsiClass.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiClassBase.cc` & `klayout-0.29.1/src/gsi/gsi/gsiClassBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiClassBase.h` & `klayout-0.29.1/src/gsi/gsi/gsiClassBase.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiCommon.h` & `klayout-0.29.1/src/gsi/gsi/gsiCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDecl.h` & `klayout-0.29.1/src/gsi/gsi/gsiDecl.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDeclBasic.cc` & `klayout-0.29.1/src/gsi/gsi/gsiDeclBasic.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDeclBasic.h` & `klayout-0.29.1/src/gsi/gsi/gsiDeclBasic.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDeclInternal.cc` & `klayout-0.29.1/src/gsi/gsi/gsiDeclInternal.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDeclTl.cc` & `klayout-0.29.1/src/gsi/gsi/gsiDeclTl.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiDeclTlPixelBuffer.cc` & `klayout-0.29.1/src/gsi/gsi/gsiDeclTlPixelBuffer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiEnums.h` & `klayout-0.29.1/src/gsi/gsi/gsiEnums.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiExpression.cc` & `klayout-0.29.1/src/gsi/gsi/gsiExpression.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiExpression.h` & `klayout-0.29.1/src/gsi/gsi/gsiExpression.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiExternalMain.cc` & `klayout-0.29.1/src/gsi/gsi/gsiExternalMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiExternalMain.h` & `klayout-0.29.1/src/gsi/gsi/gsiExternalMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiInspector.cc` & `klayout-0.29.1/src/gsi/gsi/gsiInspector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiInspector.h` & `klayout-0.29.1/src/gsi/gsi/gsiInspector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiInterpreter.cc` & `klayout-0.29.1/src/gsi/gsi/gsiInterpreter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiInterpreter.h` & `klayout-0.29.1/src/gsi/gsi/gsiInterpreter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiIterators.h` & `klayout-0.29.1/src/gsi/gsi/gsiIterators.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiMethods.cc` & `klayout-0.29.1/src/gsi/gsi/gsiMethods.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiMethods.h` & `klayout-0.29.1/src/gsi/gsi/gsiMethods.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiMethodsVar.h` & `klayout-0.29.1/src/gsi/gsi/gsiMethodsVar.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiObject.cc` & `klayout-0.29.1/src/gsi/gsi/gsiObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiObject.h` & `klayout-0.29.1/src/gsi/gsi/gsiObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiObjectHolder.cc` & `klayout-0.29.1/src/gsi/gsi/gsiObjectHolder.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiObjectHolder.h` & `klayout-0.29.1/src/gsi/gsi/gsiObjectHolder.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiSerialisation.cc` & `klayout-0.29.1/src/gsi/gsi/gsiSerialisation.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiSerialisation.h` & `klayout-0.29.1/src/gsi/gsi/gsiSerialisation.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiSignals.cc` & `klayout-0.29.1/src/gsi/gsi/gsiSignals.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiSignals.h` & `klayout-0.29.1/src/gsi/gsi/gsiSignals.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiTypes.cc` & `klayout-0.29.1/src/gsi/gsi/gsiTypes.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiTypes.h` & `klayout-0.29.1/src/gsi/gsi/gsiTypes.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiVariantArgs.cc` & `klayout-0.29.1/src/gsi/gsi/gsiVariantArgs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/gsi/gsi/gsiVariantArgs.h` & `klayout-0.29.1/src/gsi/gsi/gsiVariantArgs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/gsiDeclImg.cc` & `klayout-0.29.1/src/img/img/gsiDeclImg.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgCommon.h` & `klayout-0.29.1/src/img/img/imgCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgForceLink.cc` & `klayout-0.29.1/src/img/img/imgForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgForceLink.h` & `klayout-0.29.1/src/img/img/imgForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgLandmarksDialog.cc` & `klayout-0.29.1/src/img/img/imgLandmarksDialog.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgLandmarksDialog.h` & `klayout-0.29.1/src/img/img/imgLandmarksDialog.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgNavigator.cc` & `klayout-0.29.1/src/img/img/imgNavigator.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgNavigator.h` & `klayout-0.29.1/src/img/img/imgNavigator.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgObject.cc` & `klayout-0.29.1/src/img/img/imgObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgObject.h` & `klayout-0.29.1/src/img/img/imgObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgPlugin.cc` & `klayout-0.29.1/src/img/img/imgPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgPlugin.h` & `klayout-0.29.1/src/img/img/imgPlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgPropertiesPage.cc` & `klayout-0.29.1/src/img/img/imgPropertiesPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgPropertiesPage.h` & `klayout-0.29.1/src/img/img/imgPropertiesPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgService.cc` & `klayout-0.29.1/src/img/img/imgService.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgService.h` & `klayout-0.29.1/src/img/img/imgService.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgStream.cc` & `klayout-0.29.1/src/img/img/imgStream.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgStream.h` & `klayout-0.29.1/src/img/img/imgStream.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgWidgets.cc` & `klayout-0.29.1/src/img/img/imgWidgets.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/img/img/imgWidgets.h` & `klayout-0.29.1/src/img/img/imgWidgets.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/fixedFont.h` & `klayout-0.29.1/src/laybasic/laybasic/fixedFont.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayLayers.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayLayers.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayLayoutViewBase.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayLayoutViewBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayMarker.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayMarker.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayMenu.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayMenu.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayPlugin.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayRdbAdded.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayRdbAdded.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gsiDeclLayTlAdded.cc` & `klayout-0.29.1/src/laybasic/laybasic/gsiDeclLayTlAdded.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gtf.cc` & `klayout-0.29.1/src/laybasic/laybasic/gtf.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gtf.h` & `klayout-0.29.1/src/laybasic/laybasic/gtf.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/gtfdummy.cc` & `klayout-0.29.1/src/laybasic/laybasic/gtfdummy.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layAbstractMenu.cc` & `klayout-0.29.1/src/laybasic/laybasic/layAbstractMenu.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layAbstractMenu.h` & `klayout-0.29.1/src/laybasic/laybasic/layAbstractMenu.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layAnnotationShapes.cc` & `klayout-0.29.1/src/laybasic/laybasic/layAnnotationShapes.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layAnnotationShapes.h` & `klayout-0.29.1/src/laybasic/laybasic/layAnnotationShapes.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmap.cc` & `klayout-0.29.1/src/laybasic/laybasic/layBitmap.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmap.h` & `klayout-0.29.1/src/laybasic/laybasic/layBitmap.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmapRenderer.cc` & `klayout-0.29.1/src/laybasic/laybasic/layBitmapRenderer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmapRenderer.h` & `klayout-0.29.1/src/laybasic/laybasic/layBitmapRenderer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmapsToImage.cc` & `klayout-0.29.1/src/laybasic/laybasic/layBitmapsToImage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBitmapsToImage.h` & `klayout-0.29.1/src/laybasic/laybasic/layBitmapsToImage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBookmarkList.cc` & `klayout-0.29.1/src/laybasic/laybasic/layBookmarkList.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layBookmarkList.h` & `klayout-0.29.1/src/laybasic/laybasic/layBookmarkList.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCanvasPlane.cc` & `klayout-0.29.1/src/laybasic/laybasic/layCanvasPlane.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCanvasPlane.h` & `klayout-0.29.1/src/laybasic/laybasic/layCanvasPlane.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCellView.cc` & `klayout-0.29.1/src/laybasic/laybasic/layCellView.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCellView.h` & `klayout-0.29.1/src/laybasic/laybasic/layCellView.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layColorPalette.cc` & `klayout-0.29.1/src/laybasic/laybasic/layColorPalette.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layColorPalette.h` & `klayout-0.29.1/src/laybasic/laybasic/layColorPalette.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layConverters.cc` & `klayout-0.29.1/src/laybasic/laybasic/layConverters.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layConverters.h` & `klayout-0.29.1/src/laybasic/laybasic/layConverters.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCursor.cc` & `klayout-0.29.1/src/laybasic/laybasic/layCursor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layCursor.h` & `klayout-0.29.1/src/laybasic/laybasic/layCursor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDispatcher.cc` & `klayout-0.29.1/src/laybasic/laybasic/layDispatcher.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDispatcher.h` & `klayout-0.29.1/src/laybasic/laybasic/layDispatcher.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDisplayState.cc` & `klayout-0.29.1/src/laybasic/laybasic/layDisplayState.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDisplayState.h` & `klayout-0.29.1/src/laybasic/laybasic/layDisplayState.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDitherPattern.cc` & `klayout-0.29.1/src/laybasic/laybasic/layDitherPattern.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDitherPattern.h` & `klayout-0.29.1/src/laybasic/laybasic/layDitherPattern.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDragDropData.cc` & `klayout-0.29.1/src/laybasic/laybasic/layDragDropData.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDragDropData.h` & `klayout-0.29.1/src/laybasic/laybasic/layDragDropData.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDrawing.cc` & `klayout-0.29.1/src/laybasic/laybasic/layDrawing.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layDrawing.h` & `klayout-0.29.1/src/laybasic/laybasic/layDrawing.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layEditable.cc` & `klayout-0.29.1/src/laybasic/laybasic/layEditable.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layEditable.h` & `klayout-0.29.1/src/laybasic/laybasic/layEditable.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layEditorServiceBase.cc` & `klayout-0.29.1/src/laybasic/laybasic/layEditorServiceBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layEditorServiceBase.h` & `klayout-0.29.1/src/laybasic/laybasic/layEditorServiceBase.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layFinder.cc` & `klayout-0.29.1/src/laybasic/laybasic/layFinder.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layFinder.h` & `klayout-0.29.1/src/laybasic/laybasic/layFinder.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layFixedFont.cc` & `klayout-0.29.1/src/laybasic/laybasic/layFixedFont.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layFixedFont.h` & `klayout-0.29.1/src/laybasic/laybasic/layFixedFont.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayerProperties.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLayerProperties.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayerProperties.h` & `klayout-0.29.1/src/laybasic/laybasic/layLayerProperties.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayoutCanvas.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLayoutCanvas.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayoutCanvas.h` & `klayout-0.29.1/src/laybasic/laybasic/layLayoutCanvas.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayoutViewBase.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLayoutViewBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayoutViewBase.h` & `klayout-0.29.1/src/laybasic/laybasic/layLayoutViewBase.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLayoutViewConfig.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLayoutViewConfig.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLineStylePalette.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLineStylePalette.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLineStylePalette.h` & `klayout-0.29.1/src/laybasic/laybasic/layLineStylePalette.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLineStyles.cc` & `klayout-0.29.1/src/laybasic/laybasic/layLineStyles.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layLineStyles.h` & `klayout-0.29.1/src/laybasic/laybasic/layLineStyles.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMargin.cc` & `klayout-0.29.1/src/laybasic/laybasic/layMargin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMargin.h` & `klayout-0.29.1/src/laybasic/laybasic/layMargin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMarker.cc` & `klayout-0.29.1/src/laybasic/laybasic/layMarker.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMarker.h` & `klayout-0.29.1/src/laybasic/laybasic/layMarker.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMouseTracker.cc` & `klayout-0.29.1/src/laybasic/laybasic/layMouseTracker.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMouseTracker.h` & `klayout-0.29.1/src/laybasic/laybasic/layMouseTracker.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMove.cc` & `klayout-0.29.1/src/laybasic/laybasic/layMove.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layMove.h` & `klayout-0.29.1/src/laybasic/laybasic/layMove.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layNativePlugin.cc` & `klayout-0.29.1/src/laybasic/laybasic/layNativePlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layNativePlugin.h` & `klayout-0.29.1/src/laybasic/laybasic/layNativePlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layNetColorizer.cc` & `klayout-0.29.1/src/laybasic/laybasic/layNetColorizer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layNetColorizer.h` & `klayout-0.29.1/src/laybasic/laybasic/layNetColorizer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layObjectInstPath.cc` & `klayout-0.29.1/src/laybasic/laybasic/layObjectInstPath.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layObjectInstPath.h` & `klayout-0.29.1/src/laybasic/laybasic/layObjectInstPath.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layParsedLayerSource.cc` & `klayout-0.29.1/src/laybasic/laybasic/layParsedLayerSource.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layParsedLayerSource.h` & `klayout-0.29.1/src/laybasic/laybasic/layParsedLayerSource.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPixelBufferPainter.cc` & `klayout-0.29.1/src/laybasic/laybasic/layPixelBufferPainter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPixelBufferPainter.h` & `klayout-0.29.1/src/laybasic/laybasic/layPixelBufferPainter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPlugin.cc` & `klayout-0.29.1/src/laybasic/laybasic/layPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPlugin.h` & `klayout-0.29.1/src/laybasic/laybasic/layPlugin.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPluginConfigPage.cc` & `klayout-0.29.1/src/laybasic/laybasic/layPluginConfigPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layPluginConfigPage.h` & `klayout-0.29.1/src/laybasic/laybasic/layPluginConfigPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layProperties.cc` & `klayout-0.29.1/src/laybasic/laybasic/layProperties.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layProperties.h` & `klayout-0.29.1/src/laybasic/laybasic/layProperties.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawLayerInfo.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawLayerInfo.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawLayerInfo.h` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawLayerInfo.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThread.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThread.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThread.h` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThread.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadCanvas.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadCanvas.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadCanvas.h` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadCanvas.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadWorker.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadWorker.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRedrawThreadWorker.h` & `klayout-0.29.1/src/laybasic/laybasic/layRedrawThreadWorker.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRenderer.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRenderer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRenderer.h` & `klayout-0.29.1/src/laybasic/laybasic/layRenderer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRubberBox.cc` & `klayout-0.29.1/src/laybasic/laybasic/layRubberBox.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layRubberBox.h` & `klayout-0.29.1/src/laybasic/laybasic/layRubberBox.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laySelector.cc` & `klayout-0.29.1/src/laybasic/laybasic/laySelector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laySelector.h` & `klayout-0.29.1/src/laybasic/laybasic/laySelector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laySnap.cc` & `klayout-0.29.1/src/laybasic/laybasic/laySnap.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laySnap.h` & `klayout-0.29.1/src/laybasic/laybasic/laySnap.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layStipplePalette.cc` & `klayout-0.29.1/src/laybasic/laybasic/layStipplePalette.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layStipplePalette.h` & `klayout-0.29.1/src/laybasic/laybasic/layStipplePalette.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layStream.cc` & `klayout-0.29.1/src/laybasic/laybasic/layStream.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layStream.h` & `klayout-0.29.1/src/laybasic/laybasic/layStream.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layTextInfo.cc` & `klayout-0.29.1/src/laybasic/laybasic/layTextInfo.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layTextInfo.h` & `klayout-0.29.1/src/laybasic/laybasic/layTextInfo.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layUtils.cc` & `klayout-0.29.1/src/laybasic/laybasic/layUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layUtils.h` & `klayout-0.29.1/src/laybasic/laybasic/layUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewObject.cc` & `klayout-0.29.1/src/laybasic/laybasic/layViewObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewObject.h` & `klayout-0.29.1/src/laybasic/laybasic/layViewObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewOp.cc` & `klayout-0.29.1/src/laybasic/laybasic/layViewOp.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewOp.h` & `klayout-0.29.1/src/laybasic/laybasic/layViewOp.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewport.cc` & `klayout-0.29.1/src/laybasic/laybasic/layViewport.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layViewport.h` & `klayout-0.29.1/src/laybasic/laybasic/layViewport.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layZoomBox.cc` & `klayout-0.29.1/src/laybasic/laybasic/layZoomBox.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/layZoomBox.h` & `klayout-0.29.1/src/laybasic/laybasic/layZoomBox.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laybasicCommon.h` & `klayout-0.29.1/src/laybasic/laybasic/laybasicCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laybasicConfig.h` & `klayout-0.29.1/src/laybasic/laybasic/laybasicConfig.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laybasicForceLink.cc` & `klayout-0.29.1/src/laybasic/laybasic/laybasicForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/laybasic/laybasic/laybasicForceLink.h` & `klayout-0.29.1/src/laybasic/laybasic/laybasicForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/gsiDeclLayAdditional.cc` & `klayout-0.29.1/src/layview/layview/gsiDeclLayAdditional.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/gsiDeclLayLayoutView_noqt.cc` & `klayout-0.29.1/src/layview/layview/gsiDeclLayLayoutView_noqt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/gsiDeclLayLayoutView_qt.cc` & `klayout-0.29.1/src/layview/layview/gsiDeclLayLayoutView_qt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layGridNet.cc` & `klayout-0.29.1/src/layview/layview/layGridNet.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layGridNet.h` & `klayout-0.29.1/src/layview/layview/layGridNet.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layGridNetConfigPage.cc` & `klayout-0.29.1/src/layview/layview/layGridNetConfigPage.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layGridNetConfigPage.h` & `klayout-0.29.1/src/layview/layview/layGridNetConfigPage.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layLayoutView.h` & `klayout-0.29.1/src/layview/layview/layLayoutView.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layLayoutView_noqt.cc` & `klayout-0.29.1/src/layview/layview/layLayoutView_noqt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layLayoutView_noqt.h` & `klayout-0.29.1/src/layview/layview/layLayoutView_noqt.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layLayoutView_qt.cc` & `klayout-0.29.1/src/layview/layview/layLayoutView_qt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layLayoutView_qt.h` & `klayout-0.29.1/src/layview/layview/layLayoutView_qt.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layviewCommon.h` & `klayout-0.29.1/src/layview/layview/layviewCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layviewForceLink.cc` & `klayout-0.29.1/src/layview/layview/layviewForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/layview/layview/layviewForceLink.h` & `klayout-0.29.1/src/layview/layview/layviewForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasic.cc` & `klayout-0.29.1/src/lib/lib/libBasic.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicArc.cc` & `klayout-0.29.1/src/lib/lib/libBasicArc.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicArc.h` & `klayout-0.29.1/src/lib/lib/libBasicArc.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicCircle.cc` & `klayout-0.29.1/src/lib/lib/libBasicCircle.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicCircle.h` & `klayout-0.29.1/src/lib/lib/libBasicCircle.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicDonut.cc` & `klayout-0.29.1/src/lib/lib/libBasicDonut.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicDonut.h` & `klayout-0.29.1/src/lib/lib/libBasicDonut.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicEllipse.cc` & `klayout-0.29.1/src/lib/lib/libBasicEllipse.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicEllipse.h` & `klayout-0.29.1/src/lib/lib/libBasicEllipse.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicPie.cc` & `klayout-0.29.1/src/lib/lib/libBasicPie.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicPie.h` & `klayout-0.29.1/src/lib/lib/libBasicPie.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicRoundPath.cc` & `klayout-0.29.1/src/lib/lib/libBasicRoundPath.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicRoundPath.h` & `klayout-0.29.1/src/lib/lib/libBasicRoundPath.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicRoundPolygon.cc` & `klayout-0.29.1/src/lib/lib/libBasicRoundPolygon.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicRoundPolygon.h` & `klayout-0.29.1/src/lib/lib/libBasicRoundPolygon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicStrokedPolygon.cc` & `klayout-0.29.1/src/lib/lib/libBasicStrokedPolygon.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicStrokedPolygon.h` & `klayout-0.29.1/src/lib/lib/libBasicStrokedPolygon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicText.cc` & `klayout-0.29.1/src/lib/lib/libBasicText.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libBasicText.h` & `klayout-0.29.1/src/lib/lib/libBasicText.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libCommon.h` & `klayout-0.29.1/src/lib/lib/libCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libForceLink.cc` & `klayout-0.29.1/src/lib/lib/libForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lib/lib/libForceLink.h` & `klayout-0.29.1/src/lib/lib/libForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/gsiDeclLymMacro.cc` & `klayout-0.29.1/src/lym/lym/gsiDeclLymMacro.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymCommon.h` & `klayout-0.29.1/src/lym/lym/lymCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymForceLink.cc` & `klayout-0.29.1/src/lym/lym/lymForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymForceLink.h` & `klayout-0.29.1/src/lym/lym/lymForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacro.cc` & `klayout-0.29.1/src/lym/lym/lymMacro.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacro.h` & `klayout-0.29.1/src/lym/lym/lymMacro.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacroCollection.cc` & `klayout-0.29.1/src/lym/lym/lymMacroCollection.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacroCollection.h` & `klayout-0.29.1/src/lym/lym/lymMacroCollection.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacroInterpreter.cc` & `klayout-0.29.1/src/lym/lym/lymMacroInterpreter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/lym/lym/lymMacroInterpreter.h` & `klayout-0.29.1/src/lym/lym/lymMacroInterpreter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/common/dbPluginCommon.h` & `klayout-0.29.1/src/plugins/common/dbPluginCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/common/layPluginCommon.h` & `klayout-0.29.1/src/plugins/common/layPluginCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIF.cc` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIF.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIF.h` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIF.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFFormat.h` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFFormat.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFReader.cc` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFReader.h` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFWriter.cc` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/dbCIFWriter.h` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/dbCIFWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/cif/db_plugin/gsiDeclDbCIF.cc` & `klayout-0.29.1/src/plugins/streamers/cif/db_plugin/gsiDeclDbCIF.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXF.cc` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXF.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXF.h` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXF.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFFormat.h` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFFormat.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFReader.cc` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFReader.h` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.cc` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.h` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/dbDXFWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/dxf/db_plugin/gsiDeclDbDXF.cc` & `klayout-0.29.1/src/plugins/streamers/dxf/db_plugin/gsiDeclDbDXF.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Converter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Text.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2Text.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/contrib/dbGDS2TextWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Format.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Format.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Reader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2ReaderBase.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2Writer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.h` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/dbGDS2WriterBase.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/gds2/db_plugin/gsiDeclDbGDS2.cc` & `klayout-0.29.1/src/plugins/streamers/gds2/db_plugin/gsiDeclDbGDS2.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.cc` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.h` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbDEFImporter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.cc` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.h` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFImporter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFPlugin.cc` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFDEFPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.cc` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.h` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/dbLEFImporter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/lefdef/db_plugin/gsiDeclDbLEFDEF.cc` & `klayout-0.29.1/src/plugins/streamers/lefdef/db_plugin/gsiDeclDbLEFDEF.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAG.cc` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAG.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAG.h` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAG.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGFormat.h` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGFormat.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGReader.cc` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGReader.h` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGWriter.cc` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/dbMAGWriter.h` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/dbMAGWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/magic/db_plugin/gsiDeclDbMAG.cc` & `klayout-0.29.1/src/plugins/streamers/magic/db_plugin/gsiDeclDbMAG.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASIS.cc` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASIS.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASIS.h` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASIS.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISFormat.h` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISFormat.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISReader.cc` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISReader.h` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.cc` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.h` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/dbOASISWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/oasis/db_plugin/gsiDeclDbOASIS.cc` & `klayout-0.29.1/src/plugins/streamers/oasis/db_plugin/gsiDeclDbOASIS.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.cc` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.h` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberDrillFileReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.cc` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.h` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImportData.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.cc` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.h` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbGerberImporter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.cc` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.h` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XApertures.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.cc` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.h` & `klayout-0.29.1/src/plugins/streamers/pcb/db_plugin/dbRS274XReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.cc` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.h` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.cc` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.h` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerIO.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/dbNetTracerPlugin.cc` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/dbNetTracerPlugin.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/plugins/tools/net_tracer/db_plugin/gsiDeclDbNetTracer.cc` & `klayout-0.29.1/src/plugins/tools/net_tracer/db_plugin/gsiDeclDbNetTracer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/gsiDeclPya.cc` & `klayout-0.29.1/src/pya/pya/gsiDeclPya.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pya.cc` & `klayout-0.29.1/src/pya/pya/pya.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pya.h` & `klayout-0.29.1/src/pya/pya/pya.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaCallables.cc` & `klayout-0.29.1/src/pya/pya/pyaCallables.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaCallables.h` & `klayout-0.29.1/src/pya/pya/pyaCallables.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaCommon.h` & `klayout-0.29.1/src/pya/pya/pyaCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaConvert.cc` & `klayout-0.29.1/src/pya/pya/pyaConvert.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaConvert.h` & `klayout-0.29.1/src/pya/pya/pyaConvert.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaHelpers.cc` & `klayout-0.29.1/src/pya/pya/pyaHelpers.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaHelpers.h` & `klayout-0.29.1/src/pya/pya/pyaHelpers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaInspector.cc` & `klayout-0.29.1/src/pya/pya/pyaInspector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaInspector.h` & `klayout-0.29.1/src/pya/pya/pyaInspector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaInternal.cc` & `klayout-0.29.1/src/pya/pya/pyaInternal.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaInternal.h` & `klayout-0.29.1/src/pya/pya/pyaInternal.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaMarshal.cc` & `klayout-0.29.1/src/pya/pya/pyaMarshal.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaMarshal.h` & `klayout-0.29.1/src/pya/pya/pyaMarshal.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaModule.cc` & `klayout-0.29.1/src/pya/pya/pyaModule.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaModule.h` & `klayout-0.29.1/src/pya/pya/pyaModule.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaObject.cc` & `klayout-0.29.1/src/pya/pya/pyaObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaObject.h` & `klayout-0.29.1/src/pya/pya/pyaObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaRefs.cc` & `klayout-0.29.1/src/pya/pya/pyaRefs.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaRefs.h` & `klayout-0.29.1/src/pya/pya/pyaRefs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaSignalHandler.cc` & `klayout-0.29.1/src/pya/pya/pyaSignalHandler.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaSignalHandler.h` & `klayout-0.29.1/src/pya/pya/pyaSignalHandler.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaStatusChangedListener.cc` & `klayout-0.29.1/src/pya/pya/pyaStatusChangedListener.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaStatusChangedListener.h` & `klayout-0.29.1/src/pya/pya/pyaStatusChangedListener.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaUtils.cc` & `klayout-0.29.1/src/pya/pya/pyaUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pya/pya/pyaUtils.h` & `klayout-0.29.1/src/pya/pya/pyaUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtCore/QtCoreMain.cc` & `klayout-0.29.1/src/pymod/QtCore/QtCoreMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtCore/QtCoreMain.h` & `klayout-0.29.1/src/pymod/QtCore/QtCoreMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtCore5Compat/QtCore5CompatMain.cc` & `klayout-0.29.1/src/pymod/QtCore5Compat/QtCore5CompatMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtCore5Compat/QtCore5CompatMain.h` & `klayout-0.29.1/src/pymod/QtCore5Compat/QtCore5CompatMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtDesigner/QtDesignerMain.cc` & `klayout-0.29.1/src/pymod/QtDesigner/QtDesignerMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtDesigner/QtDesignerMain.h` & `klayout-0.29.1/src/pymod/QtDesigner/QtDesignerMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtGui/QtGuiMain.cc` & `klayout-0.29.1/src/pymod/QtGui/QtGuiMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtGui/QtGuiMain.h` & `klayout-0.29.1/src/pymod/QtGui/QtGuiMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtMultimedia/QtMultimediaMain.cc` & `klayout-0.29.1/src/pymod/QtMultimedia/QtMultimediaMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtMultimedia/QtMultimediaMain.h` & `klayout-0.29.1/src/pymod/QtMultimedia/QtMultimediaMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtNetwork/QtNetworkMain.cc` & `klayout-0.29.1/src/pymod/QtNetwork/QtNetworkMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtNetwork/QtNetworkMain.h` & `klayout-0.29.1/src/pymod/QtNetwork/QtNetworkMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtPrintSupport/QtPrintSupportMain.cc` & `klayout-0.29.1/src/pymod/QtPrintSupport/QtPrintSupportMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtPrintSupport/QtPrintSupportMain.h` & `klayout-0.29.1/src/pymod/QtPrintSupport/QtPrintSupportMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtSql/QtSqlMain.cc` & `klayout-0.29.1/src/pymod/QtSql/QtSqlMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtSql/QtSqlMain.h` & `klayout-0.29.1/src/pymod/QtSql/QtSqlMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtSvg/QtSvgMain.cc` & `klayout-0.29.1/src/pymod/QtSvg/QtSvgMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtSvg/QtSvgMain.h` & `klayout-0.29.1/src/pymod/QtSvg/QtSvgMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtUiTools/QtUiToolsMain.cc` & `klayout-0.29.1/src/pymod/QtUiTools/QtUiToolsMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtUiTools/QtUiToolsMain.h` & `klayout-0.29.1/src/pymod/QtUiTools/QtUiToolsMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtWidgets/QtWidgetsMain.cc` & `klayout-0.29.1/src/pymod/QtWidgets/QtWidgetsMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtWidgets/QtWidgetsMain.h` & `klayout-0.29.1/src/pymod/QtWidgets/QtWidgetsMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtXml/QtXmlMain.cc` & `klayout-0.29.1/src/pymod/QtXml/QtXmlMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtXml/QtXmlMain.h` & `klayout-0.29.1/src/pymod/QtXml/QtXmlMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtXmlPatterns/QtXmlPatternsMain.cc` & `klayout-0.29.1/src/pymod/QtXmlPatterns/QtXmlPatternsMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/QtXmlPatterns/QtXmlPatternsMain.h` & `klayout-0.29.1/src/pymod/QtXmlPatterns/QtXmlPatternsMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/ant/antMain.cc` & `klayout-0.29.1/src/pymod/ant/antMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/ant/antMain.h` & `klayout-0.29.1/src/pymod/ant/antMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/bridge_sample/bridge_sample.cc` & `klayout-0.29.1/src/pymod/bridge_sample/bridge_sample.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/db/dbMain.cc` & `klayout-0.29.1/src/pymod/db/dbMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/db/dbMain.h` & `klayout-0.29.1/src/pymod/db/dbMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/db/__init__.py` & `klayout-0.29.1/src/pymod/distutils_src/klayout/db/__init__.py`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/db/pcell_declaration_helper.py` & `klayout-0.29.1/src/pymod/distutils_src/klayout/db/pcell_declaration_helper.py`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/dbcore.pyi` & `klayout-0.29.1/src/pymod/distutils_src/klayout/dbcore.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,28 @@
         @brief Returns a string representing this box
 
         This string can be turned into a box again by using \from_s
         . If a DBU is given, the output units will be micrometers.
 
         The DBU argument has been added in version 0.27.6.
         """
+    def __sub__(self, box: Box) -> Box:
+        r"""
+        @brief Subtraction of boxes
+
+
+        The - operator subtracts the argument box from self.
+        This will return the bounding box of the are covered by self, but not by argument box. Subtracting a box from itself will render an empty box. Subtracting another box from self will modify the first box only if the argument box covers one side entirely.
+
+        @param box The box to subtract from this box.
+
+        @return The result box
+
+        This feature has been introduced in version 0.29.
+        """
     def _create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
     def _destroy(self) -> None:
         r"""
@@ -3937,20 +3951,20 @@
         def new(cls, s: str) -> CompoundRegionOperationNode.GeometricalOp:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -3975,20 +3989,20 @@
         def __lt__(self, other: int) -> bool:
             r"""
             @brief Returns true if the enum is less (in the enum symbol order) than the integer value
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums for inequality
+            @brief Compares an enum with an integer for inequality
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer for inequality
+            @brief Compares two enums for inequality
             """
         def __repr__(self) -> str:
             r"""
             @brief Converts an enum to a visual string
             """
         def __str__(self) -> str:
             r"""
@@ -4145,20 +4159,20 @@
         def new(cls, s: str) -> CompoundRegionOperationNode.ParameterType:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -4387,20 +4401,20 @@
         def __lt__(self, other: int) -> bool:
             r"""
             @brief Returns true if the enum is less (in the enum symbol order) than the integer value
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums for inequality
+            @brief Compares an enum with an integer for inequality
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer for inequality
+            @brief Compares two enums for inequality
             """
         def __repr__(self) -> str:
             r"""
             @brief Converts an enum to a visual string
             """
         def __str__(self) -> str:
             r"""
@@ -4473,30 +4487,34 @@
         """
     @classmethod
     def new_convex_decomposition(cls, input: CompoundRegionOperationNode, mode: PreferredOrientation) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node providing a composition into convex pieces.
         """
     @classmethod
-    def new_corners_as_dots(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool) -> CompoundRegionOperationNode:
+    def new_corners_as_dots(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool, inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node turning corners into dots (single-point edges).
+
+        'absolute' and 'inverse' arguments have been added in version 0.29.1.
         """
     @classmethod
-    def new_corners_as_edge_pairs(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool) -> CompoundRegionOperationNode:
+    def new_corners_as_edge_pairs(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool, inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node turning corners into edge pairs containing the two edges adjacent to the corner.
         The first edge will be the incoming edge and the second one the outgoing edge.
 
-        This feature has been introduced in version 0.27.1.
+        This feature has been introduced in version 0.27.1. 'absolute' and 'inverse' arguments have been added in version 0.29.1.
         """
     @classmethod
-    def new_corners_as_rectangles(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool, dim: int) -> CompoundRegionOperationNode:
+    def new_corners_as_rectangles(cls, input: CompoundRegionOperationNode, angle_min: float, include_angle_min: bool, angle_max: float, include_angle_max: bool, dim: int, inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node turning corners into rectangles.
+
+        'absolute' and 'inverse' arguments have been added in version 0.29.1.
         """
     @classmethod
     def new_count_filter(cls, inputs: CompoundRegionOperationNode, invert: Optional[bool] = ..., min_count: Optional[int] = ..., max_count: Optional[int] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node selecting results but their shape count.
         """
     @classmethod
@@ -4506,17 +4524,19 @@
         """
     @classmethod
     def new_edge_length_sum_filter(cls, input: CompoundRegionOperationNode, inverse: Optional[bool] = ..., lmin: Optional[int] = ..., lmax: Optional[int] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node filtering edges by their length sum (over the local set).
         """
     @classmethod
-    def new_edge_orientation_filter(cls, input: CompoundRegionOperationNode, inverse: bool, amin: float, include_amin: bool, amax: float, include_amax: bool) -> CompoundRegionOperationNode:
+    def new_edge_orientation_filter(cls, input: CompoundRegionOperationNode, inverse: bool, amin: float, include_amin: bool, amax: float, include_amax: bool, absolute_angle: Optional[bool] = ...) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node filtering edges by their orientation.
+
+        'absolute_angle' has been introduced in version 0.29.1.
         """
     @classmethod
     def new_edge_pair_to_first_edges(cls, input: CompoundRegionOperationNode) -> CompoundRegionOperationNode:
         r"""
         @brief Creates a node delivering the first edge of each edges pair.
         """
     @classmethod
@@ -4906,14 +4926,16 @@
     Intra-layer connections make nets begin propagated along different shapes on the same net. Without the intra-layer connections, nets are not propagated over shape boundaries. As this is usually intended, intra-layer connections should always be specified for each layer.
 
     Inter-layer connections connect shapes on different layers. Shapes which touch across layers will be connected if their layers are specified as being connected through inter-layer \connect.
 
     All layers are specified in terms of layer indexes. Layer indexes are layout layer indexes (see \Layout class).
 
     The connectivity object also manages the global nets. Global nets are substrate for example and they are propagated automatically from subcircuits to circuits. Global nets are defined by name and are managed through IDs. To get the name for a given ID, use \global_net_name.
+    Starting with version 0.29, soft connections are supported. Soft connections attach to high-ohmic substrate or diffusion layers (the 'lower' layer) are upon netlist extraction it will be checked that no wiring is routed over such connections. See \soft_connect and \soft_global_connect for details.
+
     This class has been introduced in version 0.26.
     """
     @classmethod
     def new(cls) -> Connectivity:
         r"""
         @brief Creates a new object of this class
         """
@@ -4925,14 +4947,22 @@
         r"""
         @brief Creates a copy of self
         """
     def __init__(self) -> None:
         r"""
         @brief Creates a new object of this class
         """
+    def __repr__(self) -> str:
+        r"""
+        @hide
+        """
+    def __str__(self) -> str:
+        r"""
+        @hide
+        """
     def _create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
     def _destroy(self) -> None:
         r"""
@@ -4970,19 +5000,21 @@
         r"""
         @brief Assigns another object to self
         """
     @overload
     def connect(self, layer: int) -> None:
         r"""
         @brief Specifies intra-layer connectivity.
+        This method specifies a hard connection between shapes on the given layer. Without specifying such a connection, shapes on that layer do not form connection regions.
         """
     @overload
     def connect(self, layer_a: int, layer_b: int) -> None:
         r"""
         @brief Specifies inter-layer connectivity.
+        This method specifies a hard connection between shapes on layer_a and layer_b.
         """
     def connect_global(self, layer: int, global_net_name: str) -> int:
         r"""
         @brief Connects the given layer to the global net given by name.
         Returns the ID of the global net.
         """
     def create(self) -> None:
@@ -5016,14 +5048,35 @@
         """
     def is_const_object(self) -> bool:
         r"""
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
+    def soft_connect(self, layer_a: int, layer_b: int) -> None:
+        r"""
+        @brief Specifies a soft connection between layer_a and layer_b.
+        @param layer_a The 'upper' layer
+        @param layer_b The 'lower' layer
+        Soft connections are made between a lower and an upper layer. The lower layer conceptually is a high-ohmic (i.e. substrate, diffusion) region that is not intended for signal wiring. The netlist extraction will check that no routing happens over such regions.
+
+        Soft connections have in introduced in version 0.29.
+        """
+    def soft_connect_global(self, layer: int, global_net_name: str) -> int:
+        r"""
+        @brief Soft-connects the given layer to the global net given by name.
+        Returns the ID of the global net.
+        See \soft_connect for a description of the soft connection feature. The global net is always the 'lower' (i.e. high-ohmic, substrate) part of the soft connection.
+
+        Soft connections have in introduced in version 0.29.
+        """
+    def to_s(self) -> str:
+        r"""
+        @hide
+        """
 
 class CplxTrans:
     r"""
     @brief A complex transformation
 
     A complex transformation provides magnification, mirroring at the x-axis, rotation by an arbitrary
     angle and a displacement. This is also the order, the operations are applied.
@@ -6285,14 +6338,28 @@
         @brief Returns a string representing this box
 
         This string can be turned into a box again by using \from_s
         . If a DBU is given, the output units will be micrometers.
 
         The DBU argument has been added in version 0.27.6.
         """
+    def __sub__(self, box: DBox) -> DBox:
+        r"""
+        @brief Subtraction of boxes
+
+
+        The - operator subtracts the argument box from self.
+        This will return the bounding box of the are covered by self, but not by argument box. Subtracting a box from itself will render an empty box. Subtracting another box from self will modify the first box only if the argument box covers one side entirely.
+
+        @param box The box to subtract from this box.
+
+        @return The result box
+
+        This feature has been introduced in version 0.29.
+        """
     def _create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
     def _destroy(self) -> None:
         r"""
@@ -11442,16 +11509,15 @@
     @brief Gets the vertical alignment
 
     See \valign= for a description of this property.
 
     Setter:
     @brief Sets the vertical alignment
 
-    This property specifies how the text is aligned relative to the anchor point. 
-    This property has been introduced in version 0.22 and extended to enums in 0.28.
+    This is the version accepting integer values. It's provided for backward compatibility.
     """
     x: float
     r"""
     Getter:
     @brief Gets the x location of the text
 
     This method has been introduced in version 0.23.
@@ -17030,20 +17096,20 @@
     def __deepcopy__(self) -> EdgeMode:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer value
+        @brief Compares two enums
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums
+        @brief Compares an enum with an integer value
         """
     def __hash__(self) -> int:
         r"""
         @brief Gets the hash value from the enum
         """
     @overload
     def __init__(self, i: int) -> None:
@@ -19061,14 +19127,49 @@
         Does not modify the edge pair collection but returns the transformed edge pairs.
 
         @param t The transformation to apply.
 
         @return The transformed edge pairs.
         """
     @overload
+    def with_abs_angle(self, angle: float, inverse: bool) -> EdgePairs:
+        r"""
+        @brief Filter the edge pairs by orientation of their edges
+
+        This method behaves like \with_angle, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
+    def with_abs_angle(self, min_angle: float, max_angle: float, inverse: bool, include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> EdgePairs:
+        r"""
+        @brief Filter the edge pairs by orientation of their edges
+
+        This method behaves like \with_angle, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
+    def with_abs_angle_both(self, angle: float, inverse: bool) -> EdgePairs:
+        r"""
+        @brief Filter the edge pairs by orientation of both of their edges
+
+        This method behaves like \with_angle_both, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
+    def with_abs_angle_both(self, min_angle: float, max_angle: float, inverse: bool, include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> EdgePairs:
+        r"""
+
+        This method behaves like \with_angle_both, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
     def with_angle(self, angle: float, inverse: bool) -> EdgePairs:
         r"""
         @brief Filter the edge pairs by orientation of their edges
         Filters the edge pairs in the edge pair collection by orientation. If "inverse" is false, only edge pairs with at least one edge having the given angle to the x-axis are returned. If "inverse" is true, edge pairs not fulfilling this criterion are returned.
 
         This will filter edge pairs with at least one horizontal edge:
 
@@ -19270,14 +19371,21 @@
         @brief Filters the edge pairs by length of both of their edges
         Filters the edge pairs in the edge pair collection by length of both of their edges. If "inverse" is false, only edge pairs with both edges having a length between min_length and max_length (excluding max_length itself) are returned. If "inverse" is true, edge pairs not fulfilling this criterion are returned.
 
         If you don't want to specify a lower or upper limit, pass nil to that parameter.
 
         This method has been added in version 0.27.1.
         """
+    def write(self, filename: str) -> None:
+        r"""
+        @brief Writes the region to a file
+        This method is provided for debugging purposes. It writes the object to a flat layer 0/0 in a single top cell.
+
+        This method has been introduced in version 0.29.
+        """
 
 class EdgeProcessor:
     r"""
     @brief The edge processor (boolean, sizing, merge)
 
     The edge processor implements the boolean and edge set operations (size, merge). Because the edge processor might allocate resources which can be reused in later operations, it is implemented as an object that can be used several times.
 
@@ -20561,20 +20669,20 @@
         def new(cls, s: str) -> Edges.EdgeType:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -22783,14 +22891,32 @@
         Use nil for this value to select the default.
 
         "min_projection" and "max_projection" allow selecting edges by their projected value upon each other. It is sufficient if the projection of one edge on the other matches the specified condition. The projected length must be larger or equal to "min_projection" and less than "max_projection". If you don't want to specify one threshold, pass nil to the respective value.
 
         'zero_distance_mode' has been added in version 0.29.
         """
     @overload
+    def with_abs_angle(self, angle: float, inverse: bool) -> Edges:
+        r"""
+        @brief Filter the edges by orientation
+
+        This method behaves like \with_angle, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
+    def with_abs_angle(self, min_angle: float, max_angle: float, inverse: bool, include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> Edges:
+        r"""
+        @brief Filter the edges by orientation
+
+        This method behaves like \with_angle, but angles are always positive - i.e. there is no differentiation between edges sloping 'down' vs. edges sloping 'up.
+
+        This method has been added in version 0.29.1.
+        """
+    @overload
     def with_angle(self, angle: float, inverse: bool) -> Edges:
         r"""
         @brief Filters the edges by orientation
         Filters the edges in the edge collection by orientation. If "inverse" is false, only edges which have the given angle to the x-axis are returned. If "inverse" is true, edges not having the given angle are returned.
 
         This will select horizontal edges:
 
@@ -22828,14 +22954,21 @@
     def with_length(self, min_length: Any, max_length: Any, inverse: bool) -> Edges:
         r"""
         @brief Filters the edges by length
         Filters the edges in the edge collection by length. If "inverse" is false, only edges which have a length larger or equal to "min_length" and less than "max_length" are returned. If "inverse" is true, edges not having a length less than "min_length" or larger or equal than "max_length" are returned.
 
         If you don't want to specify a lower or upper limit, pass nil to that parameter.
         """
+    def write(self, filename: str) -> None:
+        r"""
+        @brief Writes the region to a file
+        This method is provided for debugging purposes. It writes the object to a flat layer 0/0 in a single top cell.
+
+        This method has been introduced in version 0.29.
+        """
     def xor(self, other: Edges) -> Edges:
         r"""
         @brief Returns the boolean XOR between self and the other edge collection
 
         @return The result of the boolean XOR operation
 
         The boolean XOR operation will return all parts of the edges in this and the other collection except the parts where both are coincident.
@@ -25541,32 +25674,32 @@
     a: Vector
     r"""
     Getter:
     @brief Returns the displacement vector for the 'a' axis
 
     Starting with version 0.25 the displacement is of vector type.
     Setter:
-    @brief Sets the displacement vector for the 'a' axis in micrometer units
+    @brief Sets the displacement vector for the 'a' axis
 
-    Like \a= with an integer displacement, this method will set the displacement vector but it accepts a vector in micrometer units that is of \DVector type. The vector will be translated to database units internally.
+    If the instance was not an array instance before it is made one.
 
-    This method has been introduced in version 0.25.
+    This method has been introduced in version 0.23. Starting with version 0.25 the displacement is of vector type.
     """
     b: Vector
     r"""
     Getter:
     @brief Returns the displacement vector for the 'b' axis
 
     Starting with version 0.25 the displacement is of vector type.
     Setter:
-    @brief Sets the displacement vector for the 'b' axis in micrometer units
+    @brief Sets the displacement vector for the 'b' axis
 
-    Like \b= with an integer displacement, this method will set the displacement vector but it accepts a vector in micrometer units that is of \DVector type. The vector will be translated to database units internally.
+    If the instance was not an array instance before it is made one.
 
-    This method has been introduced in version 0.25.
+    This method has been introduced in version 0.23. Starting with version 0.25 the displacement is of vector type.
     """
     cell: Cell
     r"""
     Getter:
     @brief Gets the \Cell object of the cell this instance refers to
 
     Please note that before version 0.23 this method returned the cell the instance is contained in. For consistency, this method has been renamed \parent_cell.
@@ -25601,18 +25734,17 @@
     """
     cplx_trans: ICplxTrans
     r"""
     Getter:
     @brief Gets the complex transformation of the instance or the first instance in the array
     This method is always valid compared to \trans, since simple transformations can be expressed as complex transformations as well.
     Setter:
-    @brief Sets the complex transformation of the instance or the first instance in the array (in micrometer units)
-    This method sets the transformation the same way as \cplx_trans=, but the displacement of this transformation is given in micrometer units. It is internally translated into database units.
+    @brief Sets the complex transformation of the instance or the first instance in the array
 
-    This method has been introduced in version 0.25.
+    This method has been introduced in version 0.23.
     """
     da: DVector
     r"""
     Getter:
     @brief Returns the displacement vector for the 'a' axis in micrometer units
 
     Like \a, this method returns the displacement, but it will be translated to database units internally.
@@ -25733,17 +25865,18 @@
     """
     trans: Trans
     r"""
     Getter:
     @brief Gets the transformation of the instance or the first instance in the array
     The transformation returned is only valid if the array does not represent a complex transformation array
     Setter:
-    @brief Sets the transformation of the instance or the first instance in the array
+    @brief Sets the transformation of the instance or the first instance in the array (in micrometer units)
+    This method sets the transformation the same way as \cplx_trans=, but the displacement of this transformation is given in micrometer units. It is internally translated into database units.
 
-    This method has been introduced in version 0.23.
+    This method has been introduced in version 0.25.
     """
     @classmethod
     def new(cls) -> Instance:
         r"""
         @brief Creates a new object of this class
         """
     def __copy__(self) -> Instance:
@@ -30879,20 +31012,20 @@
         def __lt__(self, other: int) -> bool:
             r"""
             @brief Returns true if the enum is less (in the enum symbol order) than the integer value
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer for inequality
+            @brief Compares two enums for inequality
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums for inequality
+            @brief Compares an enum with an integer for inequality
             """
         def __repr__(self) -> str:
             r"""
             @brief Converts an enum to a visual string
             """
         def __str__(self) -> str:
             r"""
@@ -30974,14 +31107,21 @@
     Setter:
     @brief Sets a flag indicating whether to include floating subcircuits in the netlist.
 
     With 'include_floating_subcircuits' set to true, subcircuits with no connection to their parent circuit are still included in the circuit as floating subcircuits. Specifically on flattening this means that these subcircuits are properly propagated to their parent instead of appearing as additional top circuits.
 
     This attribute has been introduced in version 0.27 and replaces the arguments of \extract_netlist.
     """
+    make_soft_connection_diodes: bool
+    r"""
+    Getter:
+    @hide
+    Setter:
+    @hide
+    """
     max_vertex_count: int
     r"""
     Getter:
     See \max_vertex_count= for details about this attribute.
     Setter:
     @brief Sets the max_vertex_count parameter for the hierarchical network processor
     This parameter controls splitting of large polygons in order to enhance performance
@@ -31377,14 +31517,15 @@
         This method returns the ID of the global net. Use \global_net_name to get the name back from the ID.
         """
     @overload
     def connect_global(self, l: Texts, global_net_name: str) -> int:
         r"""
         @brief Defines a connection of the given text layer with a global net.
         This method returns the ID of the global net. Use \global_net_name to get the name back from the ID.
+
         This variant has been introduced in version 0.27.
         """
     def const_cell_mapping_into(self, layout: Layout, cell: Cell) -> CellMapping:
         r"""
         @brief Creates a cell mapping for copying shapes from the internal layout to the given target layout.
         This version will not create new cells in the target layout.
         If the required cells do not exist there yet, flatting will happen.
@@ -31716,14 +31857,64 @@
         r"""
         @brief Sends all shapes of a specific net and layer to the given Shapes container.
         If 'recursive'' is true, the returned region will contain the shapes of
         all subcircuits too.
         "prop_id" is an optional properties ID. If given, this property set will be attached to the shapes.
         The optional 'trans' parameter allows applying a transformation to all shapes. It has been introduced in version 0.28.4.
         """
+    @overload
+    def soft_connect(self, a: Region, b: Region) -> None:
+        r"""
+        @brief Defines an inter-layer connection for the given layers in soft mode.
+        Connects two layers through a soft connection.
+        Soft connections cannot make connections between two different nets.
+        These are directional connections where 'b' is the 'lower' layer (typically high-ohmic substrate or diffusion).
+
+        Soft connections have been introduced in version 0.29.
+        """
+    @overload
+    def soft_connect(self, a: Region, b: Texts) -> None:
+        r"""
+        @brief Defines an inter-layer connection for the given layers in soft mode.
+        Connects two layers through a soft connection.
+        Soft connections cannot make connections between two different nets.
+        These are directional connections where 'b' is the 'lower' layer (typically high-ohmic substrate or diffusion).
+        As one argument is a (hierarchical) text collection, this method is used to attach net labels to polygons.
+
+        Soft connections have been introduced in version 0.29.
+        """
+    @overload
+    def soft_connect(self, a: Texts, b: Region) -> None:
+        r"""
+        @brief Defines an inter-layer connection for the given layers in soft mode.
+        Connects two layers through a soft connection.
+        Soft connections cannot make connections between two different nets.
+        These are directional connections where 'b' is the 'lower' layer (typically high-ohmic substrate or diffusion).
+        As one argument is a (hierarchical) text collection, this method is used to attach net labels to polygons.
+
+        Soft connections have been introduced in version 0.29.
+        """
+    @overload
+    def soft_connect_global(self, l: Region, global_net_name: str) -> int:
+        r"""
+        @brief Defines a connection of the given layer with a global net in soft mode.
+        This method returns the ID of the global net. Use \global_net_name to get the name back from the ID.
+        Soft connections are directional, where the global net is the 'lower' layer (typically high-ohmic substrate or diffusion).
+
+        Soft connections have been introduced in version 0.29.
+        """
+    @overload
+    def soft_connect_global(self, l: Texts, global_net_name: str) -> int:
+        r"""
+        @brief Defines a connection of the given text layer with a global net in soft mode.
+        This method returns the ID of the global net. Use \global_net_name to get the name back from the ID.
+        Soft connections are directional, where the global net is the 'lower' layer (typically high-ohmic substrate or diffusion).
+
+        Soft connections have been introduced in version 0.29.
+        """
     def write(self, path: str, short_format: Optional[bool] = ...) -> None:
         r"""
         @brief Writes the extracted netlist to a file.
         This method employs the native format of KLayout.
         """
     def write_l2n(self, path: str, short_format: Optional[bool] = ...) -> None:
         r"""
@@ -32063,16 +32254,14 @@
     def dup(self) -> Library:
         r"""
         @brief Creates a copy of self
         """
     def for_technologies(self) -> bool:
         r"""
         @brief Returns a value indicating whether the library is associated with any technology.
-        The method is equivalent to checking whether the \technologies list is empty.
-
         This method has been introduced in version 0.27
         """
     def id(self) -> int:
         r"""
         @brief Returns the library's ID
         The ID is set when the library is registered and cannot be changed 
         """
@@ -32081,14 +32270,16 @@
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
     def is_for_technology(self, tech: str) -> bool:
         r"""
         @brief Returns a value indicating whether the library is associated with the given technology.
+        The method is equivalent to checking whether the \technologies list is empty.
+
         This method has been introduced in version 0.27
         """
     def layout(self) -> Layout:
         r"""
         @brief The layout object where the cells reside that this library defines
         """
     def layout_const(self) -> Layout:
@@ -32172,20 +32363,20 @@
         def new(cls, s: str) -> LoadLayoutOptions.CellConflictResolution:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -35162,24 +35353,24 @@
         @brief Returns a value indicating whether the object was already destroyed
         This method returns true, if the object was destroyed, either explicitly or by the C++ side.
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
     @overload
     def device(self) -> Device:
         r"""
-        @brief Gets the device reference.
+        @brief Gets the device reference (non-const version).
         Gets the device object that this connection is made to.
+
+        This constness variant has been introduced in version 0.26.8
         """
     @overload
     def device(self) -> Device:
         r"""
-        @brief Gets the device reference (non-const version).
+        @brief Gets the device reference.
         Gets the device object that this connection is made to.
-
-        This constness variant has been introduced in version 0.26.8
         """
     def device_class(self) -> DeviceClass:
         r"""
         @brief Gets the class of the device which is addressed.
         """
     def dup(self) -> NetTerminalRef:
         r"""
@@ -35190,22 +35381,22 @@
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
     @overload
     def net(self) -> Net:
         r"""
-        @brief Gets the net this terminal reference is attached to.
+        @brief Gets the net this terminal reference is attached to (non-const version).
+
+        This constness variant has been introduced in version 0.26.8
         """
     @overload
     def net(self) -> Net:
         r"""
-        @brief Gets the net this terminal reference is attached to (non-const version).
-
-        This constness variant has been introduced in version 0.26.8
+        @brief Gets the net this terminal reference is attached to.
         """
     def terminal_def(self) -> DeviceTerminalDefinition:
         r"""
         @brief Gets the terminal definition of the terminal that is connected
         """
     def terminal_id(self) -> int:
         r"""
@@ -35960,24 +36151,24 @@
         The name pattern is a glob expression. For example, 'blank_circuit("np*")' will blank out all circuits with names starting with 'np'.
 
         For more details see \Circuit#blank which is the corresponding method on the actual object.
         """
     @overload
     def circuit_by_cell_index(self, cell_index: int) -> Circuit:
         r"""
-        @brief Gets the circuit object for a given cell index.
+        @brief Gets the circuit object for a given cell index (const version).
         If the cell index is not valid or no circuit is registered with this index, nil is returned.
+
+        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def circuit_by_cell_index(self, cell_index: int) -> Circuit:
         r"""
-        @brief Gets the circuit object for a given cell index (const version).
+        @brief Gets the circuit object for a given cell index.
         If the cell index is not valid or no circuit is registered with this index, nil is returned.
-
-        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def circuit_by_name(self, name: str) -> Circuit:
         r"""
         @brief Gets the circuit object for a given name (const version).
         If the name is not a valid circuit name, nil is returned.
 
@@ -36058,38 +36249,38 @@
         @brief Iterates over the circuits of the netlist (const version)
 
         This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def each_circuit_bottom_up(self) -> Iterator[Circuit]:
         r"""
-        @brief Iterates over the circuits bottom-up (const version)
+        @brief Iterates over the circuits bottom-up
         Iterating bottom-up means the parent circuits come after the child circuits. This is the basically the reverse order as delivered by \each_circuit_top_down.
-
-        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def each_circuit_bottom_up(self) -> Iterator[Circuit]:
         r"""
-        @brief Iterates over the circuits bottom-up
+        @brief Iterates over the circuits bottom-up (const version)
         Iterating bottom-up means the parent circuits come after the child circuits. This is the basically the reverse order as delivered by \each_circuit_top_down.
+
+        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def each_circuit_top_down(self) -> Iterator[Circuit]:
         r"""
-        @brief Iterates over the circuits top-down
+        @brief Iterates over the circuits top-down (const version)
         Iterating top-down means the parent circuits come before the child circuits. The first \top_circuit_count circuits are top circuits - i.e. those which are not referenced by other circuits.
+
+        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def each_circuit_top_down(self) -> Iterator[Circuit]:
         r"""
-        @brief Iterates over the circuits top-down (const version)
+        @brief Iterates over the circuits top-down
         Iterating top-down means the parent circuits come before the child circuits. The first \top_circuit_count circuits are top circuits - i.e. those which are not referenced by other circuits.
-
-        This constness variant has been introduced in version 0.26.8.
         """
     @overload
     def each_device_class(self) -> Iterator[DeviceClass]:
         r"""
         @brief Iterates over the device classes of the netlist
         """
     @overload
@@ -38516,20 +38707,20 @@
         def new(cls, s: str) -> PCellParameterState.ParameterStateIcon:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -41832,20 +42023,20 @@
     def __deepcopy__(self) -> PreferredOrientation:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums
+        @brief Compares an enum with an integer value
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer value
+        @brief Compares two enums
         """
     def __hash__(self) -> int:
         r"""
         @brief Gets the hash value from the enum
         """
     @overload
     def __init__(self, i: int) -> None:
@@ -41870,20 +42061,20 @@
     def __lt__(self, other: int) -> bool:
         r"""
         @brief Returns true if the enum is less (in the enum symbol order) than the integer value
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums for inequality
+        @brief Compares an enum with an integer for inequality
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer for inequality
+        @brief Compares two enums for inequality
         """
     def __repr__(self) -> str:
         r"""
         @brief Converts an enum to a visual string
         """
     def __str__(self) -> str:
         r"""
@@ -42029,20 +42220,20 @@
     def __deepcopy__(self) -> PropertyConstraint:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer value
+        @brief Compares two enums
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums
+        @brief Compares an enum with an integer value
         """
     def __hash__(self) -> int:
         r"""
         @brief Gets the hash value from the enum
         """
     @overload
     def __init__(self, i: int) -> None:
@@ -42067,20 +42258,20 @@
     def __lt__(self, other: int) -> bool:
         r"""
         @brief Returns true if the enum is less (in the enum symbol order) than the integer value
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer for inequality
+        @brief Compares two enums for inequality
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums for inequality
+        @brief Compares an enum with an integer for inequality
         """
     def __repr__(self) -> str:
         r"""
         @brief Converts an enum to a visual string
         """
     def __str__(self) -> str:
         r"""
@@ -42763,14 +42954,30 @@
     iter.select_cells("MACRO")
     @/code
 
     Cell selection is done using cell indexes or glob pattern. Glob pattern are equivalent to the usual file name wildcards used on various command line shells. For example "A*" matches all cells starting with an "A". The curly brace notation and character classes are supported as well. For example "C{125,512}" matches "C125" and "C512" and "[ABC]*" matches all cells starting with an "A", a "B" or "C". "[^ABC]*" matches all cells not starting with one of that letters.
 
     The RecursiveShapeIterator class has been introduced in version 0.18 and has been extended substantially in 0.23.
     """
+    for_merged_input: bool
+    r"""
+    Getter:
+    @brief Gets a flag indicating whether iterator optimizes for merged input
+
+    see \for_merged_input= for details of this attribute.
+
+    This method has been introduced in version 0.29.
+
+    Setter:
+    @brief Sets a flag indicating whether iterator optimizes for merged input
+
+    If this flag is set to true, the iterator is allowed to skip shapes it deems irrelevant because they are covered entirely by other shapes. This allows shortcutting hierarchy traversal in some cases.
+
+    This method has been introduced in version 0.29.
+    """
     global_dtrans: DCplxTrans
     r"""
     Getter:
     @brief Gets the global transformation to apply to all shapes delivered (in micrometer units)
     See also \global_dtrans=.
 
     This method has been introduced in version 0.27.
@@ -43509,20 +43716,20 @@
         def new(cls, s: str) -> Region.OppositeFilter:
             r"""
             @brief Creates an enum from a string value
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer value
+            @brief Compares two enums
             """
         @overload
         def __eq__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums
+            @brief Compares an enum with an integer value
             """
         def __hash__(self) -> int:
             r"""
             @brief Gets the hash value from the enum
             """
         @overload
         def __init__(self, i: int) -> None:
@@ -43547,20 +43754,20 @@
         def __lt__(self, other: int) -> bool:
             r"""
             @brief Returns true if the enum is less (in the enum symbol order) than the integer value
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares an enum with an integer for inequality
+            @brief Compares two enums for inequality
             """
         @overload
         def __ne__(self, other: object) -> bool:
             r"""
-            @brief Compares two enums for inequality
+            @brief Compares an enum with an integer for inequality
             """
         def __repr__(self) -> str:
             r"""
             @brief Converts an enum to a visual string
             """
         def __str__(self) -> str:
             r"""
@@ -44093,19 +44300,33 @@
         r = RBA::Region::new(layout.begin_shapes(cell, layer), RBA::ICplxTrans::new(layout.dbu / dbu))
         @/code
         """
     @overload
     @classmethod
     def new(cls, shapes: Shapes) -> Region:
         r"""
-        @brief Shapes constructor
+        @brief Constructor from a shapes container
 
-        This constructor creates a region from a \Shapes collection.
+        This constructor creates a region from the shapes container.
+        Text objects and edges are not inserted, because they cannot be converted to polygons.
+        This method allows feeding the shapes from a hierarchy of cells into the region.
 
-        This constructor has been introduced in version 0.25.
+        This constructor has been introduced in version 0.25 and extended in version 0.29.
+        """
+    @overload
+    @classmethod
+    def new(cls, shapes: Shapes, trans: ICplxTrans) -> Region:
+        r"""
+        @brief Constructor from a shapes container with a transformation
+
+        This constructor creates a region from the shapes container after applying the transformation.
+        Text objects and edges are not inserted, because they cannot be converted to polygons.
+        This method allows feeding the shapes from a hierarchy of cells into the region.
+
+        This constructor variant has been introduced in version 0.29.
         """
     def __add__(self, other: Region) -> Region:
         r"""
         @brief Returns the combined region of self and the other region
 
         @return The resulting region
 
@@ -44310,19 +44531,32 @@
         dbu    = 0.1 # the target database unit
         r = RBA::Region::new(layout.begin_shapes(cell, layer), RBA::ICplxTrans::new(layout.dbu / dbu))
         @/code
         """
     @overload
     def __init__(self, shapes: Shapes) -> None:
         r"""
-        @brief Shapes constructor
+        @brief Constructor from a shapes container
 
-        This constructor creates a region from a \Shapes collection.
+        This constructor creates a region from the shapes container.
+        Text objects and edges are not inserted, because they cannot be converted to polygons.
+        This method allows feeding the shapes from a hierarchy of cells into the region.
 
-        This constructor has been introduced in version 0.25.
+        This constructor has been introduced in version 0.25 and extended in version 0.29.
+        """
+    @overload
+    def __init__(self, shapes: Shapes, trans: ICplxTrans) -> None:
+        r"""
+        @brief Constructor from a shapes container with a transformation
+
+        This constructor creates a region from the shapes container after applying the transformation.
+        Text objects and edges are not inserted, because they cannot be converted to polygons.
+        This method allows feeding the shapes from a hierarchy of cells into the region.
+
+        This constructor variant has been introduced in version 0.29.
         """
     def __ior__(self, other: Region) -> Region:
         r"""
         @brief Performs the boolean OR between self and the other region in-place (modifying self)
 
         @return The region after modification (self)
 
@@ -44517,44 +44751,47 @@
     def complex_op(self, node: CompoundRegionOperationNode, property_constraint: Optional[PropertyConstraint] = ...) -> Any:
         r"""
         @brief Executes a complex operation (see \CompoundRegionOperationNode for details)
 
         This method has been introduced in version 0.27.
         The 'property_constraint' parameter controls whether properties are considered: with 'SamePropertiesConstraint' the operation is only applied between shapes with identical properties. With 'DifferentPropertiesConstraint' only between shapes with different properties. This option has been introduced in version 0.28.4.
         """
-    def corners(self, angle_min: Optional[float] = ..., angle_max: Optional[float] = ..., dim: Optional[int] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> Region:
+    def corners(self, angle_min: Optional[float] = ..., angle_max: Optional[float] = ..., dim: Optional[int] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ..., inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> Region:
         r"""
         @brief This method will select all corners whose attached edges satisfy the angle condition.
 
         The angle values specify a range of angles: all corners whose attached edges form an angle between angle_min and angle_max will be reported boxes with 2*dim x 2*dim dimension. The default dimension is 2x2 DBU.
 
         If 'include_angle_min' is true, the angle condition is >= min. angle, otherwise it is > min. angle. Same for 'include_angle_,ax' and the max. angle.
 
-        The angle is measured between the incoming and the outcoming edge in mathematical sense: a positive value is a turn left while a negative value is a turn right. Since polygon contours are oriented clockwise, positive angles will report concave corners while negative ones report convex ones.
+        With 'absolute' set to false (the default), the angle is measured between the incoming and the outcoming edge in mathematical sense: a positive value is a turn left while a negative value is a turn right. Since polygon contours are oriented clockwise, positive angles will report concave corners while negative ones report convex ones.
+        With the 'absolute' option set to true, there is no such distinction and angle values are always positive.
+
+        With 'inverse' set to true, the method will select corners not meeting the angle criterion.
 
         A similar function that reports corners as point-like edges is \corners_dots.
 
-        This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27.
+        This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27. 'inverse' and 'absolute' have been added in version 0.29.1.
         """
-    def corners_dots(self, angle_start: Optional[float] = ..., angle_end: Optional[float] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> Edges:
+    def corners_dots(self, angle_start: Optional[float] = ..., angle_end: Optional[float] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ..., inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> Edges:
         r"""
         @brief This method will select all corners whose attached edges satisfy the angle condition.
 
         This method is similar to \corners, but delivers an \Edges collection with dot-like edges for each corner.
 
-        This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27.
+        This method has been introduced in version 0.25. 'include_min_angle' and 'include_max_angle' have been added in version 0.27. 'inverse' and 'absolute' have been added in version 0.29.1.
         """
-    def corners_edge_pairs(self, angle_start: Optional[float] = ..., angle_end: Optional[float] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ...) -> EdgePairs:
+    def corners_edge_pairs(self, angle_start: Optional[float] = ..., angle_end: Optional[float] = ..., include_min_angle: Optional[bool] = ..., include_max_angle: Optional[bool] = ..., inverse: Optional[bool] = ..., absolute: Optional[bool] = ...) -> EdgePairs:
         r"""
         @brief This method will select all corners whose attached edges satisfy the angle condition.
 
         This method is similar to \corners, but delivers an \EdgePairs collection with an edge pairs for each corner.
         The first edge is the incoming edge of the corner, the second one the outgoing edge.
 
-        This method has been introduced in version 0.27.1.
+        This method has been introduced in version 0.27.1. 'inverse' and 'absolute' have been added in version 0.29.1.
         """
     def count(self) -> int:
         r"""
         @brief Returns the (flat) number of polygons in the region
 
         This returns the number of raw polygons (not merged polygons if merged semantics is enabled).
         The count is computed 'as if flat', i.e. polygons inside a cell are multiplied by the number of times a cell is instantiated.
@@ -44657,14 +44894,26 @@
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
     def disable_progress(self) -> None:
         r"""
         @brief Disable progress reporting
         Calling this method will disable progress reporting. See \enable_progress.
         """
+    def drc_hull(self, metrics: Metrics, space: int, n_circle: Optional[int] = ...) -> Region:
+        r"""
+        @brief Computes a visualization of the forbidden region for a DRC space check
+
+        @param metrics The metrics to apply
+        @param space The space value to apply
+        @param n_circle The full-circle number of points for the Euclidian space visualization
+
+        @return The new polygons representing the forbidden region.
+
+        This method has been introduced in version 0.29.1.
+        """
     def dup(self) -> Region:
         r"""
         @brief Creates a copy of self
         """
     def each(self) -> Iterator[Polygon]:
         r"""
         @brief Returns each polygon of the region
@@ -46764,14 +47013,21 @@
 
         With 'inverse' set to false, this version filters polygons which have a relative height equal to the given value. With 'inverse' set to true, all other polygons will be returned.
 
         Merged semantics applies for this method (see \merged_semantics= for a description of this concept)
 
         This method has been introduced in version 0.27.
         """
+    def write(self, filename: str) -> None:
+        r"""
+        @brief Writes the region to a file
+        This method is provided for debugging purposes. It writes the object to a flat layer 0/0 in a single top cell.
+
+        This method has been introduced in version 0.29.
+        """
     def xor(self, other: Region) -> Region:
         r"""
         @brief Returns the boolean XOR between self and the other region
 
         @return The result of the boolean XOR operation
 
         This method will compute the boolean XOR (intersection) between two regions. The result is often but not necessarily always merged.
@@ -47503,20 +47759,20 @@
     def __lt__(self, other: int) -> bool:
         r"""
         @brief Returns true if the enum is less (in the enum symbol order) than the integer value
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums for inequality
+        @brief Compares an enum with an integer for inequality
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer for inequality
+        @brief Compares two enums for inequality
         """
     def __repr__(self) -> str:
         r"""
         @brief Converts an enum to a visual string
         """
     def __str__(self) -> str:
         r"""
@@ -48237,18 +48493,19 @@
     text: Any
     r"""
     Getter:
     @brief Returns the text object
 
     Starting with version 0.23, this method returns nil, if the shape does not represent a text.
     Setter:
-    @brief Replaces the shape by the given text (in micrometer units)
-    This method replaces the shape by the given text, like \text= with a \Text argument does. This version translates the text from micrometer units to database units internally.
+    @brief Replaces the shape by the given text object
+    This method replaces the shape by the given text object. This method can only be called for editable layouts. It does not change the user properties of the shape.
+    Calling this method will invalidate any iterators. It should not be called inside a loop iterating over shapes.
 
-    This method has been introduced in version 0.25.
+    This method has been introduced in version 0.22.
     """
     text_dpos: DVector
     r"""
     Getter:
     @brief Gets the text's position in micrometer units
 
     Applies to texts only. Will throw an exception if the object is not a text.
@@ -48529,18 +48786,34 @@
     def __eq__(self, other: object) -> bool:
         r"""
         @brief Equality operator
 
         Equality of shapes is not specified by the identity of the objects but by the
         identity of the pointers - both shapes must refer to the same object.
         """
+    def __hash__(self) -> int:
+        r"""
+        @brief Hash function
+
+        The hash function enables Shape objects as keys in hashes.
+
+        This method has been introduced in version 0.29.1.
+        """
     def __init__(self) -> None:
         r"""
         @brief Creates a new object of this class
         """
+    def __lt__(self, other: Shape) -> bool:
+        r"""
+        @brief Less operator
+
+        The less operator implementation is based on pointers and not strictly reproducible.However, it is good enough so Shape objects can serve as keys in hashes (see also \hash).
+
+        This method has been introduced in version 0.29.1.
+        """
     def __ne__(self, other: object) -> bool:
         r"""
         @brief Inequality operator
         """
     def __repr__(self) -> str:
         r"""
         @brief Create a string showing the contents of the reference
@@ -48668,14 +48941,22 @@
         r"""
         @brief Returns the perimeter of the shape in micrometer units
 
         This method will return an approximation of the perimeter for paths.
 
         This method has been added in version 0.25.
         """
+    def drectangle(self) -> Any:
+        r"""
+        @brief Gets the rectangle in micron units if the object represents one or nil if not
+
+        If the shape represents a rectangle - i.e. a box or box polygon, a path with two points and no round ends - this method returns the box. If not, nil is returned.
+
+        This method has been introduced in version 0.29.
+        """
     def dup(self) -> Shape:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def each_dedge(self) -> Iterator[DEdge]:
         r"""
@@ -48764,14 +49045,22 @@
         This method applies to polygons and delivers all points of the polygon hull contour.
         It will throw an exception for other objects.
         """
     def has_prop_id(self) -> bool:
         r"""
         @brief Returns true, if the shape has properties, i.e. has a properties ID
         """
+    def hash(self) -> int:
+        r"""
+        @brief Hash function
+
+        The hash function enables Shape objects as keys in hashes.
+
+        This method has been introduced in version 0.29.1.
+        """
     def holes(self) -> int:
         r"""
         @brief Returns the number of holes
 
         This method applies to polygons and will throw an exception for other objects..
         Simple polygons deliver a value of zero.
         """
@@ -48878,14 +49167,22 @@
         """
     def property(self, key: Any) -> Any:
         r"""
         @brief Gets the user property with the given key
         This method is a convenience method that gets the property with the given key. If no property with that key does not exist, it will return nil. Using that method is more convenient than using the layout object and the properties ID to retrieve the property value. 
         This method has been introduced in version 0.22.
         """
+    def rectangle(self) -> Any:
+        r"""
+        @brief Gets the rectangle if the object represents one or nil if not
+
+        If the shape represents a rectangle - i.e. a box or box polygon, a path with two points and no round ends - this method returns the box. If not, nil is returned.
+
+        This method has been introduced in version 0.29.
+        """
     def set_property(self, key: Any, value: Any) -> None:
         r"""
         @brief Sets the user property with the given key to the given value
         This method is a convenience method that sets the property with the given key to the given value. If no property with that key exists, it will create one. Using that method is more convenient than creating a new property set with a new ID and assigning that properties ID.
         This method may change the properties ID. Note: GDS only supports integer keys. OASIS supports numeric and string keys. Calling this method will invalidate any iterators. It should not be called inside a loop iterating over shapes.
 
         This method has been introduced in version 0.22.
@@ -51444,39 +51741,39 @@
         Calling this method will make this object no longer owned by the script's memory management. Instead, the object must be managed in some other way. Usually this method may be called if it is known that some C++ object holds and manages this object. Technically speaking, this method will turn the script's reference into a weak reference. After the script engine decides to delete the reference, the object itself will still exist. If the object is not managed otherwise, memory leaks will occur.
 
         Usually it's not required to call this method. It has been introduced in version 0.24.
         """
     @overload
     def circuit(self) -> Circuit:
         r"""
-        @brief Gets the circuit the subcircuit lives in.
-        This is NOT the circuit which is referenced. For getting the circuit that the subcircuit references, use \circuit_ref.
-        """
-    @overload
-    def circuit(self) -> Circuit:
-        r"""
         @brief Gets the circuit the subcircuit lives in (non-const version).
         This is NOT the circuit which is referenced. For getting the circuit that the subcircuit references, use \circuit_ref.
 
         This constness variant has been introduced in version 0.26.8
         """
     @overload
-    def circuit_ref(self) -> Circuit:
+    def circuit(self) -> Circuit:
         r"""
-        @brief Gets the circuit referenced by the subcircuit.
+        @brief Gets the circuit the subcircuit lives in.
+        This is NOT the circuit which is referenced. For getting the circuit that the subcircuit references, use \circuit_ref.
         """
     @overload
     def circuit_ref(self) -> Circuit:
         r"""
         @brief Gets the circuit referenced by the subcircuit (non-const version).
 
 
         This constness variant has been introduced in version 0.26.8
         """
     @overload
+    def circuit_ref(self) -> Circuit:
+        r"""
+        @brief Gets the circuit referenced by the subcircuit.
+        """
+    @overload
     def connect_pin(self, pin: Pin, net: Net) -> None:
         r"""
         @brief Connects the given pin to the specified net.
         This version takes a \Pin reference instead of a pin ID.
         """
     @overload
     def connect_pin(self, pin_id: int, net: Net) -> None:
@@ -51572,14 +51869,15 @@
 
     See \default_grids for details.
 
     This property has been introduced in version 0.28.17.
     Setter:
     @brief Sets the default grids
     If not empty, this list replaces the global grid list for this technology.
+    Note that this method will reset the default grid (see \default_grid). Use \set_default_grids to set the default grids and the strong default one.
 
     This property has been introduced in version 0.28.17.
     """
     description: str
     r"""
     Getter:
     @brief Gets the description
@@ -51826,14 +52124,25 @@
         See \base_path for details about the default base path.
         """
     def create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
+    def default_grid(self) -> float:
+        r"""
+        @brief Gets the default grid
+
+        The default grid is a specific one from the default grid list.
+        It indicates the one that is taken if the current grid is not matching one of the default grids.
+
+        To set the default grid, use \set_default_grids.
+
+        This property has been introduced in version 0.29.
+        """
     def destroy(self) -> None:
         r"""
         @brief Explicitly destroys the object
         Explicitly destroys the object on C++ side if it was owned by the script interpreter. Subsequent access to this object will throw an exception.
         If the object is not owned by the script, this method will do nothing.
         """
     def destroyed(self) -> bool:
@@ -51868,14 +52177,22 @@
         r"""
         @brief Loads the technology definition from a file
         """
     def save(self, file: str) -> None:
         r"""
         @brief Saves the technology definition to a file
         """
+    def set_default_grids(self, grids: Sequence[float], default_grid: Optional[float] = ...) -> None:
+        r"""
+        @brief Sets the default grids and the strong default one
+        See \default_grids and \default_grid for a description of this property.
+        Note that the default grid has to be a member of the 'grids' array to become active.
+
+        This method has been introduced in version 0.29.
+        """
     def to_xml(self) -> str:
         r"""
         @brief Returns a XML representation of this technolog
 
         \technology_from_xml can be used to restore the technology definition.
         """
 
@@ -52064,15 +52381,16 @@
     @brief Gets the vertical alignment
 
     See \valign= for a description of this property.
 
     Setter:
     @brief Sets the vertical alignment
 
-    This is the version accepting integer values. It's provided for backward compatibility.
+    This property specifies how the text is aligned relative to the anchor point. 
+    This property has been introduced in version 0.22 and extended to enums in 0.28.
     """
     x: int
     r"""
     Getter:
     @brief Gets the x location of the text
 
     This method has been introduced in version 0.23.
@@ -53822,14 +54140,21 @@
         """
     def with_text(self, text: str, inverse: bool) -> Texts:
         r"""
         @brief Filter the text by text string
         If "inverse" is false, this method returns the texts with the given string.
         If "inverse" is true, this method returns the texts not having the given string.
         """
+    def write(self, filename: str) -> None:
+        r"""
+        @brief Writes the region to a file
+        This method is provided for debugging purposes. It writes the object to a flat layer 0/0 in a single top cell.
+
+        This method has been introduced in version 0.29.
+        """
 
 class TileOutputReceiver(TileOutputReceiverBase):
     r"""
     @brief A receiver abstraction for the tiling processor.
 
     The tiling processor (\TilingProcessor) is a framework for executing sequences of operations on tiles of a layout or multiple layouts. The \TileOutputReceiver class is used to specify an output channel for the tiling processor. See \TilingProcessor#output for more details.
 
@@ -55323,20 +55648,20 @@
     def __lt__(self, other: int) -> bool:
         r"""
         @brief Returns true if the enum is less (in the enum symbol order) than the integer value
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer for inequality
+        @brief Compares two enums for inequality
         """
     @overload
     def __ne__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums for inequality
+        @brief Compares an enum with an integer for inequality
         """
     def __repr__(self) -> str:
         r"""
         @brief Converts an enum to a visual string
         """
     def __str__(self) -> str:
         r"""
@@ -55606,20 +55931,20 @@
     def __deepcopy__(self) -> VAlign:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums
+        @brief Compares an enum with an integer value
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer value
+        @brief Compares two enums
         """
     def __hash__(self) -> int:
         r"""
         @brief Gets the hash value from the enum
         """
     @overload
     def __init__(self, i: int) -> None:
@@ -57073,20 +57398,20 @@
     def __deepcopy__(self) -> ZeroDistanceMode:
         r"""
         @brief Creates a copy of self
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares an enum with an integer value
+        @brief Compares two enums
         """
     @overload
     def __eq__(self, other: object) -> bool:
         r"""
-        @brief Compares two enums
+        @brief Compares an enum with an integer value
         """
     def __hash__(self) -> int:
         r"""
         @brief Gets the hash value from the enum
         """
     @overload
     def __init__(self, i: int) -> None:
```

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/laycore.pyi` & `klayout-0.29.1/src/pymod/distutils_src/klayout/laycore.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2508,14 +2508,274 @@
         @brief Writes configuration to a file
         @return A value indicating whether the operation was successful
 
         If the configuration file cannot be written, false 
         is returned but no exception is thrown.
         """
 
+class EditorHooks:
+    r"""
+    @brief An implementation base class for editor hooks
+
+    Editor hooks allow implementing technology-specific callbacks into the editor for example to implement visual feedback about DRC rules.
+
+    This class provides the basic interface. To implement callbacks, use the \EditorHooks class. You should not need to instantiate this class.
+
+    The following is an excample for editor hooks that add DRC space indicators for polygon-alike shapes,
+    It implements the shape creation protocol to capture new shapes and the modification protocol to capture shape manipulations. It displays a halo following hard-coded DRC rules to indicate the forbidden zones around the shapes:
+
+    @code
+    class MyEditorHooks < RBA::EditorHooks
+
+      def initialize()
+  
+        register("editor_hooks_demo")
+
+        cleanup    
+
+        # some demo values    
+        @spaces = {
+          RBA::LayerInfo::new(1, 0) => [ 0.2, RBA::Region::Euclidian ],
+          RBA::LayerInfo::new(2, 0) => [ 0.5, RBA::Region::Projection ]
+        }
+    
+      end
+
+      # Utilities
+  
+      # pick the space value from layer or set to nil
+      def set_space_from_layer(layer_index)
+        lp = @layout.get_info(layer_index)
+        if @spaces[lp]
+          (s, m) = @spaces[lp]
+          @space = s / @layout.dbu
+          @metrics = m
+        else
+          @space = nil
+        end
+      end
+      
+      def add_marker_from_shape(shape, trans)
+  
+        if !@space
+          return   # no space value set
+        end
+    
+        p = shape.polygon
+        if !p
+          return   # not a polygon-like object
+        end
+    
+        r = RBA::Region::new
+        # maintain 2-point polygons for the first edge drawn
+        r.merged_semantics = (p.num_points != 2)
+        r.insert(p)
+    
+        # compute DRC hull and prepare markers
+        r.drc_hull(@metrics, @space).each do |pp|
+          m = RBA::Marker::new(@view)
+          m.line_style = 2
+          m.vertex_size = 0
+          m.set_polygon(trans * pp)
+          @markers.append(m)
+        end
+    
+      end
+  
+      # setup session
+      def start(cv)
+        cleanup
+        @view = cv.view
+        @layout = cv.layout
+      end
+  
+      # end session
+      def cleanup
+        @space = nil
+        @view = nil
+        @layout = nil
+        clear_markers
+      end
+  
+      def clear_markers
+        @markers && @markers.each do |m|
+          # this is how a marker gets removed in Ruby:
+          m._destroy
+        end
+        @markers = []
+      end
+        
+      # Shape creation protocol
+  
+      def begin_create_shapes(cv, layer)
+        start(cv)
+        set_space_from_layer(layer.layer_index)
+      end
+
+      def begin_new_shapes
+        clear_markers
+      end
+
+      def create_shape(shape, trans)
+        add_marker_from_shape(shape, trans)
+      end
+      
+      def end_create_shapes
+        cleanup
+      end
+    
+      # Modification protocol
+  
+      def begin_edit(cv)
+        start(cv)
+      end
+
+      def begin_edits
+        # create new markers
+        clear_markers
+      end
+
+      # transformation of a shape or instance
+      def transformed(path, applied, trans)
+        if path.shape
+          set_space_from_layer(path.layer)
+          add_marker_from_shape(path.shape, trans * applied)
+        end
+      end
+
+      # modification of a shape
+      def modified(path, shape, trans)
+        set_space_from_layer(path.layer)
+        add_marker_from_shape(shape, trans)
+      end
+
+      def end_edit
+        cleanup
+      end
+  
+    end
+
+    # instantiation of the hooks object
+    MyEditorHooks::new
+    @/code
+
+    The EditorHooks class has been introduced in version 0.29.1.
+    """
+    @property
+    def technology(self) -> None:
+        r"""
+        WARNING: This variable can only be set, not retrieved.
+        @brief sets the name of the technology the hooks are associated with
+        This will clear all technology associations and associate the hooks with that technology only.
+        """
+    @classmethod
+    def new(cls) -> EditorHooks:
+        r"""
+        @brief Creates a new object of this class
+        """
+    def __init__(self) -> None:
+        r"""
+        @brief Creates a new object of this class
+        """
+    def _create(self) -> None:
+        r"""
+        @brief Ensures the C++ object is created
+        Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
+        """
+    def _destroy(self) -> None:
+        r"""
+        @brief Explicitly destroys the object
+        Explicitly destroys the object on C++ side if it was owned by the script interpreter. Subsequent access to this object will throw an exception.
+        If the object is not owned by the script, this method will do nothing.
+        """
+    def _destroyed(self) -> bool:
+        r"""
+        @brief Returns a value indicating whether the object was already destroyed
+        This method returns true, if the object was destroyed, either explicitly or by the C++ side.
+        The latter may happen, if the object is owned by a C++ object which got destroyed itself.
+        """
+    def _is_const_object(self) -> bool:
+        r"""
+        @brief Returns a value indicating whether the reference is a const reference
+        This method returns true, if self is a const reference.
+        In that case, only const methods may be called on self.
+        """
+    def _manage(self) -> None:
+        r"""
+        @brief Marks the object as managed by the script side.
+        After calling this method on an object, the script side will be responsible for the management of the object. This method may be called if an object is returned from a C++ function and the object is known not to be owned by any C++ instance. If necessary, the script side may delete the object if the script's reference is no longer required.
+
+        Usually it's not required to call this method. It has been introduced in version 0.24.
+        """
+    def _unmanage(self) -> None:
+        r"""
+        @brief Marks the object as no longer owned by the script side.
+        Calling this method will make this object no longer owned by the script's memory management. Instead, the object must be managed in some other way. Usually this method may be called if it is known that some C++ object holds and manages this object. Technically speaking, this method will turn the script's reference into a weak reference. After the script engine decides to delete the reference, the object itself will still exist. If the object is not managed otherwise, memory leaks will occur.
+
+        Usually it's not required to call this method. It has been introduced in version 0.24.
+        """
+    def add_technology(self, tech: str) -> None:
+        r"""
+        @brief Additionally associates the hooks with the given technology.
+        See also \clear_technologies.
+        """
+    def clear_technologies(self) -> None:
+        r"""
+        @brief Clears the list of technologies the hooks are associated with.
+        See also \add_technology.
+        """
+    def create(self) -> None:
+        r"""
+        @brief Ensures the C++ object is created
+        Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
+        """
+    def destroy(self) -> None:
+        r"""
+        @brief Explicitly destroys the object
+        Explicitly destroys the object on C++ side if it was owned by the script interpreter. Subsequent access to this object will throw an exception.
+        If the object is not owned by the script, this method will do nothing.
+        """
+    def destroyed(self) -> bool:
+        r"""
+        @brief Returns a value indicating whether the object was already destroyed
+        This method returns true, if the object was destroyed, either explicitly or by the C++ side.
+        The latter may happen, if the object is owned by a C++ object which got destroyed itself.
+        """
+    def for_technologies(self) -> bool:
+        r"""
+        @brief Returns a value indicating whether the hooks are associated with any technology.
+        """
+    def is_const_object(self) -> bool:
+        r"""
+        @brief Returns a value indicating whether the reference is a const reference
+        This method returns true, if self is a const reference.
+        In that case, only const methods may be called on self.
+        """
+    def is_for_technology(self, tech: str) -> bool:
+        r"""
+        @brief Returns a value indicating whether the hooks are associated with the given technology.
+        The method is equivalent to checking whether the \technologies list is empty.
+        """
+    def name(self) -> str:
+        r"""
+        @brief Gets the name of the hooks object.
+        This is the name, the object was registered under in the system.
+        """
+    def register(self, name: str) -> None:
+        r"""
+        @brief Registers the hooks in the system.
+        The hooks will not be active before they are registered in the system. Registration will also transfer object ownership to the system.
+
+        The name is arbitary, but should be unique. Upon registration, this hooks object will replace others with the same name already registered in the system. This will simplify debugging as you can re-run the same code, without accumulating hooks.
+        """
+    def technologies(self) -> List[str]:
+        r"""
+        @brief Gets the list of technologies these hooks are associated with.
+        """
+
 class Image(BasicImage):
     r"""
     @brief An image to be stored as a layout annotation
 
     Images can be put onto the layout canvas as annotations, along with rulers and markers.
     Images can be monochrome (represent scalar data) as well as color (represent color images).
     The display of images can be adjusted in various ways, i.e. color mapping (translation of scalar values to
@@ -9153,14 +9413,22 @@
         Initially this property is set to true. This means that the plugin will have a visible entry in the toolbar. This property can be set to false to disable this feature. In that case, the title and icon given on registration will be ignored. 
         """
     @classmethod
     def new(cls) -> PluginFactory:
         r"""
         @brief Creates a new object of this class
         """
+    def __copy__(self) -> PluginFactory:
+        r"""
+        @brief Creates a copy of self
+        """
+    def __deepcopy__(self) -> PluginFactory:
+        r"""
+        @brief Creates a copy of self
+        """
     def __init__(self) -> None:
         r"""
         @brief Creates a new object of this class
         """
     def _create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
@@ -9252,14 +9520,18 @@
         """
     def add_submenu(self, menu_name: str, insert_pos: str, title: str) -> None:
         r"""
         @brief Specifies a menu item or sub-menu
 
         This method has been introduced in version 0.27.
         """
+    def assign(self, other: PluginFactory) -> None:
+        r"""
+        @brief Assigns another object to self
+        """
     def create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
     def destroy(self) -> None:
         r"""
@@ -9269,14 +9541,18 @@
         """
     def destroyed(self) -> bool:
         r"""
         @brief Returns a value indicating whether the object was already destroyed
         This method returns true, if the object was destroyed, either explicitly or by the C++ side.
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
+    def dup(self) -> PluginFactory:
+        r"""
+        @brief Creates a copy of self
+        """
     def is_const_object(self) -> bool:
         r"""
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
     @overload
```

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/rdbcore.pyi` & `klayout-0.29.1/src/pymod/distutils_src/klayout/rdbcore.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -82,23 +82,39 @@
         """
     def destroyed(self) -> bool:
         r"""
         @brief Returns a value indicating whether the object was already destroyed
         This method returns true, if the object was destroyed, either explicitly or by the C++ side.
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
+    @overload
     def each_item(self) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database which are associated with this category
 
         This method has been introduced in version 0.23.
         """
+    @overload
+    def each_item(self) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database which are associated with this category (non-const version)
+
+        This method has been introduced in version 0.29.
+        """
+    @overload
     def each_sub_category(self) -> Iterator[RdbCategory]:
         r"""
         @brief Iterates over all sub-categories
+
+        The const version has been added in version 0.29.
+        """
+    @overload
+    def each_sub_category(self) -> Iterator[RdbCategory]:
+        r"""
+        @brief Iterates over all sub-categories (non-const version)
         """
     def is_const_object(self) -> bool:
         r"""
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
@@ -114,18 +130,27 @@
         The number of items includes the items in sub-categories of this category.
         """
     def num_items_visited(self) -> int:
         r"""
         @brief Gets the number of visited items in this category
         The number of items includes the items in sub-categories of this category.
         """
+    @overload
     def parent(self) -> RdbCategory:
         r"""
         @brief Gets the parent category of this category
         @return The parent category or nil if this category is a top-level category
+
+        The const version has been added in version 0.29.
+        """
+    @overload
+    def parent(self) -> RdbCategory:
+        r"""
+        @brief Gets the parent category of this category (non-const version)
+        @return The parent category or nil if this category is a top-level category
         """
     def path(self) -> str:
         r"""
         @brief Gets the category path
         The category path is the category name for top level categories. For child categories, the path contains the names of all parent categories separated by a dot.
         @return The path for this category
         """
@@ -258,84 +283,132 @@
         @brief Removes all references from this cell
         """
     def create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
+    @overload
     def database(self) -> ReportDatabase:
         r"""
         @brief Gets the database object that category is associated with
 
         This method has been introduced in version 0.23.
         """
+    @overload
+    def database(self) -> ReportDatabase:
+        r"""
+        @brief Gets the database object that category is associated with (non-const version)
+
+        This method has been introduced in version 0.29.
+        """
     def destroy(self) -> None:
         r"""
         @brief Explicitly destroys the object
         Explicitly destroys the object on C++ side if it was owned by the script interpreter. Subsequent access to this object will throw an exception.
         If the object is not owned by the script, this method will do nothing.
         """
     def destroyed(self) -> bool:
         r"""
         @brief Returns a value indicating whether the object was already destroyed
         This method returns true, if the object was destroyed, either explicitly or by the C++ side.
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
+    @overload
     def each_item(self) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database which are associated with this cell
 
         This method has been introduced in version 0.23.
         """
+    @overload
+    def each_item(self) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database which are associated with this cell (non-const version)
+
+        This method has been introduced in version 0.29.
+        """
+    @overload
     def each_reference(self) -> Iterator[RdbReference]:
         r"""
         @brief Iterates over all references
         """
+    @overload
+    def each_reference(self) -> Iterator[RdbReference]:
+        r"""
+        @brief Iterates over all references (non-const version)
+
+        This method has been introduced in version 0.23.
+        """
     def is_const_object(self) -> bool:
         r"""
         @brief Returns a value indicating whether the reference is a const reference
         This method returns true, if self is a const reference.
         In that case, only const methods may be called on self.
         """
+    def layout_name(self) -> str:
+        r"""
+        @brief Gets the name of the layout cell
+        For variants, this string is the name of the actual layout cell. If empty, the cell is assume to be called 'name'.
+        @return The layout cell name
+        This read-only attribute has been added in version 0.29.1.
+        """
     def name(self) -> str:
         r"""
         @brief Gets the cell name
-        The cell name is an string that identifies the category in the database. Additionally, a cell may carry a variant identifier which is a string that uniquely identifies a cell in the context of its variants. The "qualified name" contains both the cell name and the variant name. Cell names are also used to identify report database cell's with layout cells. @return The cell name
+        The cell name is an string that identifies the category in the database. Additionally, a cell may carry a variant identifier which is a string that uniquely identifies a cell in the context of its variants. The "qualified name" contains both the cell name and the variant name. Cell names are also used to identify report database cells with layout cells. For variants, the layout cell name can be specified explicitly with the \layout_name attribute (see \RdbDatabase#create_cell). The latter is available since version 0.29.1.
+        @return The cell name
         """
     def num_items(self) -> int:
         r"""
         @brief Gets the number of items for this cell
         """
     def num_items_visited(self) -> int:
         r"""
         @brief Gets the number of visited items for this cell
         """
     def qname(self) -> str:
         r"""
-        @brief Gets the cell's qualified name
+        @brief Gets the qualified name of the cell
         The qualified name is a combination of the cell name and optionally the variant name. It is used to identify the cell by name in a unique way.
         @return The qualified name
         """
     def rdb_id(self) -> int:
         r"""
         @brief Gets the cell ID
         The cell ID is an integer that uniquely identifies the cell. It is used for referring to a cell in \RdbItem for example.
         @return The cell ID
         """
     def variant(self) -> str:
         r"""
         @brief Gets the cell variant name
-        A variant name additionally identifies the cell when multiple cells with the same name are present. A variant name is either assigned automatically or set when creating a cell. @return The cell variant name
+        A variant name additionally identifies the cell when multiple cells with the same name are present. A variant name is either assigned automatically or set when creating a cell.
+        @return The cell variant name
         """
 
 class RdbItem:
     r"""
     @brief An item inside the report database
     An item is the basic information entity in the RDB. It is associated with a cell and a category. It can be assigned values which encapsulate other objects such as strings and geometrical objects. In addition, items can be assigned an image (i.e. a screenshot image) and tags which are basically boolean flags that can be defined freely.
     """
+    comment: str
+    r"""
+    Getter:
+    @brief Gets the common associated with this item as a string
+    @return The comment string
+    The comment string is an arbitrary string added by the user to the item.
+
+    This attribute has been added in version 0.29.1.
+
+    Setter:
+    @brief Sets the common associated with this item as a string
+    See \comment for a description of that attribute.
+
+    This attribute has been added in version 0.29.1.
+    """
     @property
     def image(self) -> None:
         r"""
         WARNING: This variable can only be set, not retrieved.
         @brief Sets the attached image from a PixelBuffer object
 
         This method has been added in version 0.28.
@@ -559,14 +632,19 @@
         @return True, if the item has been visited already
         """
     def remove_tag(self, tag_id: int) -> None:
         r"""
         @brief Remove the tag with the given id from the item
         If a tag with that ID does not exists on this item, this method does nothing.
         """
+    def remove_tags(self) -> None:
+        r"""
+        @brief Removes all tags from the item
+        This method has been introduced in version 0.29.1.
+        """
 
 class RdbItemValue:
     r"""
     @brief A value object inside the report database
     Value objects are attached to items to provide markers. An arbitrary number of such value objects can be attached to an item.
     Currently, a value can represent a box, a polygon or an edge. Geometrical objects are represented in micron units and are therefore "D" type objects (DPolygon, DEdge and DBox). 
     """
@@ -951,14 +1029,22 @@
         @brief Assigns another object to self
         """
     def create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
+    @overload
+    def database(self) -> ReportDatabase:
+        r"""
+        @brief Gets the database object that category is associated with (non-const version)
+
+        This method has been introduced in version 0.29.
+        """
+    @overload
     def database(self) -> ReportDatabase:
         r"""
         @brief Gets the database object that category is associated with
 
         This method has been introduced in version 0.23.
         """
     def destroy(self) -> None:
@@ -1037,14 +1123,22 @@
     @classmethod
     def new(cls, name: str) -> ReportDatabase:
         r"""
         @brief Creates a report database
         @param name The name of the database
         The name of the database will be used in the user interface to refer to a certain database.
         """
+    def __copy__(self) -> ReportDatabase:
+        r"""
+        @brief Creates a copy of self
+        """
+    def __deepcopy__(self) -> ReportDatabase:
+        r"""
+        @brief Creates a copy of self
+        """
     def __init__(self, name: str) -> None:
         r"""
         @brief Creates a report database
         @param name The name of the database
         The name of the database will be used in the user interface to refer to a certain database.
         """
     def _create(self) -> None:
@@ -1080,37 +1174,106 @@
     def _unmanage(self) -> None:
         r"""
         @brief Marks the object as no longer owned by the script side.
         Calling this method will make this object no longer owned by the script's memory management. Instead, the object must be managed in some other way. Usually this method may be called if it is known that some C++ object holds and manages this object. Technically speaking, this method will turn the script's reference into a weak reference. After the script engine decides to delete the reference, the object itself will still exist. If the object is not managed otherwise, memory leaks will occur.
 
         Usually it's not required to call this method. It has been introduced in version 0.24.
         """
+    def apply(self, other: ReportDatabase) -> None:
+        r"""
+        @brief Transfers item attributes from one database to another for identical items
+        This method will identify items that are identical between the two databases and transfer item attributes from the 'other' database to this database. Transferable attributes are:
+
+        @ul
+        @li Images @/li
+        @li Item tags @/li
+        @/ul
+
+        Existing attributes in this database are overwritten.
+
+        Items are identical if
+
+        @ul
+        @li They belong to the same cell (by qname) @/li
+        @li They belong to the same category (by name) @/li
+        @li Their values are identical @/li
+        @/ul
+
+        Values are identical if their individual values and (optional) value tags are identical. Values tagged with a tag unknown to the other database are ignored. The order of values matters during the compare. So the value pair (17.0, 'abc') is different from ('abc', 17.0).
+
+        The intended application for this method is use for error waiving: as the waived attribute is a transferable attribute, it is possible to apply the waived flag from from a waiver database (the 'other' database) using this method.
+
+        This method has been added in version 0.29.1.
+        """
+    def assign(self, other: ReportDatabase) -> None:
+        r"""
+        @brief Assigns another object to self
+        """
+    @overload
     def category_by_id(self, id: int) -> RdbCategory:
         r"""
         @brief Gets a category by ID
         @return The (const) category object or nil if the ID is not valid
         """
+    @overload
+    def category_by_id(self, id: int) -> RdbCategory:
+        r"""
+        @brief Gets a category by ID (non-const version)
+        @return The (const) category object or nil if the ID is not valid
+
+        This non-const variant has been introduced in version 0.29.
+        """
+    @overload
     def category_by_path(self, path: str) -> RdbCategory:
         r"""
         @brief Gets a category by path
         @param path The full path to the category starting from the top level (subcategories separated by dots)
         @return The (const) category object or nil if the name is not valid
         """
+    @overload
+    def category_by_path(self, path: str) -> RdbCategory:
+        r"""
+        @brief Gets a category by path (non-const version)
+        @param path The full path to the category starting from the top level (subcategories separated by dots)
+        @return The (const) category object or nil if the name is not valid
+
+        This non-const variant has been introduced in version 0.29.
+        """
+    @overload
     def cell_by_id(self, id: int) -> RdbCell:
         r"""
         @brief Returns the cell for a given ID
         @param id The ID of the cell
         @return The cell object or nil if no cell with that ID exists
         """
+    @overload
+    def cell_by_id(self, id: int) -> RdbCell:
+        r"""
+        @brief Returns the cell for a given ID (non-const version)
+        @param id The ID of the cell
+        @return The cell object or nil if no cell with that ID exists
+
+        This non-const variant has been added version 0.29.
+        """
+    @overload
     def cell_by_qname(self, qname: str) -> RdbCell:
         r"""
         @brief Returns the cell for a given qualified name
         @param qname The qualified name of the cell (name plus variant name optionally)
         @return The cell object or nil if no such cell exists
         """
+    @overload
+    def cell_by_qname(self, qname: str) -> RdbCell:
+        r"""
+        @brief Returns the cell for a given qualified name (non-const version)
+        @param qname The qualified name of the cell (name plus variant name optionally)
+        @return The cell object or nil if no such cell exists
+
+        This non-const variant has been added version 0.29.
+        """
     def create(self) -> None:
         r"""
         @brief Ensures the C++ object is created
         Use this method to ensure the C++ object is created, for example to ensure that resources are allocated. Usually C++ objects are created on demand and not necessarily when the script object is created.
         """
     @overload
     def create_category(self, name: str) -> RdbCategory:
@@ -1120,27 +1283,30 @@
         """
     @overload
     def create_category(self, parent: RdbCategory, name: str) -> RdbCategory:
         r"""
         @brief Creates a new sub-category
         @param parent The category under which the category should be created
         @param name The name of the category
+        Since version 0.29.1, 'parent' can be nil. In that case, a top-level category is created.
         """
     @overload
     def create_cell(self, name: str) -> RdbCell:
         r"""
         @brief Creates a new cell
         @param name The name of the cell
         """
     @overload
-    def create_cell(self, name: str, variant: str) -> RdbCell:
+    def create_cell(self, name: str, variant: str, layout_name: Optional[str] = ...) -> RdbCell:
         r"""
         @brief Creates a new cell, potentially as a variant for a cell with the same name
         @param name The name of the cell
         @param variant The variant name of the cell
+        @param layout_name For variants, this is the name of the layout cell. If empty, 'name' is used for the layout cell name.
+        The 'layout_name' argument has been added in version 0.29.1.
         """
     @overload
     def create_item(self, cell: RdbCell, category: RdbCategory) -> RdbItem:
         r"""
         @brief Creates a new item for the given cell/category combination
         @param cell The cell to which the item is associated
         @param category The category to which the item is associated
@@ -1298,41 +1464,97 @@
         """
     def destroyed(self) -> bool:
         r"""
         @brief Returns a value indicating whether the object was already destroyed
         This method returns true, if the object was destroyed, either explicitly or by the C++ side.
         The latter may happen, if the object is owned by a C++ object which got destroyed itself.
         """
+    def dup(self) -> ReportDatabase:
+        r"""
+        @brief Creates a copy of self
+        """
+    @overload
     def each_category(self) -> Iterator[RdbCategory]:
         r"""
         @brief Iterates over all top-level categories
         """
+    @overload
+    def each_category(self) -> Iterator[RdbCategory]:
+        r"""
+        @brief Iterates over all top-level categories (non-const version)
+
+        The non-const variant has been added in version 0.29.
+        """
+    @overload
     def each_cell(self) -> Iterator[RdbCell]:
         r"""
         @brief Iterates over all cells
         """
+    @overload
+    def each_cell(self) -> Iterator[RdbCell]:
+        r"""
+        @brief Iterates over all cells (non-const version)
+
+        This non-const variant has been added version 0.29.
+        """
+    @overload
     def each_item(self) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database
         """
+    @overload
+    def each_item(self) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database (non-const version)
+
+        This non-const variant has been added in version 0.29.
+        """
+    @overload
     def each_item_per_category(self, category_id: int) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database which are associated with the given category
         @param category_id The ID of the category for which all associated items should be retrieved
         """
+    @overload
+    def each_item_per_category(self, category_id: int) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database which are associated with the given category (non-const version)
+        @param category_id The ID of the category for which all associated items should be retrieved
+
+        This non-const variant has been added in version 0.29.
+        """
+    @overload
     def each_item_per_cell(self, cell_id: int) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database which are associated with the given cell
         @param cell_id The ID of the cell for which all associated items should be retrieved
         """
+    @overload
+    def each_item_per_cell(self, cell_id: int) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database which are associated with the given cell (non-const version)
+        @param cell_id The ID of the cell for which all associated items should be retrieved
+
+        This non-const variant has been added in version 0.29.
+        """
+    @overload
+    def each_item_per_cell_and_category(self, cell_id: int, category_id: int) -> Iterator[RdbItem]:
+        r"""
+        @brief Iterates over all items inside the database which are associated with the given cell and category
+        @param cell_id The ID of the cell for which all associated items should be retrieved
+        @param category_id The ID of the category for which all associated items should be retrieved
+        """
+    @overload
     def each_item_per_cell_and_category(self, cell_id: int, category_id: int) -> Iterator[RdbItem]:
         r"""
         @brief Iterates over all items inside the database which are associated with the given cell and category
         @param cell_id The ID of the cell for which all associated items should be retrieved
         @param category_id The ID of the category for which all associated items should be retrieved
+
+        This non-const variant has been added in version 0.29.
         """
     def filename(self) -> str:
         r"""
         @brief Gets the file name and path where the report database is stored
         This property is set when a database is saved or loaded. It cannot be set manually.
         @return The file name and path
         """
```

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout/tlcore.pyi` & `klayout-0.29.1/src/pymod/distutils_src/klayout/tlcore.pyi`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/PKG-INFO` & `klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klayout
-Version: 0.29.0
+Version: 0.29.1
 Summary: KLayout standalone Python package
 Home-page: https://github.com/klayout/klayout
 Author: Matthias Koefferlein
 Author-email: matthias@klayout.de
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klayout-0.29.0/src/pymod/distutils_src/klayout.egg-info/SOURCES.txt` & `klayout-0.29.1/src/pymod/distutils_src/klayout.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -432,22 +432,26 @@
 src/edt/edt/edtCommon.h
 src/edt/edt/edtConfig.cc
 src/edt/edt/edtConfig.h
 src/edt/edt/edtDialogs.cc
 src/edt/edt/edtDialogs.h
 src/edt/edt/edtDistribute.cc
 src/edt/edt/edtDistribute.h
+src/edt/edt/edtEditorHooks.cc
+src/edt/edt/edtEditorHooks.h
 src/edt/edt/edtEditorOptionsPages.cc
 src/edt/edt/edtEditorOptionsPages.h
 src/edt/edt/edtForceLink.cc
 src/edt/edt/edtForceLink.h
 src/edt/edt/edtInstPropertiesPage.cc
 src/edt/edt/edtInstPropertiesPage.h
 src/edt/edt/edtMainService.cc
 src/edt/edt/edtMainService.h
+src/edt/edt/edtMoveTrackerService.cc
+src/edt/edt/edtMoveTrackerService.h
 src/edt/edt/edtPCellParametersPage.cc
 src/edt/edt/edtPCellParametersPage.h
 src/edt/edt/edtPartialService.cc
 src/edt/edt/edtPartialService.h
 src/edt/edt/edtPlugin.cc
 src/edt/edt/edtPlugin.h
 src/edt/edt/edtPropertiesPageUtils.cc
@@ -459,14 +463,15 @@
 src/edt/edt/edtService.cc
 src/edt/edt/edtService.h
 src/edt/edt/edtServiceImpl.cc
 src/edt/edt/edtServiceImpl.h
 src/edt/edt/edtUtils.cc
 src/edt/edt/edtUtils.h
 src/edt/edt/gsiDeclEdt.cc
+src/edt/edt/gsiDeclEdtEditorHooks.cc
 src/gsi/gsi/gsi.cc
 src/gsi/gsi/gsi.h
 src/gsi/gsi/gsiCallback.h
 src/gsi/gsi/gsiCallbackVar.h
 src/gsi/gsi/gsiClass.cc
 src/gsi/gsi/gsiClass.h
 src/gsi/gsi/gsiClassBase.cc
```

### Comparing `klayout-0.29.0/src/pymod/distutils_src/pya/__init__.py` & `klayout-0.29.1/src/pymod/distutils_src/pya/__init__.py`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/edt/edtMain.cc` & `klayout-0.29.1/src/pymod/edt/edtMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/edt/edtMain.h` & `klayout-0.29.1/src/pymod/edt/edtMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/img/imgMain.cc` & `klayout-0.29.1/src/pymod/img/imgMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/img/imgMain.h` & `klayout-0.29.1/src/pymod/img/imgMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lay/layMain.cc` & `klayout-0.29.1/src/pymod/lay/layMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lay/layMain.h` & `klayout-0.29.1/src/pymod/lay/layMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lib/libMain.cc` & `klayout-0.29.1/src/pymod/lib/libMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lib/libMain.h` & `klayout-0.29.1/src/pymod/lib/libMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lym/lymMain.cc` & `klayout-0.29.1/src/pymod/lym/lymMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/lym/lymMain.h` & `klayout-0.29.1/src/pymod/lym/lymMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/pya/pyaMain.cc` & `klayout-0.29.1/src/pymod/pya/pyaMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/pymodHelper.h` & `klayout-0.29.1/src/pymod/pymodHelper.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/rdb/rdbMain.cc` & `klayout-0.29.1/src/pymod/rdb/rdbMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/rdb/rdbMain.h` & `klayout-0.29.1/src/pymod/rdb/rdbMain.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/tl/tlMain.cc` & `klayout-0.29.1/src/pymod/tl/tlMain.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/pymod/unit_tests/pymod_tests.cc` & `klayout-0.29.1/src/pymod/unit_tests/pymod_tests.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rbastub/rba.cc` & `klayout-0.29.1/src/rbastub/rba.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rbastub/rba.h` & `klayout-0.29.1/src/rbastub/rba.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rbastub/rbaCommon.h` & `klayout-0.29.1/src/rbastub/rbaCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/gsiDeclRdb.cc` & `klayout-0.29.1/src/rdb/rdb/gsiDeclRdb.cc`

 * *Files 2% similar despite different names*

```diff
@@ -261,25 +261,33 @@
     "This method has been introduced in version 0.29."
   ) +
   gsi::method ("name", &rdb::Cell::name,
     "@brief Gets the cell name\n"
     "The cell name is an string that identifies the category in the database. "
     "Additionally, a cell may carry a variant identifier which is a string that uniquely identifies a cell "
     "in the context of its variants. The \"qualified name\" contains both the cell name and the variant name. "
-    "Cell names are also used to identify report database cell's with layout cells. "
+    "Cell names are also used to identify report database cells with layout cells. For variants, the layout cell name "
+    "can be specified explicitly with the \\layout_name attribute (see \\RdbDatabase#create_cell). The latter is available "
+    "since version 0.29.1.\n"
     "@return The cell name\n"
   ) +
   gsi::method ("variant", &rdb::Cell::variant, 
     "@brief Gets the cell variant name\n"
     "A variant name additionally identifies the cell when multiple cells with the same name are present. "
-    "A variant name is either assigned automatically or set when creating a cell. "
+    "A variant name is either assigned automatically or set when creating a cell.\n"
     "@return The cell variant name\n"
   ) +
-  gsi::method ("qname", &rdb::Cell::qname, 
-    "@brief Gets the cell's qualified name\n"
+  gsi::method ("layout_name", &rdb::Cell::layout_name,
+    "@brief Gets the name of the layout cell\n"
+    "For variants, this string is the name of the actual layout cell. If empty, the cell is assume to be called 'name'.\n"
+    "@return The layout cell name\n"
+    "This read-only attribute has been added in version 0.29.1.\n"
+  ) +
+  gsi::method ("qname", &rdb::Cell::qname,
+    "@brief Gets the qualified name of the cell\n"
     "The qualified name is a combination of the cell name and optionally the variant name. "
     "It is used to identify the cell by name in a unique way.\n"
     "@return The qualified name\n"
   ) +
   gsi::method ("num_items", &rdb::Cell::num_items, 
     "@brief Gets the number of items for this cell\n"
   ) +
@@ -907,14 +915,18 @@
     "Each tag can be added once to the item. The tags of an item thus form a set. "
     "If a tag with that ID already exists, this method does nothing."
   ) +
   gsi::method ("remove_tag", &rdb::Item::remove_tag, gsi::arg ("tag_id"),
     "@brief Remove the tag with the given id from the item\n"
     "If a tag with that ID does not exists on this item, this method does nothing."
   ) +
+  gsi::method ("remove_tags", &rdb::Item::remove_tags,
+    "@brief Removes all tags from the item\n"
+    "This method has been introduced in version 0.29.1."
+  ) +
   gsi::method ("has_tag?", &rdb::Item::has_tag, gsi::arg ("tag_id"),
     "@brief Returns a value indicating whether the item has a tag with the given ID\n"
     "@return True, if the item has a tag with the given ID\n"
   ) +
   gsi::method ("tags_str", &rdb::Item::tag_str, 
     "@brief Returns a string listing all tags of this item\n"
     "@return A comma-separated list of tags\n"
@@ -924,14 +936,27 @@
     "@param tags A comma-separated list of tags\n"
   ) +
   gsi::method ("has_image?", &rdb::Item::has_image,
     "@brief Gets a value indicating that the item has an image attached\n"
     "See \\image_str how to obtain the image.\n\n"
     "This method has been introduced in version 0.28.\n"
   ) +
+  gsi::method ("comment", &rdb::Item::comment,
+    "@brief Gets the common associated with this item as a string\n"
+    "@return The comment string\n"
+    "The comment string is an arbitrary string added by the user to the item.\n"
+    "\n"
+    "This attribute has been added in version 0.29.1.\n"
+  ) +
+  gsi::method ("comment=", &rdb::Item::set_comment, gsi::arg ("comment"),
+    "@brief Sets the common associated with this item as a string\n"
+    "See \\comment for a description of that attribute.\n"
+    "\n"
+    "This attribute has been added in version 0.29.1.\n"
+  ) +
   gsi::method ("image_str", &rdb::Item::image_str,
     "@brief Gets the image associated with this item as a string\n"
     "@return A base64-encoded image file (in PNG format)\n"
   ) +
   gsi::method ("image_str=", &rdb::Item::set_image_str, gsi::arg ("image"),
     "@brief Sets the image from a string\n"
     "@param image A base64-encoded image file (preferably in PNG format)\n"
@@ -1313,14 +1338,15 @@
     "@brief Creates a new top level category\n"
     "@param name The name of the category\n"
   ) +
   gsi::method ("create_category", (rdb::Category *(rdb::Database::*) (rdb::Category *, const std::string &)) &rdb::Database::create_category, gsi::arg ("parent"), gsi::arg ("name"),
     "@brief Creates a new sub-category\n"
     "@param parent The category under which the category should be created\n"
     "@param name The name of the category\n"
+    "Since version 0.29.1, 'parent' can be nil. In that case, a top-level category is created."
   ) +
   gsi::method ("category_by_path", &rdb::Database::category_by_name, gsi::arg ("path"),
     "@brief Gets a category by path\n"
     "@param path The full path to the category starting from the top level (subcategories separated by dots)\n"
     "@return The (const) category object or nil if the name is not valid\n"
   ) +
   gsi::method ("category_by_path", &rdb::Database::category_by_name_non_const, gsi::arg ("path"),
@@ -1340,18 +1366,20 @@
     "\n"
     "This non-const variant has been introduced in version 0.29."
   ) +
   gsi::method ("create_cell", (rdb::Cell *(rdb::Database::*) (const std::string &)) &rdb::Database::create_cell, gsi::arg ("name"),
     "@brief Creates a new cell\n"
     "@param name The name of the cell\n"
   ) +
-  gsi::method ("create_cell", (rdb::Cell *(rdb::Database::*) (const std::string &, const std::string &)) &rdb::Database::create_cell, gsi::arg ("name"), gsi::arg ("variant"),
+  gsi::method ("create_cell", (rdb::Cell *(rdb::Database::*) (const std::string &, const std::string &, const std::string &)) &rdb::Database::create_cell, gsi::arg ("name"), gsi::arg ("variant"), gsi::arg ("layout_name", std::string ()),
     "@brief Creates a new cell, potentially as a variant for a cell with the same name\n"
     "@param name The name of the cell\n"
     "@param variant The variant name of the cell\n"
+    "@param layout_name For variants, this is the name of the layout cell. If empty, 'name' is used for the layout cell name.\n"
+    "The 'layout_name' argument has been added in version 0.29.1.\n"
   ) +
   gsi::method ("variants", &rdb::Database::variants, gsi::arg ("name"),
     "@brief Gets the variants for a given cell name\n"
     "@param name The basic name of the cell\n"
     "@return An array of ID's representing cells that are variants for the given base name\n"
   ) +
   gsi::method ("cell_by_qname", &rdb::Database::cell_by_qname, gsi::arg ("qname"),
@@ -1558,14 +1586,44 @@
     "This method has been introduced in version 0.23.\n"
     "\n"
     "@param cell_id The ID of the cell to which the item is associated\n"
     "@param category_id The ID of the category to which the item is associated\n"
     "@param trans The transformation to apply\n"
     "@param edge_pairs The list of edge_pairs for which the items are created\n"
   ) +
+  gsi::method ("apply", &rdb::Database::apply, gsi::arg ("other"),
+    "@brief Transfers item attributes from one database to another for identical items\n"
+    "This method will identify items that are identical between the two databases and transfer "
+    "item attributes from the 'other' database to this database. Transferable attributes are:\n"
+    "\n"
+    "@ul\n"
+    "@li Images @/li\n"
+    "@li Item tags @/li\n"
+    "@/ul\n"
+    "\n"
+    "Existing attributes in this database are overwritten.\n"
+    "\n"
+    "Items are identical if\n"
+    "\n"
+    "@ul\n"
+    "@li They belong to the same cell (by qname) @/li\n"
+    "@li They belong to the same category (by name) @/li\n"
+    "@li Their values are identical @/li\n"
+    "@/ul\n"
+    "\n"
+    "Values are identical if their individual values and (optional) value tags are identical. "
+    "Values tagged with a tag unknown to the other database are ignored. "
+    "The order of values matters during the compare. So the value pair (17.0, 'abc') is different from ('abc', 17.0).\n"
+    "\n"
+    "The intended application for this method is use for error waiving: as the waived attribute is a transferable "
+    "attribute, it is possible to apply the waived flag from from a waiver database (the 'other' database) using this "
+    "method.\n"
+    "\n"
+    "This method has been added in version 0.29.1."
+  ) +
   gsi::method ("is_modified?", &rdb::Database::is_modified,
     "@brief Returns a value indicating whether the database has been modified\n"
   ) +
   gsi::method ("reset_modified", &rdb::Database::reset_modified,
     "@brief Reset the modified flag\n"
   ) +
   gsi::iterator_ext ("each_item", &database_items_begin, &database_items_end,
```

### Comparing `klayout-0.29.0/src/rdb/rdb/rdb.cc` & `klayout-0.29.1/src/rdb/rdb/rdb.cc`

 * *Files 11% similar despite different names*

```diff
@@ -56,24 +56,26 @@
 
 // ------------------------------------------------------------------------------------------
 //  Value implementation
 
 //  type index specializations
 
 template <> RDB_PUBLIC int type_index_of<double> ()        { return 0; }
-template <> RDB_PUBLIC int type_index_of<std::string> ()   { return 1; }
-template <> RDB_PUBLIC int type_index_of<db::DPolygon> ()  { return 2; }
-template <> RDB_PUBLIC int type_index_of<db::DEdge> ()     { return 3; }
-template <> RDB_PUBLIC int type_index_of<db::DEdgePair> () { return 4; }
-template <> RDB_PUBLIC int type_index_of<db::DBox> ()      { return 5; }
-template <> RDB_PUBLIC int type_index_of<db::DPath> ()     { return 6; }
-template <> RDB_PUBLIC int type_index_of<db::DText> ()     { return 7; }
+template <> RDB_PUBLIC int type_index_of<int> ()           { return 1; }
+template <> RDB_PUBLIC int type_index_of<std::string> ()   { return 2; }
+template <> RDB_PUBLIC int type_index_of<db::DPolygon> ()  { return 3; }
+template <> RDB_PUBLIC int type_index_of<db::DEdge> ()     { return 4; }
+template <> RDB_PUBLIC int type_index_of<db::DEdgePair> () { return 5; }
+template <> RDB_PUBLIC int type_index_of<db::DBox> ()      { return 6; }
+template <> RDB_PUBLIC int type_index_of<db::DPath> ()     { return 7; }
+template <> RDB_PUBLIC int type_index_of<db::DText> ()     { return 8; }
 
 //  Explicit instantiations to make VC++ happy in debug mode
 template class RDB_PUBLIC Value<double>;
+template class RDB_PUBLIC Value<int>;
 template class RDB_PUBLIC Value<std::string>;
 template class RDB_PUBLIC Value<db::DPolygon>;
 template class RDB_PUBLIC Value<db::DEdge>;
 template class RDB_PUBLIC Value<db::DEdgePair>;
 template class RDB_PUBLIC Value<db::DBox>;
 template class RDB_PUBLIC Value<db::DPath>;
 template class RDB_PUBLIC Value<db::DText>;
@@ -81,14 +83,19 @@
 //  to_string implementations
 
 template <> RDB_PUBLIC std::string Value<double>::to_string () const
 {
   return "float: " + tl::to_string (m_value);
 }
 
+template <> RDB_PUBLIC std::string Value<int>::to_string () const
+{
+  return "int: " + tl::to_string (m_value);
+}
+
 template <> RDB_PUBLIC std::string Value<std::string>::to_string () const
 {
   return "text: " + tl::to_word_or_quoted_string (m_value);
 }
 
 template <> RDB_PUBLIC std::string Value<db::DPolygon>::to_string () const
 {
@@ -123,14 +130,19 @@
 //  to_display_string implementations
 
 template <> RDB_PUBLIC std::string Value<double>::to_display_string () const
 {
   return tl::to_string (m_value);
 }
 
+template <> RDB_PUBLIC std::string Value<int>::to_display_string () const
+{
+  return tl::to_string (m_value);
+}
+
 template <> RDB_PUBLIC std::string Value<std::string>::to_display_string () const
 {
   return m_value;
 }
 
 template <> RDB_PUBLIC std::string Value<db::DPolygon>::to_display_string () const
 {
@@ -158,21 +170,82 @@
 }
 
 template <> RDB_PUBLIC std::string Value<db::DText>::to_display_string () const
 {
   return to_string ();
 }
 
+//  compare implementations
+
+template <> RDB_PUBLIC bool Value<double>::compare (const ValueBase *o) const
+{
+  const Value<double> *other = static_cast<const Value<double> *> (o);
+  return m_value < other->m_value - db::epsilon;
+}
+
+template <> RDB_PUBLIC bool Value<int>::compare (const ValueBase *o) const
+{
+  const Value<int> *other = static_cast<const Value<int> *> (o);
+  return m_value < other->m_value;
+}
+
+template <> RDB_PUBLIC bool Value<std::string>::compare (const ValueBase *o) const
+{
+  const Value<std::string> *other = static_cast<const Value<std::string> *> (o);
+  return m_value < other->m_value;
+}
+
+template <> RDB_PUBLIC bool Value<db::DPolygon>::compare (const ValueBase *o) const
+{
+  const Value<db::DPolygon> *other = static_cast<const Value<db::DPolygon> *> (o);
+  return m_value.less (other->m_value);
+}
+
+template <> RDB_PUBLIC bool Value<db::DEdge>::compare (const ValueBase *o) const
+{
+  const Value<db::DEdge> *other = static_cast<const Value<db::DEdge> *> (o);
+  return m_value.less (other->m_value);
+}
+
+template <> RDB_PUBLIC bool Value<db::DEdgePair>::compare (const ValueBase *o) const
+{
+  const Value<db::DEdgePair> *other = static_cast<const Value<db::DEdgePair> *> (o);
+  return m_value.less (other->m_value);
+}
+
+template <> RDB_PUBLIC bool Value<db::DBox>::compare (const ValueBase *o) const
+{
+  const Value<db::DBox> *other = static_cast<const Value<db::DBox> *> (o);
+  return m_value.less (other->m_value);
+}
+
+template <> RDB_PUBLIC bool Value<db::DPath>::compare (const ValueBase *o) const
+{
+  const Value<db::DPath> *other = static_cast<const Value<db::DPath> *> (o);
+  return m_value.less (other->m_value);
+}
+
+template <> RDB_PUBLIC bool Value<db::DText>::compare (const ValueBase *o) const
+{
+  const Value<db::DText> *other = static_cast<const Value<db::DText> *> (o);
+  return m_value.less (other->m_value);
+}
+
 //  is_shape implementations
 
 template <> RDB_PUBLIC bool Value<double>::is_shape () const
 {
   return false;
 }
 
+template <> RDB_PUBLIC bool Value<int>::is_shape () const
+{
+  return false;
+}
+
 template <> RDB_PUBLIC bool Value<std::string>::is_shape () const
 {
   return false;
 }
 
 template <> RDB_PUBLIC bool Value<db::DPolygon>::is_shape () const
 {
@@ -399,14 +472,66 @@
 Values &
 Values::operator= (const Values &d)
 {
   m_values = d.m_values;
   return *this;
 }
 
+bool
+Values::compare (const Values &other, const std::map<id_type, id_type> &tag_map, const std::map<id_type, id_type> &rev_tag_map) const
+{
+  Values::const_iterator a = begin (), b = other.begin ();
+  while (a != end () && b != other.end ()) {
+
+    id_type t12 = 0;
+    while (a != end () && a->tag_id () != 0) {
+      auto j = tag_map.find (a->tag_id ());
+      if (j != tag_map.end ()) {
+        t12 = j->second;
+        break;
+      }
+      ++a;
+    }
+
+    id_type t2 = 0;
+    while (b != other.end () && b->tag_id () != 0) {
+      auto j = rev_tag_map.find (b->tag_id ());
+      if (j != rev_tag_map.end ()) {
+        t2 = j->first;
+        break;
+      }
+      ++b;
+    }
+
+    if (a == end () || b == other.end ()) {
+      return b != other.end ();
+    }
+
+    if (t12 != t2) {
+      return t12 < t2;
+    }
+
+    if (a->get () && b->get ()) {
+      if (rdb::ValueBase::compare (a->get (), b->get ())) {
+        return true;
+      } else if (rdb::ValueBase::compare (b->get (), a->get ())) {
+        return false;
+      }
+    } else if ((a->get () != 0) != (b->get () != 0)) {
+      return (a->get () != 0) < (b->get () != 0);
+    }
+
+    ++a;
+    ++b;
+
+  }
+
+  return b != other.end ();
+}
+
 std::string 
 Values::to_string (const Database *rdb) const
 {
   std::string r;
   r.reserve (200);
 
   for (const_iterator v = begin (); v != end (); ++v) {
@@ -443,15 +568,15 @@
 //  Cell implementation
 
 void 
 Cells::import_cell (const Cell &c)
 {
   Cell *cell;
   if (mp_database) {
-    cell = mp_database->create_cell (c.name (), c.variant ());
+    cell = mp_database->create_cell (c.name (), c.variant (), c.layout_name ());
   } else {
     cell = new Cell (0, c.name ());
     add_cell (cell);
   }
 
   for (References::const_iterator r = c.references ().begin (); r != c.references ().end (); ++r) {
     cell->references ().insert (*r);
@@ -475,16 +600,16 @@
 
 Cell::Cell (id_type id, const std::string &name)
   : m_id (id), m_name (name), m_num_items (0), m_num_items_visited (0), mp_database (0)
 {
   //  .. nothing yet ..
 }
 
-Cell::Cell (id_type id, const std::string &name, const std::string &variant)
-  : m_id (id), m_name (name), m_variant (variant), m_num_items (0), m_num_items_visited (0), mp_database (0)
+Cell::Cell (id_type id, const std::string &name, const std::string &variant, const std::string &layout_name = std::string ())
+  : m_id (id), m_name (name), m_variant (variant), m_layout_name (layout_name), m_num_items (0), m_num_items_visited (0), mp_database (0)
 {
   //  .. nothing yet ..
 }
 
 Cell::~Cell ()
 {
   //  .. nothing yet ..
@@ -808,22 +933,22 @@
   }
   return m_tags [i->second - 1];
 }
 
 const Tag &
 Tags::tag (id_type id) const
 {
-  tl_assert (id - 1 < m_tags.size () && id > 0);
+  tl_assert (id < m_tags.size () + 1 && id > 0);
   return m_tags [id - 1];
 }
 
 Tag &
 Tags::tag (id_type id)
 {
-  tl_assert (id - 1 < m_tags.size () && id > 0);
+  tl_assert (id < m_tags.size () + 1 && id > 0);
   return m_tags [id - 1];
 }
 
 void
 Tags::import_tag (const Tag &t)
 {
   Tag &tt = tag (t.name (), t.is_user_tag ());
@@ -866,14 +991,15 @@
 {
   if (this != &d) {
     m_values = d.m_values;
     m_cell_id = d.m_cell_id;
     m_category_id = d.m_category_id;
     m_visited = d.m_visited;
     m_multiplicity = d.m_multiplicity;
+    m_comment = d.m_comment;
     m_tag_ids = d.m_tag_ids;
     m_image_str = d.m_image_str;
   }
 
   return *this;
 }
 
@@ -1201,14 +1327,18 @@
     m_cells.import_cell (*c);
   }
 }
 
 Category *
 Database::create_category (Category *parent, const std::string &name)
 {
+  if (! parent) {
+    return create_category (name);
+  }
+
   set_modified ();
 
   Category *cat = create_category (&parent->sub_categories (), name);
   cat->set_parent (parent);
   return cat;
 }
 
@@ -1248,15 +1378,15 @@
     return c->second;
   } else {
     return 0;
   }
 }
 
 Cell *
-Database::create_cell (const std::string &name, const std::string &variant)
+Database::create_cell (const std::string &name, const std::string &variant, const std::string &layout_name)
 {
   set_modified ();
 
   Cell *new_cell;
 
   if (variant.empty ()) {
 
@@ -1285,31 +1415,31 @@
       for (unsigned int n = (std::numeric_limits<unsigned int>::max () / 2) + 1; n > 0; n /= 2) {
         qname = name + ":" + tl::to_string (variant_index + n);
         if (m_cells_by_qname.find (qname) != m_cells_by_qname.end ()) {
           variant_index += n;
         }
       }
 
-      new_cell = new Cell (++m_next_id, name, tl::to_string (variant_index + 1));
+      new_cell = new Cell (++m_next_id, name, tl::to_string (variant_index + 1), layout_name);
 
       variant->second.push_back (new_cell->id ());
 
     } else {
 
-      new_cell = new Cell (++m_next_id, name);
+      new_cell = new Cell (++m_next_id, name, std::string (), layout_name);
       
     }
 
     m_cells.add_cell (new_cell);
     m_cells_by_id.insert (std::make_pair (new_cell->id (), new_cell));
     m_cells_by_qname.insert (std::make_pair (new_cell->qname (), new_cell));
 
   } else {
       
-    new_cell = new Cell (++m_next_id, name, variant);
+    new_cell = new Cell (++m_next_id, name, variant, layout_name);
     m_cells.add_cell (new_cell);
     m_cells_by_id.insert (std::make_pair (new_cell->id (), new_cell));
     m_cells_by_qname.insert (std::make_pair (new_cell->qname (), new_cell));
 
     std::map <std::string, std::vector <id_type> >::iterator variant = m_cell_variants.insert (std::make_pair (name, std::vector <id_type> ())).first;
 
     //  If another cell with that name already exists, rename it to a suitable variant
@@ -1395,14 +1525,21 @@
 void  
 Database::remove_item_tag (const Item *item, id_type tag)
 {
   set_modified ();
   const_cast <Item *> (item)->remove_tag (tag);
 }
 
+void
+Database::set_item_comment (const Item *item, const std::string &comment)
+{
+  set_modified ();
+  const_cast <Item *> (item)->set_comment (comment);
+}
+
 #if defined(HAVE_QT)
 void 
 Database::set_item_image (const Item *item, const QImage &image)
 {
   set_modified ();
   const_cast <Item *> (item)->set_image (image);
 }
@@ -1621,15 +1758,15 @@
 
   if (layout.begin_top_down () != layout.end_top_down ()) {
     db->scan_layout (layout, *layout.begin_top_down (), layers, false /*hierarchical*/);
   }
 }
 
 void
-Database::load (const std::string &fn)
+Database::load (std::string fn)
 {
   tl::log << "Loading RDB from " << fn;
 
   clear ();
 
   tl::InputStream stream (fn);
 
@@ -1655,14 +1792,169 @@
   reset_modified ();
 
   if (tl::verbosity () >= 10) {
     tl::info << "Loaded RDB from " << fn;
   }
 }
 
+namespace
+{
+  class ValueMapEntryCompare
+  {
+  public:
+    ValueMapEntryCompare (const std::map<id_type, id_type> &tag2tag, const std::map<id_type, id_type> &rev_tag2tag)
+    {
+      mp_tag2tag = &tag2tag;
+      mp_rev_tag2tag = &rev_tag2tag;
+    }
+
+    bool operator() (const Item *a, const Item *b) const
+    {
+      return a->values ().compare (b->values (), *mp_tag2tag, *mp_rev_tag2tag);
+    }
+
+  private:
+    const std::map<id_type, id_type> *mp_tag2tag;
+    const std::map<id_type, id_type> *mp_rev_tag2tag;
+  };
+
+  class ValueMapEntry
+  {
+  public:
+    ValueMapEntry ()
+      : mp_tag2tag (0), mp_rev_tag2tag (0)
+    { }
+
+    void build (const rdb::Database &rdb, id_type cell_id, id_type cat_id, const std::map<id_type, id_type> &tag2tag, const std::map<id_type, id_type> &rev_tag2tag)
+    {
+      mp_tag2tag = &tag2tag;
+      mp_rev_tag2tag = &rev_tag2tag;
+
+      auto i2i = rdb.items_by_cell_and_category (cell_id, cat_id);
+
+      size_t n = 0;
+      for (auto i = i2i.first; i != i2i.second; ++i) {
+        ++n;
+      }
+      m_items.reserve (n);
+
+      for (auto i = i2i.first; i != i2i.second; ++i) {
+        m_items.push_back ((*i).operator-> ());
+      }
+
+      ValueMapEntryCompare cmp (*mp_tag2tag, *mp_rev_tag2tag);
+      std::sort (m_items.begin (), m_items.end (), cmp);
+    }
+
+    const Item *find (const rdb::Item &item) const
+    {
+      ValueMapEntryCompare cmp (*mp_tag2tag, *mp_rev_tag2tag);
+
+      auto i = std::lower_bound (m_items.begin (), m_items.end (), &item, cmp);
+      if (i == m_items.end ()) {
+        return 0;
+      }
+
+      if (cmp (&item, *i) || cmp (*i, &item)) {
+        return 0;
+      } else {
+        return *i;
+      }
+    }
+
+  public:
+    std::vector<const Item *> m_items;
+    const std::map<id_type, id_type> *mp_tag2tag;
+    const std::map<id_type, id_type> *mp_rev_tag2tag;
+  };
+}
+
+static void map_category (const rdb::Category &cat, const rdb::Database &db, std::map<id_type, id_type> &cat2cat)
+{
+  const rdb::Category *this_cat = db.category_by_name (cat.path ());
+  if (this_cat) {
+    cat2cat.insert (std::make_pair (this_cat->id (), cat.id ()));
+  }
+
+  for (auto c = cat.sub_categories ().begin (); c != cat.sub_categories ().end (); ++c) {
+    map_category (*c, db, cat2cat);
+  }
+}
+
+void
+Database::apply (const rdb::Database &other)
+{
+  std::map<id_type, id_type> cell2cell;
+  std::map<id_type, id_type> cat2cat;
+  std::map<id_type, id_type> tag2tag;
+  std::map<id_type, id_type> rev_tag2tag;
+
+  for (auto c = other.cells ().begin (); c != other.cells ().end (); ++c) {
+    //  TODO: do we have a consistent scheme of naming variants? What requirements
+    //  exist towards detecting variant specific waivers
+    const rdb::Cell *this_cell = cell_by_qname (c->qname ());
+    if (this_cell) {
+      cell2cell.insert (std::make_pair (this_cell->id (), c->id ()));
+    }
+  }
+
+  for (auto c = other.categories ().begin (); c != other.categories ().end (); ++c) {
+    map_category (*c, *this, cat2cat);
+  }
+
+  std::map<std::string, id_type> tags_by_name;
+  for (auto c = tags ().begin_tags (); c != tags ().end_tags (); ++c) {
+    tags_by_name.insert (std::make_pair (c->name (), c->id ()));
+  }
+
+  for (auto c = other.tags ().begin_tags (); c != other.tags ().end_tags (); ++c) {
+    auto t = tags_by_name.find (c->name ());
+    if (t != tags_by_name.end ()) {
+      tag2tag.insert (std::make_pair (t->second, c->id ()));
+      rev_tag2tag.insert (std::make_pair (c->id (), t->second));
+    }
+  }
+
+  std::map<std::pair<id_type, id_type>, ValueMapEntry> value_map;
+
+  for (Items::iterator i = items_non_const ().begin (); i != items_non_const ().end (); ++i) {
+
+    auto icell = cell2cell.find (i->cell_id ());
+    if (icell == cell2cell.end ()) {
+      continue;
+    }
+
+    auto icat = cat2cat.find (i->category_id ());
+    if (icat == cat2cat.end ()) {
+      continue;
+    }
+
+    //  build a cache of value vs. value
+    auto vmap = value_map.find (std::make_pair (icell->second, icat->second));
+    if (vmap == value_map.end ()) {
+      vmap = value_map.insert (std::make_pair (std::make_pair (icell->second, icat->second), ValueMapEntry ())).first;
+      vmap->second.build (other, icell->second, icat->second, tag2tag, rev_tag2tag);
+    }
+
+    //  find a value in the reference DB
+    const rdb::Item *other = vmap->second.find (*i);
+    if (other) {
+
+      //  actually transfer the attributes here
+
+      i->set_comment (other->comment ());
+      //  TODO: this has some optimization potential in terms of performance ...
+      i->set_image_str (other->image_str ());
+      i->set_tag_str (other->tag_str ());
+
+    }
+
+  }
+}
+
 void
 Database::scan_layout (const db::Layout &layout, db::cell_index_type cell_index, const std::vector<std::pair<unsigned int, std::string> > &layers_and_descriptions, bool flat)
 {
   tl::AbsoluteProgress progress (tl::to_string (tr ("Shapes To Markers")), 10000);
   progress.set_format (tl::to_string (tr ("%.0f0000 markers")));
   progress.set_unit (10000);
```

### Comparing `klayout-0.29.0/src/rdb/rdb/rdb.h` & `klayout-0.29.1/src/rdb/rdb/rdb.h`

 * *Files 2% similar despite different names*

```diff
@@ -502,18 +502,15 @@
   }
 
   int type_index () const 
   { 
     return type_index_of<C> (); 
   }
 
-  bool compare (const ValueBase *other) const 
-  {
-    return m_value < static_cast<const Value<C> *> (other)->m_value;
-  }
+  bool compare (const ValueBase *other) const;
 
   bool is_shape () const;
 
   std::string to_string () const;
 
   std::string to_display_string () const;
 
@@ -676,14 +673,27 @@
 
   /**
    *  @brief Assignment 
    */
   Values &operator= (const Values &d);
 
   /**
+   *  @brief Compare two value sets (less operator)
+   *
+   *  This compare function will use the tag mapping provided by tag map ("this" tag id to "other" tag id).
+   *  Values with tags not listed in the tag map will not be compared.
+   *  Untagged values (tag_id 0) will be compared always.
+   *
+   *  "rev_tag_map" needs to be the reverse of "tag_map".
+   *
+   *  The order of the values matters.
+   */
+  bool compare (const Values &other, const std::map<id_type, id_type> &tag_map, const std::map<id_type, id_type> &rev_tag_map) const;
+
+  /**
    *  @brief The const iterator (begin)
    */
   const_iterator begin () const
   {
     return m_values.begin ();
   }
 
@@ -736,14 +746,22 @@
    */
   void swap (Values &other)
   {
     m_values.swap (other.m_values);
   }
 
   /**
+   *  @brief Clears the values
+   */
+  void clear ()
+  {
+    m_values.clear ();
+  }
+
+  /**
    *  @brief Convert the values collection to a string 
    */
   std::string to_string (const Database *rdb) const;
 
   /**
    *  @brief Fill the values collection from the string
    */
@@ -990,14 +1008,34 @@
    *
    *  If the image string is empty, the image will be cleared.
    *  If the image string is not valid, the image will also be cleared.
    */
   void set_image_str (const std::string &s);
 
   /**
+   *  @brief Gets the item comment
+   *
+   *  The comment string is an arbitrary string attached to the item.
+   */
+  const std::string &comment () const
+  {
+    return m_comment;
+  }
+
+  /**
+   *  @brief Sets the item comment
+   *
+   *  The comment string is an arbitrary string attached to the item.
+   */
+  void set_comment (const std::string &s)
+  {
+    m_comment = s;
+  }
+
+  /**
    *  @brief Get the database reference
    */
   Database *database ()
   {
     return mp_database;
   }
 
@@ -1013,14 +1051,15 @@
   friend class Database;
   friend class Items;
 
   Values m_values;
   id_type m_cell_id;
   id_type m_category_id;
   size_t m_multiplicity;
+  std::string m_comment;
   bool m_visited;
   std::vector <bool> m_tag_ids;
   Database *mp_database;
   std::string m_image_str;
 
   Item ();
 
@@ -1437,15 +1476,15 @@
   Cell (id_type id, const std::string &name);
 
   /**
    *  @brief the constructor from an id and a name and a variant id
    *
    *  This method is provided for persistency application only. It should not be used otherwise.
    */
-  Cell (id_type id, const std::string &name, const std::string &variant);
+  Cell (id_type id, const std::string &name, const std::string &variant, const std::string &layout_name);
 
   /**
    *  @brief Cell destructor
    */
   ~Cell ();
 
   /**
@@ -1463,50 +1502,68 @@
    */
   void set_id (id_type id) 
   {
     m_id = id;
   }
 
   /**
-   *  @brief Get the cell name
+   *  @brief Gets the cell name
    */
   const std::string &name () const
   {
     return m_name;
   }
 
   /**
-   *  @brief Set the name string (setter)
+   *  @brief Sets the name string
    *
    *  This method must not be used for items in the database to keep the database consistent.
    */
   void set_name (const std::string &d) 
   {
     m_name = d;
   }
 
   /**
-   *  @brief Get the variant id
+   *  @brief Gets the variant id
    */
   const std::string &variant () const
   {
     return m_variant;
   }
 
   /**
-   *  @brief Set the variant string (setter)
+   *  @brief Sets the variant string
    *
    *  This method must not be used for items in the database to keep the database consistent.
    */
   void set_variant (const std::string &v) 
   {
     m_variant = v;
   }
 
   /**
+   *  @brief Gets the layout cell name
+   */
+  const std::string &layout_name () const
+  {
+    return m_layout_name;
+  }
+
+  /**
+   *  @brief Sets the layout cell string
+   *
+   *  This method must not be used for items in the database to keep the database consistent.
+   */
+  void set_layout_name (const std::string &s)
+  {
+    m_layout_name = s;
+  }
+
+  /**
    *  @brief Get the qualified name (name plus optionally the variant id separated by a colon)
    */
   std::string qname () const;
 
   /**
    *  @brief Report the number of items in total
    */
@@ -1575,14 +1632,15 @@
 private:
   friend class Database;
   friend class Cells;
 
   id_type m_id;
   std::string m_name;
   std::string m_variant;
+  std::string m_layout_name;
   size_t m_num_items;
   size_t m_num_items_visited;
   References m_references;
   Database *mp_database;
 
   Cell (const Cell &d);
   Cell &operator= (const Cell &d);
@@ -2178,25 +2236,28 @@
   /**
    *  @brief Create a cell and register it
    *
    *  If a cell with that name already exists, a variant is created
    */
   Cell *create_cell (const std::string &name)
   {
-    return create_cell (name, std::string ());
+    return create_cell (name, std::string (), std::string ());
   }
 
   /**
    *  @brief Create a cell variant and register it
    *
    *  A cell with name name/variant combination must not exist already.
    *  If the variant string is empty, this method behaves the same as the 
    *  method without variant.
+   *
+   *  "layout_name" is the name of the cell in the layout. If empty, the layout
+   *  cell is assumed to be identical to "name".
    */
-  Cell *create_cell (const std::string &name, const std::string &variant);
+  Cell *create_cell (const std::string &name, const std::string &variant, const std::string &layout_name);
 
   /**
    *  @brief Get all variants registered for a given cell name (not qname!)
    *
    *  @return a vector of id's corresponding to the given variants or an empty vector if the name is not valid or the cell has no variants
    */
   const std::vector <id_type> &variants (const std::string &name);
@@ -2282,14 +2343,19 @@
   void add_item_tag (const Item *item, id_type tag);
 
   /**
    *  @brief Remove a tag from the given item
    */
   void remove_item_tag (const Item *item, id_type tag);
 
+  /**
+   *  @brief Sets the comment string of the item
+   */
+  void set_item_comment (const Item *item, const std::string &comment);
+
 #if defined(HAVE_QT)
   /**
    *  @brief Set the image of an item
    */
   void set_item_image (const Item *item, const QImage &image);
 #endif
 
@@ -2375,19 +2441,36 @@
 
   /**
    *  @brief Save the database to a file
    */
   void save (const std::string &filename);
 
   /**
+   *  @brief Write the database to a file
+   *
+   *  This function is like "save", but does not update the file name attribute.
+   */
+  void write (const std::string &filename);
+
+  /**
    *  @brief Load the database from a file
    *
-   *  @brief This clears the existing database.
+   *  Note: This clears the existing database.
+   *  The argument intentionally is a copy, so we can call
+   *  "load (this->filename ())" for reloading.
+   */
+  void load (std::string filename);
+
+  /**
+   *  @brief Applies the attributes from a different database
+   *
+   *  Attributes are waived flags, images etc.
+   *  The attributes are applied to markers with identical value(s), category and cell context.
    */
-  void load (const std::string &filename);
+  void apply (const rdb::Database &other);
 
   /**
    *  @brief Scans a layout into this RDB
    *
    *  @param layout The layout to scan
    *  @param cell_index The top cell to scan
    *  @param layers_and_descriptions The layers and (optional) descriptions/names of the layer to scan
```

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbCommon.h` & `klayout-0.29.1/src/rdb/rdb/rdbCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbFile.cc` & `klayout-0.29.1/src/rdb/rdb/rdbFile.cc`

 * *Files 9% similar despite different names*

```diff
@@ -87,50 +87,60 @@
       &categories_format
     ) +
     tl::make_element_with_parent_ref<rdb::Cells, rdb::Database> (&rdb::Database::cells, &rdb::Database::import_cells, "cells",
       // must be sorted cells (children after parents)!
       tl::make_element_with_parent_ref<rdb::Cell, rdb::Cells::const_iterator, rdb::Cells> (&rdb::Cells::begin, &rdb::Cells::end, &rdb::Cells::import_cell, "cell", 
         tl::make_member<std::string, rdb::Cell> (&rdb::Cell::name, &rdb::Cell::set_name, "name") +
         tl::make_member<std::string, rdb::Cell> (&rdb::Cell::variant, &rdb::Cell::set_variant, "variant") +
-        tl::make_element_with_parent_ref<rdb::References, rdb::Cell> (&rdb::Cell::references, &rdb::Cell::import_references, "references", 
+        tl::make_member<std::string, rdb::Cell> (&rdb::Cell::layout_name, &rdb::Cell::set_layout_name, "layout-name") +
+        tl::make_element_with_parent_ref<rdb::References, rdb::Cell> (&rdb::Cell::references, &rdb::Cell::import_references, "references",
           tl::make_element_with_parent_ref<rdb::Reference, rdb::References::const_iterator, rdb::References> (&rdb::References::begin, &rdb::References::end, &rdb::References::insert, "ref", 
             tl::make_member<std::string, rdb::Reference> (&rdb::Reference::parent_cell_qname, &rdb::Reference::set_parent_cell_qname, "parent") + 
             tl::make_member<std::string, rdb::Reference> (&rdb::Reference::trans_str, &rdb::Reference::set_trans_str, "trans") 
           )
         )
       )
     ) + 
     tl::make_element_with_parent_ref<rdb::Items, rdb::Database> (&rdb::Database::items, &rdb::Database::set_items, "items",
       tl::make_element_with_parent_ref<rdb::Item, rdb::Items::const_iterator, rdb::Items> (&rdb::Items::begin, &rdb::Items::end, &rdb::Items::add_item, "item", 
         tl::make_member<std::string, rdb::Item> (&rdb::Item::tag_str, &rdb::Item::set_tag_str, "tags") + 
         tl::make_member<std::string, rdb::Item> (&rdb::Item::category_name, &rdb::Item::set_category_name, "category") + 
         tl::make_member<std::string, rdb::Item> (&rdb::Item::cell_qname, &rdb::Item::set_cell_qname, "cell") +
         tl::make_member<bool, rdb::Item> (&rdb::Item::visited, &rdb::Item::set_visited, "visited") +
         tl::make_member<size_t, rdb::Item> (&rdb::Item::multiplicity, &rdb::Item::set_multiplicity, "multiplicity") +
+        tl::make_member<std::string, rdb::Item> (&rdb::Item::comment, &rdb::Item::set_comment, "comment") +
         tl::make_member<std::string, rdb::Item> (&rdb::Item::image_str, &rdb::Item::set_image_str, "image") +
         tl::make_element<rdb::Values, rdb::Item> (&rdb::Item::values, &rdb::Item::set_values, "values", 
           tl::make_member<rdb::ValueWrapper, rdb::Values::const_iterator, rdb::Values> (&rdb::Values::begin, &rdb::Values::end, &rdb::Values::add, "value", ValueConverter (rdb)) 
         )
       )
     )
   );
 }
 
 // -------------------------------------------------------------
-//  Implementation of rdb::Database::save
+//  Implementation of rdb::Database::save and write
 //  TODO: move this somewhere else - with generalized functionality
 
 void
 rdb::Database::save (const std::string &fn)
 {
-  tl::OutputStream os (fn, tl::OutputStream::OM_Auto);
-  make_rdb_structure (this).write (os, *this); 
+  write (fn);
   set_filename (fn);
+}
+
+void
+rdb::Database::write (const std::string &fn)
+{
+  tl::OutputStream os (fn, tl::OutputStream::OM_Auto);
+  make_rdb_structure (this).write (os, *this);
 
-  tl::log << "Saved RDB to " << fn;
+  if (tl::verbosity () >= 10) {
+    tl::log << "Saved RDB to " << fn;
+  }
 }
 
 // -------------------------------------------------------------
 //  Implementation of rdb::Database::load and the standard file plugin
 
 class StandardReader 
   : public ReaderBase
```

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbForceLink.cc` & `klayout-0.29.1/src/rdb/rdb/rdbForceLink.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbForceLink.h` & `klayout-0.29.1/src/rdb/rdb/rdbForceLink.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbRVEReader.cc` & `klayout-0.29.1/src/rdb/rdb/rdbRVEReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbReader.cc` & `klayout-0.29.1/src/rdb/rdb/rdbReader.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbReader.h` & `klayout-0.29.1/src/rdb/rdb/rdbReader.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbTiledRdbOutputReceiver.cc` & `klayout-0.29.1/src/rdb/rdb/rdbTiledRdbOutputReceiver.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbTiledRdbOutputReceiver.h` & `klayout-0.29.1/src/rdb/rdb/rdbTiledRdbOutputReceiver.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbUtils.cc` & `klayout-0.29.1/src/rdb/rdb/rdbUtils.cc`

 * *Files 2% similar despite different names*

```diff
@@ -170,18 +170,36 @@
   db::CplxTrans m_trans;
   rdb::Cell *mp_rdb_cell;
   bool m_with_properties;
 
   const rdb::Cell *cell_for_id (const db::Layout *layout, db::cell_index_type ci)
   {
     tl_assert (layout != 0);
+
     std::string cn = layout->cell_name (ci);
-    const rdb::Cell *rdb_cell = mp_rdb->cell_by_qname (cn);
+    std::string layout_cn = cn;
+    std::string qname = cn;
+    std::string var;
+
+    //  resolve references to original cells in deep mode and determine variant
+    if (layout->builder ()) {
+      const db::Layout *source = layout->builder ()->source ().layout ();
+      if (source) {
+        const std::pair<db::cell_index_type, std::string> &vs = layout->builder ()->variant_of_source (ci);
+        if (! vs.second.empty () && source->is_valid_cell_index (vs.first)) {
+          var = vs.second;
+          cn = source->cell_name (vs.first);
+          qname = cn + ":" + var;
+        }
+      }
+    }
+
+    const rdb::Cell *rdb_cell = mp_rdb->cell_by_qname (qname);
     if (! rdb_cell) {
-      return mp_rdb->create_cell (cn);
+      return mp_rdb->create_cell (cn, var, layout_cn);
     } else {
       return rdb_cell;
     }
   }
 };
 
 class CreateItemsFlatReceiver
```

### Comparing `klayout-0.29.0/src/rdb/rdb/rdbUtils.h` & `klayout-0.29.1/src/rdb/rdb/rdbUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/atomic/atomic.h` & `klayout-0.29.1/src/tl/tl/atomic/atomic.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/atomic/atomic_msvc.h` & `klayout-0.29.1/src/tl/tl/atomic/atomic_msvc.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/atomic/spinlock.h` & `klayout-0.29.1/src/tl/tl/atomic/spinlock.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlAlgorithm.h` & `klayout-0.29.1/src/tl/tl/tlAlgorithm.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlArch.cc` & `klayout-0.29.1/src/tl/tl/tlArch.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlArch.h` & `klayout-0.29.1/src/tl/tl/tlArch.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlAssert.cc` & `klayout-0.29.1/src/tl/tl/tlAssert.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlAssert.h` & `klayout-0.29.1/src/tl/tl/tlAssert.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlBase64.cc` & `klayout-0.29.1/src/tl/tl/tlBase64.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlBase64.h` & `klayout-0.29.1/src/tl/tl/tlBase64.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlClassRegistry.cc` & `klayout-0.29.1/src/tl/tl/tlClassRegistry.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlClassRegistry.h` & `klayout-0.29.1/src/tl/tl/tlClassRegistry.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlColor.cc` & `klayout-0.29.1/src/tl/tl/tlColor.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlColor.h` & `klayout-0.29.1/src/tl/tl/tlColor.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCommandLineParser.cc` & `klayout-0.29.1/src/tl/tl/tlCommandLineParser.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCommandLineParser.h` & `klayout-0.29.1/src/tl/tl/tlCommandLineParser.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCommon.h` & `klayout-0.29.1/src/tl/tl/tlCommon.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCopyOnWrite.cc` & `klayout-0.29.1/src/tl/tl/tlCopyOnWrite.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCopyOnWrite.h` & `klayout-0.29.1/src/tl/tl/tlCopyOnWrite.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlCpp.h` & `klayout-0.29.1/src/tl/tl/tlCpp.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDataMapping.cc` & `klayout-0.29.1/src/tl/tl/tlDataMapping.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDataMapping.h` & `klayout-0.29.1/src/tl/tl/tlDataMapping.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeferredExecution.cc` & `klayout-0.29.1/src/tl/tl/tlDeferredExecution.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeferredExecution.h` & `klayout-0.29.1/src/tl/tl/tlDeferredExecution.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeferredExecutionQt.cc` & `klayout-0.29.1/src/tl/tl/tlDeferredExecutionQt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeferredExecutionQt.h` & `klayout-0.29.1/src/tl/tl/tlDeferredExecutionQt.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeflate.cc` & `klayout-0.29.1/src/tl/tl/tlDeflate.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDeflate.h` & `klayout-0.29.1/src/tl/tl/tlDeflate.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlDefs.h` & `klayout-0.29.1/src/tl/tl/tlDefs.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEnv.cc` & `klayout-0.29.1/src/tl/tl/tlEnv.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEnv.h` & `klayout-0.29.1/src/tl/tl/tlEnv.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEquivalenceClusters.cc` & `klayout-0.29.1/src/tl/tl/tlEquivalenceClusters.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEquivalenceClusters.h` & `klayout-0.29.1/src/tl/tl/tlEquivalenceClusters.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEvents.cc` & `klayout-0.29.1/src/tl/tl/tlEvents.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEvents.h` & `klayout-0.29.1/src/tl/tl/tlEvents.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlEventsVar.h` & `klayout-0.29.1/src/tl/tl/tlEventsVar.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlException.cc` & `klayout-0.29.1/src/tl/tl/tlException.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlException.h` & `klayout-0.29.1/src/tl/tl/tlException.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlExceptions.cc` & `klayout-0.29.1/src/tl/tl/tlExceptions.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlExceptions.h` & `klayout-0.29.1/src/tl/tl/tlExceptions.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlExpression.cc` & `klayout-0.29.1/src/tl/tl/tlExpression.cc`

 * *Files 2% similar despite different names*

```diff
@@ -141,75 +141,75 @@
     return std::string (tl::to_string (tr ("[unspecified location]")));
   }
 }
 
 // ----------------------------------------------------------------------------
 //  Utilities for evaluation
 
-static double to_double (const ExpressionParserContext &context, const tl::Variant &v)
+static double to_double (const ExpressionParserContext &context, const tl::Variant &v, unsigned int narg)
 {
   if (v.can_convert_to_double ()) {
     return v.to_double ();
   } else if (v.is_list ()) {
     return v.get_list ().size ();
   } else {
-    throw EvalError (tl::to_string (tr ("Double precision floating point value expected")), context);
+    throw EvalError (tl::to_string (tr ("Double precision floating point value expected for argument #")) + tl::to_string (narg + 1), context);
   }
 }
 
 static double to_double (const ExpressionParserContext &context, const std::vector <tl::Variant> &v)
 {
   if (v.size () != 1) {
     throw EvalError (tl::to_string (tr ("Function expects a single numeric argument")), context);
   }
 
-  return to_double (context, v [0]);
+  return to_double (context, v [0], 0);
 }
 
-static long to_long (const ExpressionParserContext &context, const tl::Variant &v)
+static long to_long (const ExpressionParserContext &context, const tl::Variant &v, int narg)
 {
   if (v.can_convert_to_long ()) {
     return v.to_long ();
   } else if (v.is_list ()) {
     return long (v.get_list ().size ());
   } else {
-    throw EvalError (tl::to_string (tr ("Integer value expected")), context);
+    throw EvalError (tl::to_string (tr ("Integer value expected for argument #")) + tl::to_string (narg + 1), context);
   }
 }
 
-static unsigned long to_ulong (const ExpressionParserContext &context, const tl::Variant &v)
+static unsigned long to_ulong (const ExpressionParserContext &context, const tl::Variant &v, int narg)
 {
   if (v.can_convert_to_ulong ()) {
     return v.to_ulong ();
   } else if (v.is_list ()) {
     return (unsigned long) (v.get_list ().size ());
   } else {
-    throw EvalError (tl::to_string (tr ("Unsigned integer value expected")), context);
+    throw EvalError (tl::to_string (tr ("Unsigned integer value expected for argument #")) + tl::to_string (narg + 1), context);
   }
 }
 
-static long long to_longlong (const ExpressionParserContext &context, const tl::Variant &v)
+static long long to_longlong (const ExpressionParserContext &context, const tl::Variant &v, int narg)
 {
   if (v.can_convert_to_longlong ()) {
     return v.to_longlong ();
   } else if (v.is_list ()) {
     return long (v.get_list ().size ());
   } else {
-    throw EvalError (tl::to_string (tr ("Integer value expected")), context);
+    throw EvalError (tl::to_string (tr ("Integer value expected for argument #")) + tl::to_string (narg + 1), context);
   }
 }
 
-static unsigned long long to_ulonglong (const ExpressionParserContext &context, const tl::Variant &v)
+static unsigned long long to_ulonglong (const ExpressionParserContext &context, const tl::Variant &v, int narg)
 {
   if (v.can_convert_to_ulonglong ()) {
     return v.to_ulong ();
   } else if (v.is_list ()) {
     return (unsigned long long) (v.get_list ().size ());
   } else {
-    throw EvalError (tl::to_string (tr ("Unsigned integer value expected")), context);
+    throw EvalError (tl::to_string (tr ("Unsigned integer value expected for argument #")) + tl::to_string (narg + 1), context);
   }
 }
 
 // ----------------------------------------------------------------------------
 //  EvalTarget: a class that encapsulates the target of an evaluation
 
 class TL_PUBLIC EvalTarget
@@ -1085,21 +1085,21 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "<<", vv, 0);
       v.swap (o);
 
     } else if (v->is_longlong ()) {
-      v.set (tl::Variant (v->to_longlong () << to_longlong (m_context, *b)));
+      v.set (tl::Variant (v->to_longlong () << to_longlong (m_context, *b, 1)));
     } else if (v->is_ulonglong ()) {
-      v.set (tl::Variant (v->to_ulonglong () << to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (v->to_ulonglong () << to_ulonglong (m_context, *b, 1)));
     } else if (v->is_ulong ()) {
-      v.set (tl::Variant (v->to_ulong () << to_ulong (m_context, *b)));
+      v.set (tl::Variant (v->to_ulong () << to_ulong (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_long (m_context, *v) << to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) << to_long (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Shift right expression node
  */
@@ -1141,21 +1141,21 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), ">>", vv, 0);
       v.swap (o);
 
     } else if (v->is_longlong ()) {
-      v.set (tl::Variant (v->to_longlong () >> to_longlong (m_context, *b)));
+      v.set (tl::Variant (v->to_longlong () >> to_longlong (m_context, *b, 1)));
     } else if (v->is_ulonglong ()) {
-      v.set (tl::Variant (v->to_ulonglong () >> to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (v->to_ulonglong () >> to_ulonglong (m_context, *b, 1)));
     } else if (v->is_ulong ()) {
-      v.set (tl::Variant (v->to_ulong () >> to_ulong (m_context, *b)));
+      v.set (tl::Variant (v->to_ulong () >> to_ulong (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_long (m_context, *v) >> to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) >> to_long (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Plus expression node
  */
@@ -1199,25 +1199,25 @@
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "+", vv, 0);
       v.swap (o);
 
     } else if (v->is_a_string () || b->is_a_string ()) {
       v.set (tl::Variant (std::string (v->to_string ()) + b->to_string ()));
     } else if (v->is_double () || b->is_double ()) {
-      v.set (tl::Variant (to_double (m_context, *v) + to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) + to_double (m_context, *b, 1)));
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) + to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) + to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) + to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) + to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) + to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) + to_ulong (m_context, *b, 1)));
     } else if (v->is_long () || b->is_long ()) {
-      v.set (tl::Variant (to_long (m_context, *v) + to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) + to_long (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_double (m_context, *v) + to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) + to_double (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Minus expression node
  */
@@ -1259,25 +1259,25 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "-", vv, 0);
       v.swap (o);
 
     } else if (v->is_double () || b->is_double ()) {
-      v.set (tl::Variant (to_double (m_context, *v) - to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) - to_double (m_context, *b, 1)));
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) - to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) - to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) - to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) - to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) - to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) - to_ulong (m_context, *b, 1)));
     } else if (v->is_long () || b->is_long ()) {
-      v.set (tl::Variant (to_long (m_context, *v) - to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) - to_long (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_double (m_context, *v) - to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) - to_double (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Star expression node
  */
@@ -1320,54 +1320,54 @@
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "*", vv, 0);
       v.swap (o);
 
     } else if (v->is_a_string ()) {
 
-      long x = to_long (m_context, *b);
+      long x = to_long (m_context, *b, 1);
       if (x < 0) {
         throw EvalError (tl::to_string (tr ("Numeric argument of '*' operator with string must be positive")), m_context);
       }
 
       std::string s;
       s.reserve (strlen (v->to_string ()) * size_t (x));
       while (x-- > 0) {
         s += v->to_string ();
       }
 
       v.set (tl::Variant (s));
 
     } else if (b->is_a_string ()) {
 
-      long x = to_long (m_context, *v);
+      long x = to_long (m_context, *v, 0);
       if (x < 0) {
         throw EvalError (tl::to_string (tr ("Numeric argument of '*' operator with string must be positive")), m_context);
       }
 
       std::string s;
       s.reserve (strlen (b->to_string ()) * size_t (x));
       while (x-- > 0) {
         s += b->to_string ();
       }
 
       v.set (tl::Variant (s));
 
     } else if (v->is_double () || b->is_double ()) {
-      v.set (tl::Variant (to_double (m_context, *v) * to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) * to_double (m_context, *b, 1)));
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) * to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) * to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) * to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) * to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) * to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) * to_ulong (m_context, *b, 1)));
     } else if (v->is_long () || b->is_long ()) {
-      v.set (tl::Variant (to_long (m_context, *v) * to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) * to_long (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_double (m_context, *v) * to_double (m_context, *b)));
+      v.set (tl::Variant (to_double (m_context, *v, 0) * to_double (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Slash expression node
  */
@@ -1409,49 +1409,49 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "/", vv, 0);
       v.swap (o);
 
     } else if (v->is_double () || b->is_double ()) {
-      double d = to_double (m_context, *b);
+      double d = to_double (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_double (m_context, *v) / d));
+      v.set (tl::Variant (to_double (m_context, *v, 0) / d));
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      unsigned long long d = to_ulonglong (m_context, *b);
+      unsigned long long d = to_ulonglong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_ulonglong (m_context, *v) / d));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) / d));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      long long d = to_longlong (m_context, *b);
+      long long d = to_longlong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_longlong (m_context, *v) / d));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) / d));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      unsigned long d = to_ulong (m_context, *b);
+      unsigned long d = to_ulong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_ulong (m_context, *v) / d));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) / d));
     } else if (v->is_long () || b->is_long ()) {
-      long d = to_long (m_context, *b);
+      long d = to_long (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_long (m_context, *v) / d));
+      v.set (tl::Variant (to_long (m_context, *v, 0) / d));
     } else {
-      double d = to_double (m_context, *b);
+      double d = to_double (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Division by zero")), m_context);
       }
-      v.set (tl::Variant (to_double (m_context, *v) / d));
+      v.set (tl::Variant (to_double (m_context, *v, 0) / d));
     }
   }
 };
 
 /**
  *  @brief Percent expression node
  */
@@ -1493,37 +1493,37 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "%", vv, 0);
       v.swap (o);
 
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      unsigned long long d = to_ulonglong (m_context, *b);
+      unsigned long long d = to_ulonglong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Modulo by zero")), m_context);
       }
-      v.set (tl::Variant (to_ulonglong (m_context, *v) % d));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) % d));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      long long d = to_longlong (m_context, *b);
+      long long d = to_longlong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Modulo by zero")), m_context);
       }
-      v.set (tl::Variant (to_longlong (m_context, *v) % d));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) % d));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      unsigned long d = to_ulong (m_context, *b);
+      unsigned long d = to_ulong (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Modulo by zero")), m_context);
       }
-      v.set (tl::Variant (to_ulong (m_context, *v) % d));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) % d));
     } else {
-      long d = to_long (m_context, *b);
+      long d = to_long (m_context, *b, 1);
       if (d == 0) {
         throw EvalError (tl::to_string (tr ("Modulo by zero")), m_context);
       }
-      v.set (tl::Variant (to_long (m_context, *v) % d));
+      v.set (tl::Variant (to_long (m_context, *v, 0) % d));
     }
   }
 };
 
 /**
  *  @brief Ampersand expression node
  */
@@ -1565,21 +1565,21 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "&", vv, 0);
       v.swap (o);
 
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) & to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) & to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) & to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) & to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) & to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) & to_ulong (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_long (m_context, *v) & to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) & to_long (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Pipe expression node
  */
@@ -1621,21 +1621,21 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "|", vv, 0);
       v.swap (o);
 
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) | to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) | to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) | to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) | to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) | to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) | to_ulong (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_long (m_context, *v) | to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) | to_long (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Acute expression node
  */
@@ -1677,21 +1677,21 @@
       tl::Variant o;
       std::vector <tl::Variant> vv;
       vv.push_back (*b);
       c->execute (m_context, o, v.get (), "^", vv, 0);
       v.swap (o);
 
     } else if (v->is_ulonglong () || b->is_ulonglong ()) {
-      v.set (tl::Variant (to_ulonglong (m_context, *v) ^ to_ulonglong (m_context, *b)));
+      v.set (tl::Variant (to_ulonglong (m_context, *v, 0) ^ to_ulonglong (m_context, *b, 1)));
     } else if (v->is_longlong () || b->is_longlong ()) {
-      v.set (tl::Variant (to_longlong (m_context, *v) ^ to_longlong (m_context, *b)));
+      v.set (tl::Variant (to_longlong (m_context, *v, 0) ^ to_longlong (m_context, *b, 1)));
     } else if (v->is_ulong () || b->is_ulong ()) {
-      v.set (tl::Variant (to_ulong (m_context, *v) ^ to_ulong (m_context, *b)));
+      v.set (tl::Variant (to_ulong (m_context, *v, 0) ^ to_ulong (m_context, *b, 1)));
     } else {
-      v.set (tl::Variant (to_long (m_context, *v) ^ to_long (m_context, *b)));
+      v.set (tl::Variant (to_long (m_context, *v, 0) ^ to_long (m_context, *b, 1)));
     }
   }
 };
 
 /**
  *  @brief Index expression node
  */
@@ -1822,15 +1822,15 @@
     } else if (v->is_ulong ()) {
       v.set (-long (v->to_ulong ()));
     } else if (v->is_longlong ()) {
       v.set (-v->to_longlong ());
     } else if (v->is_ulonglong ()) {
       v.set (-(long long)(v->to_ulonglong ()));
     } else {
-      v.set (-to_double (m_context, *v));
+      v.set (-to_double (m_context, *v, 0));
     }
   }
 };
 
 /**
  *  @brief Unary tilde expression node
  */
@@ -1877,15 +1877,15 @@
     } else if (v->is_ulong ()) {
       v.set (~v->to_ulong ());
     } else if (v->is_longlong ()) {
       v.set (~v->to_longlong ());
     } else if (v->is_ulonglong ()) {
       v.set (~v->to_ulonglong ());
     } else {
-      v.set (~to_long (m_context, *v));
+      v.set (~to_long (m_context, *v, 0));
     }
   }
 };
 
 /**
  *  @brief Unary not expression node
  */
@@ -2384,15 +2384,15 @@
   } else if (v[0].is_longlong ()) {
     out = llabs (v[0].to_longlong ());
   } else if (v[0].is_ulonglong ()) {
     out = v[0].to_ulonglong ();
   } else if (v[0].is_double ()) {
     out = fabs (v[0].to_double ());
   } else {
-    out = labs (to_long (context, v[0]));
+    out = labs (to_long (context, v[0], 0));
   }
 }
 
 static void
 acos_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &v)
 {
   out = acos (to_double (context, v));
@@ -2459,25 +2459,25 @@
 static void
 pow_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
 {
   if (vv.size () != 2) {
     throw EvalError (tl::to_string (tr ("'pow' function expects exactly two arguments")), context);
   }
 
-  out = pow (to_double (context, vv [0]), to_double (context, vv [1]));
+  out = pow (to_double (context, vv [0], 0), to_double (context, vv [1], 1));
 }
 
 static void
 atan2_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
 {
   if (vv.size () != 2) {
     throw EvalError (tl::to_string (tr ("'atan2' function expects exactly two arguments")), context);
   }
 
-  out = atan2 (to_double (context, vv [0]), to_double (context, vv [1]));
+  out = atan2 (to_double (context, vv [0], 0), to_double (context, vv [1], 1));
 }
 
 static void
 to_f_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
 {
   if (vv.size () != 1) {
     throw EvalError (tl::to_string (tr ("'to_f' function expects exactly one argument")), context);
@@ -2686,18 +2686,18 @@
     throw EvalError (tl::to_string (tr ("'substr' function expects two or three arguments")), context);
   }
 
   std::string s (vv [0].to_string ());
 
   long len = -1;
   if (vv.size () > 2) {
-    len = std::max (long (0), to_long (context, vv [2]));
+    len = std::max (long (0), to_long (context, vv [2], 2));
   }
 
-  long l = to_long (context, vv [1]);
+  long l = to_long (context, vv [1], 1);
   if (l < 0) {
     l = long (s.size ()) + l;
     if (l < 0) {
       len += l;
       l = 0;
     }
   } 
@@ -2710,14 +2710,34 @@
     out = std::string (s, from);
   } else {
     out = std::string (s, from, len);
   }
 }
 
 static void
+upcase_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
+{
+  if (vv.size () != 1) {
+    throw EvalError (tl::to_string (tr ("'upcase' function expects one argument")), context);
+  }
+
+  out = tl::to_upper_case (vv [0].to_string ());
+}
+
+static void
+downcase_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
+{
+  if (vv.size () != 1) {
+    throw EvalError (tl::to_string (tr ("'upcase' function expects one argument")), context);
+  }
+
+  out = tl::to_lower_case (vv [0].to_string ());
+}
+
+static void
 join_f (const ExpressionParserContext &context, tl::Variant &out, const std::vector <tl::Variant> &vv)
 {
   if (vv.size () != 2) {
     throw EvalError (tl::to_string (tr ("'join' function expects exactly two arguments")), context);
   }
 
   if (! vv[0].is_list ()) {
@@ -2748,15 +2768,15 @@
     throw EvalError (tl::to_string (tr ("'item' function expects exactly two arguments")), context);
   }
 
   if (! vv[0].is_list ()) {
     throw EvalError (tl::to_string (tr ("First argument of 'item' function must be a list")), context);
   }
 
-  long index = to_long (context, vv [1]);
+  long index = to_long (context, vv [1], 1);
   if (index < 0 || index >= long (vv [0].end () - vv [0].begin ())) {
     out = tl::Variant ();
   } else {
     out = *(vv [0].begin () + index);
   }
 }
 
@@ -3038,14 +3058,16 @@
 static EvalStaticFunction f52 ("path", &path_f);
 static EvalStaticFunction f53 ("basename", &basename_f);
 static EvalStaticFunction f54 ("extension", &extension_f);
 static EvalStaticFunction f55 ("file_exists", &file_exists_f);
 static EvalStaticFunction f56 ("is_dir", &is_dir_f);
 static EvalStaticFunction f57 ("combine", &combine_f);
 static EvalStaticFunction f58 ("abs", &abs_f);
+static EvalStaticFunction f59 ("upcase", &upcase_f);
+static EvalStaticFunction f60 ("downcase", &downcase_f);
 
 // ----------------------------------------------------------------------------
 //  Implementation of a constant wrapper
 
 class EvalStaticConstant 
 {
 public:
```

### Comparing `klayout-0.29.0/src/tl/tl/tlExpression.h` & `klayout-0.29.1/src/tl/tl/tlExpression.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlFileSystemWatcher.cc` & `klayout-0.29.1/src/tl/tl/tlFileSystemWatcher.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlFileSystemWatcher.h` & `klayout-0.29.1/src/tl/tl/tlFileSystemWatcher.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlFileUtils.cc` & `klayout-0.29.1/src/tl/tl/tlFileUtils.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlFileUtils.h` & `klayout-0.29.1/src/tl/tl/tlFileUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlFixedVector.h` & `klayout-0.29.1/src/tl/tl/tlFixedVector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlGit.cc` & `klayout-0.29.1/src/tl/tl/tlGit.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlGit.h` & `klayout-0.29.1/src/tl/tl/tlGit.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlGlobPattern.cc` & `klayout-0.29.1/src/tl/tl/tlGlobPattern.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlGlobPattern.h` & `klayout-0.29.1/src/tl/tl/tlGlobPattern.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHeap.cc` & `klayout-0.29.1/src/tl/tl/tlHeap.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHeap.h` & `klayout-0.29.1/src/tl/tl/tlHeap.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStream.cc` & `klayout-0.29.1/src/tl/tl/tlHttpStream.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStream.h` & `klayout-0.29.1/src/tl/tl/tlHttpStream.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStreamCurl.cc` & `klayout-0.29.1/src/tl/tl/tlHttpStreamCurl.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStreamCurl.h` & `klayout-0.29.1/src/tl/tl/tlHttpStreamCurl.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStreamNoQt.cc` & `klayout-0.29.1/src/tl/tl/tlHttpStreamNoQt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStreamQt.cc` & `klayout-0.29.1/src/tl/tl/tlHttpStreamQt.cc`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 #include "tlHttpStream.h"
 #include "tlHttpStreamQt.h"
 #include "tlLog.h"
 #include "tlStaticObjects.h"
 #include "tlDeferredExecution.h"
 #include "tlObject.h"
 #include "tlTimer.h"
+#include "tlSleep.h"
 
 #include <QNetworkAccessManager>
 #include <QNetworkReply>
 #include <QNetworkRequest>
 #include <QNetworkProxy>
 #include <QAuthenticator>
 #include <QCoreApplication>
@@ -443,17 +444,26 @@
   //  Prevents deferred methods to be executed during the processEvents below (undesired side effects)
   tl::NoDeferredMethods silent;
 
   if (mp_reply == 0) {
     issue_request (QUrl (tl::to_qstring (m_url)));
   }
 
-  tl::Clock start_time = tl::Clock::current ();
-  while (mp_reply == 0 && (m_timeout <= 0.0 || (tl::Clock::current() - start_time).seconds () < m_timeout)) {
+  const unsigned long tick_ms = 10;
+  double time_waited = 0.0;
+
+  while (mp_reply == 0 && (m_timeout <= 0.0 || time_waited < m_timeout)) {
+
     mp_stream->tick ();
+
+    //  NOTE: as tick() includes waiting for the password dialog, we must not include
+    //  the time spent there.
+    tl::msleep (tick_ms);
+    time_waited += tick_ms * 1e-3;
+
   }
 
   if (! mp_reply) {
 
     //  Reason for this may be HTTPS initialization failure (OpenSSL)
 
     std::string em = tl::to_string (QObject::tr ("Request creation failed"));
```

### Comparing `klayout-0.29.0/src/tl/tl/tlHttpStreamQt.h` & `klayout-0.29.1/src/tl/tl/tlHttpStreamQt.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInclude.cc` & `klayout-0.29.1/src/tl/tl/tlInclude.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInclude.h` & `klayout-0.29.1/src/tl/tl/tlInclude.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInt128Support.cc` & `klayout-0.29.1/src/tl/tl/tlInt128Support.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInt128Support.h` & `klayout-0.29.1/src/tl/tl/tlInt128Support.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInternational.cc` & `klayout-0.29.1/src/tl/tl/tlInternational.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlInternational.h` & `klayout-0.29.1/src/tl/tl/tlInternational.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlIntervalMap.h` & `klayout-0.29.1/src/tl/tl/tlIntervalMap.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlIntervalSet.h` & `klayout-0.29.1/src/tl/tl/tlIntervalSet.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlIteratorUtils.h` & `klayout-0.29.1/src/tl/tl/tlIteratorUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlKDTree.h` & `klayout-0.29.1/src/tl/tl/tlKDTree.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlList.cc` & `klayout-0.29.1/src/tl/tl/tlList.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlList.h` & `klayout-0.29.1/src/tl/tl/tlList.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlLog.cc` & `klayout-0.29.1/src/tl/tl/tlLog.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlLog.h` & `klayout-0.29.1/src/tl/tl/tlLog.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlLongInt.cc` & `klayout-0.29.1/src/tl/tl/tlLongInt.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlLongInt.h` & `klayout-0.29.1/src/tl/tl/tlLongInt.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlMath.h` & `klayout-0.29.1/src/tl/tl/tlMath.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlObject.cc` & `klayout-0.29.1/src/tl/tl/tlObject.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlObject.h` & `klayout-0.29.1/src/tl/tl/tlObject.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlObjectCollection.h` & `klayout-0.29.1/src/tl/tl/tlObjectCollection.h`

 * *Files 5% similar despite different names*

```diff
@@ -112,20 +112,18 @@
     mp_holder = mp_holder->prev;
     return *this;
   }
 
   /**
    *  @brief Post-decrement
    */
-  weak_or_shared_collection_iterator<T, Holder, Shared> operator-- (int n)
+  weak_or_shared_collection_iterator<T, Holder, Shared> operator-- (int)
   {
     weak_or_shared_collection_iterator<T, Holder, Shared> ret = *this;
-    while (n-- > 0) {
-      operator-- ();
-    }
+    operator-- ();
     return ret;
   }
 
   /**
    *  @brief Pre-increment
    */
   weak_or_shared_collection_iterator<T, Holder, Shared> &operator++ ()
@@ -134,20 +132,18 @@
     mp_holder = mp_holder->next;
     return *this;
   }
 
   /**
    *  @brief Post-increment
    */
-  weak_or_shared_collection_iterator<T, Holder, Shared> operator++ (int n)
+  weak_or_shared_collection_iterator<T, Holder, Shared> operator++ (int)
   {
     weak_or_shared_collection_iterator<T, Holder, Shared> ret = *this;
-    while (n-- > 0) {
-      operator++ ();
-    }
+    operator++ ();
     return ret;
   }
 
   /**
    *  @brief Internal: access to the holder object
    */
   Holder *holder () const
@@ -172,46 +168,44 @@
 class weak_or_shared_collection
 {
 public:
   class holder_type
     : public weak_or_shared_ptr<T, Shared>
   {
   public:
-    holder_type (weak_or_shared_collection<T, Shared> *collection)
-      : weak_or_shared_ptr<T, Shared> (), next (0), prev (0), mp_collection (collection)
+    holder_type (weak_or_shared_collection<T, Shared> *_collection)
+      : weak_or_shared_ptr<T, Shared> (), next (0), prev (0), collection (_collection)
     {
       //  .. nothing yet ..
     }
 
-    holder_type (weak_or_shared_collection<T, Shared> *collection, T *t)
-      : weak_or_shared_ptr<T, Shared> (t), next (0), prev (0), mp_collection (collection)
+    holder_type (weak_or_shared_collection<T, Shared> *_collection, T *t)
+      : weak_or_shared_ptr<T, Shared> (t), next (0), prev (0), collection (_collection)
     {
       //  .. nothing yet ..
     }
 
-    holder_type (weak_or_shared_collection<T, Shared> *collection, const weak_or_shared_ptr<T, Shared> &d)
-      : weak_or_shared_ptr<T, Shared> (d), next (0), prev (0), mp_collection (collection)
+    holder_type (weak_or_shared_collection<T, Shared> *_collection, const weak_or_shared_ptr<T, Shared> &d)
+      : weak_or_shared_ptr<T, Shared> (d), next (0), prev (0), collection (_collection)
     {
       //  .. nothing yet ..
     }
 
     holder_type *next, *prev;
+    weak_or_shared_collection<T, Shared> *collection;
 
   protected:
     virtual void reset_object ()
     {
       weak_or_shared_ptr<T, Shared>::reset_object ();
-      if (mp_collection) {
+      if (collection) {
         //  Caution: this will probably delete "this"!
-        mp_collection->remove_element (this);
+        collection->remove_element (this);
       }
     }
-
-  private:
-    weak_or_shared_collection<T, Shared> *mp_collection;
   };
 
   typedef weak_or_shared_collection_iterator<T, holder_type, Shared> iterator;
   typedef weak_or_shared_collection_iterator<const T, holder_type, Shared> const_iterator;
   typedef T value_type;
   typedef T &reference;
   typedef T *pointer;
@@ -221,24 +215,73 @@
    */
   weak_or_shared_collection ()
     : mp_first (0), mp_last (0), m_size (0)
   {
   }
 
   /**
+   *  @brief The copy constructor
+   */
+  weak_or_shared_collection (const weak_or_shared_collection<T, Shared> &other)
+    : mp_first (0), mp_last (0), m_size (0)
+  {
+    operator= (other);
+  }
+
+  /**
+   *  @brief The move constructor
+   */
+  weak_or_shared_collection (weak_or_shared_collection<T, Shared> &&other)
+    : mp_first (0), mp_last (0), m_size (0)
+  {
+    swap (other);
+  }
+
+  /**
    *  @brief Destructor
    */
   ~weak_or_shared_collection ()
   {
     while (! empty ()) {
       erase (mp_first);
     }
   }
 
   /**
+   *  @brief Assignment
+   */
+  weak_or_shared_collection &operator= (const weak_or_shared_collection<T, Shared> &other)
+  {
+    if (this != &other) {
+      clear ();
+      for (auto i = other.begin (); i != other.end (); ++i) {
+        push_back (const_cast<T *> (i.operator-> ()));
+      }
+    }
+    return *this;
+  }
+
+  /**
+   *  @brief Swap
+   */
+  void swap (weak_or_shared_collection<T, Shared> &other)
+  {
+    std::swap (mp_first, other.mp_first);
+    std::swap (mp_last, other.mp_last);
+    std::swap (m_size, other.m_size);
+
+    for (holder_type *h = mp_first; h; h = h->next) {
+      h->collection = this;
+    }
+    for (holder_type *h = other.mp_first; h; h = h->next) {
+      h->collection = &other;
+    }
+  }
+
+  /**
    *  @brief Returns a value indicating whether the collection is empty
    */
   bool empty () const
   {
     return mp_first == 0;
   }
```

### Comparing `klayout-0.29.0/src/tl/tl/tlOptional.cc` & `klayout-0.29.1/src/tl/tl/tlOptional.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlOptional.h` & `klayout-0.29.1/src/tl/tl/tlOptional.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlPixelBuffer.cc` & `klayout-0.29.1/src/tl/tl/tlPixelBuffer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlPixelBuffer.h` & `klayout-0.29.1/src/tl/tl/tlPixelBuffer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlProgress.cc` & `klayout-0.29.1/src/tl/tl/tlProgress.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlProgress.h` & `klayout-0.29.1/src/tl/tl/tlProgress.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlRecipe.cc` & `klayout-0.29.1/src/tl/tl/tlRecipe.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlRecipe.h` & `klayout-0.29.1/src/tl/tl/tlRecipe.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlResources.cc` & `klayout-0.29.1/src/tl/tl/tlResources.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlResources.h` & `klayout-0.29.1/src/tl/tl/tlResources.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlReuseVector.h` & `klayout-0.29.1/src/tl/tl/tlReuseVector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlSList.cc` & `klayout-0.29.1/src/tl/tl/tlSList.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlSList.h` & `klayout-0.29.1/src/tl/tl/tlSList.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlScriptError.cc` & `klayout-0.29.1/src/tl/tl/tlScriptError.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlScriptError.h` & `klayout-0.29.1/src/tl/tl/tlScriptError.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlSelect.h` & `klayout-0.29.1/src/tl/tl/tlSelect.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlSleep.cc` & `klayout-0.29.1/src/tl/tl/tlSleep.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlSleep.h` & `klayout-0.29.1/src/tl/tl/tlSleep.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStableVector.h` & `klayout-0.29.1/src/tl/tl/tlStableVector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStaticObjects.cc` & `klayout-0.29.1/src/tl/tl/tlStaticObjects.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStaticObjects.h` & `klayout-0.29.1/src/tl/tl/tlStaticObjects.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStream.cc` & `klayout-0.29.1/src/tl/tl/tlStream.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStream.h` & `klayout-0.29.1/src/tl/tl/tlStream.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlString.cc` & `klayout-0.29.1/src/tl/tl/tlString.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlString.h` & `klayout-0.29.1/src/tl/tl/tlString.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlStringEx.h` & `klayout-0.29.1/src/tl/tl/tlStringEx.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlThreadedWorkers.cc` & `klayout-0.29.1/src/tl/tl/tlThreadedWorkers.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlThreadedWorkers.h` & `klayout-0.29.1/src/tl/tl/tlThreadedWorkers.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlThreads.cc` & `klayout-0.29.1/src/tl/tl/tlThreads.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlThreads.h` & `klayout-0.29.1/src/tl/tl/tlThreads.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlTimer.cc` & `klayout-0.29.1/src/tl/tl/tlTimer.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlTimer.h` & `klayout-0.29.1/src/tl/tl/tlTimer.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlTypeTraits.h` & `klayout-0.29.1/src/tl/tl/tlTypeTraits.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUniqueId.cc` & `klayout-0.29.1/src/tl/tl/tlUniqueId.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUniqueId.h` & `klayout-0.29.1/src/tl/tl/tlUniqueId.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUniqueName.cc` & `klayout-0.29.1/src/tl/tl/tlUniqueName.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUniqueName.h` & `klayout-0.29.1/src/tl/tl/tlUniqueName.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUnitTest.cc` & `klayout-0.29.1/src/tl/tl/tlUnitTest.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUnitTest.h` & `klayout-0.29.1/src/tl/tl/tlUnitTest.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUri.cc` & `klayout-0.29.1/src/tl/tl/tlUri.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUri.h` & `klayout-0.29.1/src/tl/tl/tlUri.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlUtils.h` & `klayout-0.29.1/src/tl/tl/tlUtils.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlVariant.cc` & `klayout-0.29.1/src/tl/tl/tlVariant.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlVariant.h` & `klayout-0.29.1/src/tl/tl/tlVariant.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlVariantUserClasses.h` & `klayout-0.29.1/src/tl/tl/tlVariantUserClasses.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlVector.cc` & `klayout-0.29.1/src/tl/tl/tlVector.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlVector.h` & `klayout-0.29.1/src/tl/tl/tlVector.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlWebDAV.cc` & `klayout-0.29.1/src/tl/tl/tlWebDAV.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlWebDAV.h` & `klayout-0.29.1/src/tl/tl/tlWebDAV.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlXMLParser.cc` & `klayout-0.29.1/src/tl/tl/tlXMLParser.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlXMLParser.h` & `klayout-0.29.1/src/tl/tl/tlXMLParser.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlXMLWriter.cc` & `klayout-0.29.1/src/tl/tl/tlXMLWriter.cc`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/tlXMLWriter.h` & `klayout-0.29.1/src/tl/tl/tlXMLWriter.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/tl/tl/utf_casefolding.h` & `klayout-0.29.1/src/tl/tl/utf_casefolding.h`

 * *Files identical despite different names*

### Comparing `klayout-0.29.0/src/version/version.h` & `klayout-0.29.1/src/version/version.h`

 * *Files identical despite different names*

