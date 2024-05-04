# Comparing `tmp/starrail_damage_cal-1.5.5.tar.gz` & `tmp/starrail_damage_cal-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail_damage_cal-1.5.5.tar", last modified: Sun Apr 28 03:15:48 2024, max compression
+gzip compressed data, was "starrail_damage_cal-1.6.0.tar", last modified: Sat May  4 15:05:12 2024, max compression
```

## Comparing `starrail_damage_cal-1.5.5.tar` & `starrail_damage_cal-1.6.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1064 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/LICENSE
--rw-r--r--   0        0        0       20 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/README.md
--rw-r--r--   0        0        0     1246 2024-04-28 03:15:48.408581 starrail_damage_cal-1.5.5/pyproject.toml
--rw-r--r--   0        0        0       48 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/__init__.py
--rw-r--r--   0        0        0     4037 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/cal_damage.py
--rw-r--r--   0        0        0     4232 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Avatar.py
--rw-r--r--   0        0        0   159417 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/AvatarDamage/__init__.py
--rw-r--r--   0        0        0     5563 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/AvatarBase.py
--rw-r--r--   0        0        0     3199 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/RelicBase.py
--rw-r--r--   0        0        0     1171 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/SkillBase.py
--rw-r--r--   0        0        0     2567 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/WeaponBase.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/__init__.py
--rw-r--r--   0        0        0     2611 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/model.py
--rw-r--r--   0        0        0    68035 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Excel/SkillData.json
--rw-r--r--   0        0        0    20149 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Excel/weapon_effect.json
--rw-r--r--   0        0        0    35194 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Relic/Relic.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Relic/__init__.py
--rw-r--r--   0        0        0    14474 2024-04-28 03:15:33.272657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Role.py
--rw-r--r--   0        0        0    96034 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Weapon/Weapon.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Weapon/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/__init__.py
--rw-r--r--   0        0        0     2738 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/damage/utils.py
--rw-r--r--   0        0        0   341001 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/AvatarPromotionConfig.json
--rw-r--r--   0        0        0   485707 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/EquipmentPromotionConfig.json
--rw-r--r--   0        0        0    30312 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/RelicMainAffixConfig.json
--rw-r--r--   0        0        0    12017 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/RelicSubAffixConfig.json
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/__init__.py
--rw-r--r--   0        0        0    95747 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/light_cone_ranks.json
--rw-r--r--   0        0        0     9282 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/model.py
--rw-r--r--   0        0        0      624 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/excel/read_excel.py
--rw-r--r--   0        0        0     1241 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/exception.py
--rw-r--r--   0        0        0       64 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/logger.py
--rw-r--r--   0        0        0     4645 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/SR_MAP_PATH.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/__init__.py
--rw-r--r--   0        0        0    25390 2024-04-28 03:15:33.276657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/AvatarRelicScore.json
--rw-r--r--   0        0        0    47199 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json
--rw-r--r--   0        0        0     3220 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json
--rw-r--r--   0        0        0     3004 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     1503 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0    16428 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     2423 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/Property2Name.json
--rw-r--r--   0        0        0     2423 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7314 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json
--rw-r--r--   0        0        0     6896 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0     7714 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json
--rw-r--r--   0        0        0     4223 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json
--rw-r--r--   0        0        0     1184 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     1143 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json
--rw-r--r--   0        0        0     1196 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json
--rw-r--r--   0        0        0     1222 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0      867 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json
--rw-r--r--   0        0        0      867 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json
--rw-r--r--   0        0        0    23778 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json
--rw-r--r--   0        0        0     9285 2024-04-28 03:15:33.280657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/char_alias.json
--rw-r--r--   0        0        0  1445499 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json
--rw-r--r--   0        0        0    10716 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7739 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json
--rw-r--r--   0        0        0    10748 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json
--rw-r--r--   0        0        0     7535 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json
--rw-r--r--   0        0        0      701 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/model/RelicSetSkill.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/model/__init__.py
--rw-r--r--   0        0        0      491 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/map/name_covert.py
--rw-r--r--   0        0        0      202 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/mihomo/__init__.py
--rw-r--r--   0        0        0     2120 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/mihomo/models.py
--rw-r--r--   0        0        0     1335 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/mihomo/requests.py
--rw-r--r--   0        0        0     4472 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/mono/Character.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/mono/__init__.py
--rw-r--r--   0        0        0    11700 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/to_data.py
--rw-r--r--   0        0        0       28 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/starrail_damage_cal/version.py
--rw-r--r--   0        0        0        0 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/test/__init__.py
--rw-r--r--   0        0        0    12611 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/test/test.json
--rw-r--r--   0        0        0     1228 2024-04-28 03:15:33.284657 starrail_damage_cal-1.5.5/test/test_get_char.py
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 starrail_damage_cal-1.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/LICENSE
+-rw-r--r--   0        0        0       20 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/README.md
+-rw-r--r--   0        0        0     1246 2024-05-04 15:05:12.154282 starrail_damage_cal-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/__init__.py
+-rw-r--r--   0        0        0     4037 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/cal_damage.py
+-rw-r--r--   0        0        0     4232 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Avatar.py
+-rw-r--r--   0        0        0   159053 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/AvatarDamage/__init__.py
+-rw-r--r--   0        0        0     5563 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/AvatarBase.py
+-rw-r--r--   0        0        0     3199 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/RelicBase.py
+-rw-r--r--   0        0        0     1171 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/SkillBase.py
+-rw-r--r--   0        0        0     2567 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/WeaponBase.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/__init__.py
+-rw-r--r--   0        0        0     2611 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/model.py
+-rw-r--r--   0        0        0    68035 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Excel/SkillData.json
+-rw-r--r--   0        0        0    20149 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Excel/weapon_effect.json
+-rw-r--r--   0        0        0    35194 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Relic/Relic.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Relic/__init__.py
+-rw-r--r--   0        0        0    14474 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Role.py
+-rw-r--r--   0        0        0    96034 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Weapon/Weapon.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Weapon/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/__init__.py
+-rw-r--r--   0        0        0     2738 2024-05-04 15:04:57.322200 starrail_damage_cal-1.6.0/starrail_damage_cal/damage/utils.py
+-rw-r--r--   0        0        0   341001 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/AvatarPromotionConfig.json
+-rw-r--r--   0        0        0   485707 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/EquipmentPromotionConfig.json
+-rw-r--r--   0        0        0    30312 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/RelicMainAffixConfig.json
+-rw-r--r--   0        0        0    12017 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/RelicSubAffixConfig.json
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/__init__.py
+-rw-r--r--   0        0        0    95747 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/light_cone_ranks.json
+-rw-r--r--   0        0        0     9282 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/model.py
+-rw-r--r--   0        0        0      624 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/excel/read_excel.py
+-rw-r--r--   0        0        0     1241 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/exception.py
+-rw-r--r--   0        0        0       64 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/logger.py
+-rw-r--r--   0        0        0     4645 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/SR_MAP_PATH.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/__init__.py
+-rw-r--r--   0        0        0    25390 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/AvatarRelicScore.json
+-rw-r--r--   0        0        0    47199 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json
+-rw-r--r--   0        0        0     3220 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json
+-rw-r--r--   0        0        0     3004 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1503 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0    16428 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     2423 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/Property2Name.json
+-rw-r--r--   0        0        0     2423 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7314 2024-05-04 15:04:57.326200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json
+-rw-r--r--   0        0        0     6896 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7714 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json
+-rw-r--r--   0        0        0     4223 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1184 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1143 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1196 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json
+-rw-r--r--   0        0        0     1222 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0      867 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json
+-rw-r--r--   0        0        0      867 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json
+-rw-r--r--   0        0        0    23778 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json
+-rw-r--r--   0        0        0     9285 2024-05-04 15:04:57.330200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/char_alias.json
+-rw-r--r--   0        0        0  1445499 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json
+-rw-r--r--   0        0        0    10716 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7739 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json
+-rw-r--r--   0        0        0    10748 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json
+-rw-r--r--   0        0        0     7535 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json
+-rw-r--r--   0        0        0      701 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/model/RelicSetSkill.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/model/__init__.py
+-rw-r--r--   0        0        0      491 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/map/name_covert.py
+-rw-r--r--   0        0        0      202 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/mihomo/__init__.py
+-rw-r--r--   0        0        0     2120 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/mihomo/models.py
+-rw-r--r--   0        0        0     1335 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/mihomo/requests.py
+-rw-r--r--   0        0        0     4472 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/mono/Character.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/mono/__init__.py
+-rw-r--r--   0        0        0    11700 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/to_data.py
+-rw-r--r--   0        0        0       28 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/starrail_damage_cal/version.py
+-rw-r--r--   0        0        0        0 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/test/__init__.py
+-rw-r--r--   0        0        0    12611 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/test/test.json
+-rw-r--r--   0        0        0     1228 2024-05-04 15:04:57.334200 starrail_damage_cal-1.6.0/test/test_get_char.py
+-rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 starrail_damage_cal-1.6.0/PKG-INFO
```

### Comparing `starrail_damage_cal-1.5.5/LICENSE` & `starrail_damage_cal-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/pyproject.toml` & `starrail_damage_cal-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "starrail_damage_cal"
-version = "1.5.5"
+version = "1.6.0"
 description = "For StarRail Role Damage Cal"
 authors = [
     { name = "qwerdvd", email = "105906879+qwerdvd@users.noreply.github.com" },
 ]
 dependencies = [
     "msgspec>=0.18.6",
     "httpx>=0.27.0",
```

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/cal_damage.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/cal_damage.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Avatar.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Avatar.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/AvatarDamage/AvatarDamage.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,16 +94,15 @@
         )
         skill_info_list.append({"name": "终结技", "damagelist": damagelist3})
 
         # 银狼降防终结技伤害
         skill_multiplier = self.Skill_num("Ultra", "Ultra")
         add_attr_bonus = copy.deepcopy(attribute_bonus)
         add_attr_bonus["ignore_defence"] = 0.45 + add_attr_bonus.get(
-            "ignore_defence",
-            0,
+            "ignore_defence", 0
         )
         damagelist4 = await calculate_damage(
             base_attr,
             add_attr_bonus,
             "Ultra",
             "Ultra",
             self.avatar_element,
@@ -507,16 +506,15 @@
             add_attr_bonus = copy.deepcopy(attribute_bonus)
             damage_buff = min(max_buff, 10)
             add_attr_bonus["AllDamageAddedRatio"] = (
                 damage_buff * injury_add + add_attr_bonus.get("AllDamageAddedRatio", 0)
             )
             critical_buff = 4 * critical_damage_add
             add_attr_bonus["CriticalDamageBase"] = critical_buff + add_attr_bonus.get(
-                "CriticalDamageBase",
-                0,
+                "CriticalDamageBase", 0
             )
             damage1, damage2, damage3 = await calculate_damage(
                 base_attr,
                 add_attr_bonus,
                 "Ultra",
                 "Ultra",
                 self.avatar_element,
@@ -564,16 +562,15 @@
     ):
         talent_cc_add = self.Skill_num("Talent", "Talent")
         attribute_bonus["CriticalChanceBase"] = (
             talent_cc_add * 10 + attribute_bonus.get("CriticalChanceBase", 0)
         )
         if self.avatar_rank >= 4:
             attribute_bonus["CriticalDamageBase"] = 0.08 + attribute_bonus.get(
-                "CriticalDamageBase",
-                0,
+                "CriticalDamageBase", 0
             )
             attribute_bonus["CriticalChanceBase"] = (
                 talent_cc_add * 2 + attribute_bonus.get("CriticalChanceBase", 0)
             )
 
         skill_info_list = []
         # 计算普攻伤害
@@ -1084,18 +1081,17 @@
             self.avatar_level,
             1,
         )
         damagelist7[0] += damagelist6[0]
         damagelist7[1] += damagelist6[1]
         damagelist7[2] += damagelist6[2]
         if self.avatar_rank >= 6:
-            hp = (
-                base_attr["hp"] * (1 + attribute_bonus["HPAddedRatio"])
-                + attribute_bonus["HPDelta"]
-            )
+            hp = base_attr["hp"] * (
+                1 + attribute_bonus.get("HPAddedRatio", 0)
+            ) + attribute_bonus.get("HPDelta", 0)
             damage_add = hp * 0.5
             damagelist7[0] += damage_add
             damagelist7[1] += damage_add
             damagelist7[2] += damage_add
         skill_info_list.append({"name": "追加攻击", "damagelist": damagelist7})
 
         return skill_info_list
@@ -1159,15 +1155,14 @@
             "Ultra",
             "Ultra",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
             1,
         )
-        damagelist2[2] += damage2
         skill_info_list.append({"name": "终结技", "damagelist": damagelist2})
 
         # 计算终结技治疗
         damagelist3 = await calculate_heal(
             base_attr,
             attribute_bonus,
             "Ultra",
@@ -2033,18 +2028,17 @@
         attribute_bonus: Dict[str, float],
     ):
         # 计算战技生命上限
         skill_multiplier = self.Skill_num("BPSkill", "BPSkill_HP")
         skill_num = self.Skill_num("BPSkill", "BPSkill_HP_G")
         if self.avatar_rank >= 6:
             skill_multiplier += 0.06
-        hp = (
-            base_attr["hp"] * (1 + attribute_bonus["HPAddedRatio"])
-            + attribute_bonus["HPDelta"]
-        )
+        hp = base_attr["hp"] * (
+            1 + attribute_bonus.get("HPAddedRatio", 0)
+        ) + attribute_bonus.get("HPDelta", 0)
         hp_add = hp * skill_multiplier + skill_num
         attribute_bonus["HPDelta"] = attribute_bonus.get("HPDelta", 0) + hp_add
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal_HP")
         damagelist1 = await calculate_damage(
@@ -2338,21 +2332,22 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 终结技增加伤害
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
-            "AttackAddedRatio",
-            0,
+            "AttackAddedRatio", 0
         ) + self.Skill_num("Ultra", "Ultra_A")
+
         add_critical_damage_base = (
             attribute_bonus.get("CriticalDamageBase", 0)
             * self.Skill_num("Ultra", "Ultra")
         ) + self.Skill_num("Ultra", "Ultra_G")
+
         attribute_bonus["CriticalDamageBase"] = (
             attribute_bonus.get("CriticalDamageBase", 0) + add_critical_damage_base
         )
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
@@ -2401,24 +2396,21 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 终结技增加伤害
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
-            "AttackAddedRatio",
-            0,
+            "AttackAddedRatio", 0
         ) + self.Skill_num("BPSkill", "BPSkill")
         attribute_bonus["CriticalChanceBase"] = attribute_bonus.get(
-            "CriticalChanceBase",
-            0,
+            "CriticalChanceBase", 0
         ) + self.Skill_num("Ultra", "Ultra_CC")
         attribute_bonus["CriticalDamageBase"] = attribute_bonus.get(
-            "CriticalDamageBase",
-            0,
+            "CriticalDamageBase", 0
         ) + self.Skill_num("Ultra", "Ultra_CD")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -2587,16 +2579,15 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算终结技提供的易伤加成
         attribute_bonus["DmgRatio"] = attribute_bonus.get(
-            "DmgRatio",
-            0,
+            "DmgRatio", 0
         ) + self.Skill_num("Ultra", "Ultra_d")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -2704,16 +2695,15 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算穿透加成
         attribute_bonus["WindResistancePenetration"] = attribute_bonus.get(
-            "WindResistancePenetration",
-            0,
+            "WindResistancePenetration", 0
         ) + self.Skill_num("Talent", "Talent")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -2783,16 +2773,15 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算天赋伤害加成
         attribute_bonus["AllDamageAddedRatio"] = attribute_bonus.get(
-            "AllDamageAddedRatio",
-            0,
+            "AllDamageAddedRatio", 0
         ) + self.Skill_num("Talent", "Talent")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -2860,16 +2849,15 @@
     ):
         # 计算天赋加成
         attribute_bonus["AttackAddedRatio"] = (
             attribute_bonus.get("AttackAddedRatio", 0)
             + self.Skill_num("Talent", "Talent") * 5
         )
         attribute_bonus["SpeedDelta"] = attribute_bonus.get(
-            "SpeedDelta",
-            0,
+            "SpeedDelta", 0
         ) + self.Skill_num("Ultra", "Ultra")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -3113,16 +3101,15 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算终结技降防
         attribute_bonus["ignore_defence"] = attribute_bonus.get(
-            "ignore_defence",
-            0,
+            "ignore_defence", 0
         ) + self.Skill_num("Ultra", "Ultra_d")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -3199,16 +3186,15 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算终结技持续伤害加成
         attribute_bonus["DOTDmgAdd"] = attribute_bonus.get(
-            "DOTDmgAdd",
-            0,
+            "DOTDmgAdd", 0
         ) + self.Skill_num("Ultra", "Ultra_d")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -3771,23 +3757,21 @@
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 计算天赋易伤加成
         attribute_bonus["DmgRatio"] = attribute_bonus.get(
-            "DmgRatio",
-            0,
+            "DmgRatio", 0
         ) + self.Skill_num("Talent", "Talent")
         if self.avatar_rank >= 6:
             attribute_bonus["DmgRatio"] = attribute_bonus.get("DmgRatio", 0) + 0.1
 
         attribute_bonus["AttackAddedRatio"] = attribute_bonus.get(
-            "AttackAddedRatio",
-            0,
+            "AttackAddedRatio", 0
         ) + self.Skill_num("Ultra", "Ultra_A")
 
         skill_info_list = []
         # 计算普攻伤害
         skill_multiplier = self.Skill_num("Normal", "Normal")
         damagelist1 = await calculate_damage(
             base_attr,
@@ -4485,18 +4469,17 @@
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 天赋增加暴击
-        defence = (
-            base_attr["defence"] * (1 + attribute_bonus["DefenceAddedRatio"])
-            + attribute_bonus["DefenceDelta"]
-        )
+        defence = base_attr["defence"] * (
+            1 + attribute_bonus.get("DefenceAddedRatio", 0)
+        ) + attribute_bonus.get("DefenceDelta", 0)
         if defence > 1600:
             adddefrnce = defence - 1600
             Critical_Chance_Base = (defence / 100) * 0.02
             Critical_Chance_Base = min(Critical_Chance_Base, 0.48)
             attribute_bonus["CriticalChanceBase"] = (
                 attribute_bonus.get("CriticalChanceBase", 0) + Critical_Chance_Base
             )
@@ -4681,21 +4664,19 @@
         self.eidolons()
         self.extra_ability()
 
     def Technique(self):
         pass
 
     def eidolons(self):
-        if self.avatar_rank >= 2:
-            self.eidolon_attribute["CriticalDamageBase"] = 0.2
-        if self.avatar_rank >= 6:
-            self.eidolon_attribute["AllDamageResistancePenetration"] = 0.2
+        if self.avatar_rank >= 1:
+            self.eidolon_attribute["AllDamageResistancePenetration"] = 0.24
 
     def extra_ability(self):
-        pass
+        self.extra_ability_attribute["Talent_CriticalDamageBase"] = 0.25
 
     async def getdamage(
         self,
         base_attr: Dict[str, float],
         attribute_bonus: Dict[str, float],
     ):
         # 战技伤害加成
@@ -4743,28 +4724,26 @@
         skill_info_list.append({"name": "终结技攻击提高", "damagelist": damagelist2})
 
         # 计算追击伤害
         skill_multiplier = self.Skill_num("Ultra", "Ultra")
         add_attr_bonus = copy.deepcopy(attribute_bonus)
         add_attr_bonus["CriticalDamageBase"] = 1
         add_attr_bonus["CriticalChanceBase"] = 0.95
-        if self.avatar_rank >= 1:
-            skill_multiplier = skill_multiplier + 0.72
         if self.avatar_rank >= 6:
-            add_attr_bonus["CriticalDamageBase"] = 3
+            add_attr_bonus["CriticalDamageBase"] = 5.5
         damagelist4 = await calculate_damage(
             base_attr,
             add_attr_bonus,
-            "Talent",
-            "Talent",
+            "fujia",
+            "fujia",
             self.avatar_element,
             skill_multiplier,
             self.avatar_level,
         )
-        skill_info_list.append({"name": "【协奏】追加伤害", "damagelist": damagelist4})
+        skill_info_list.append({"name": "【协奏】附加伤害", "damagelist": damagelist4})
 
         return skill_info_list
 
 
 class AvatarDamage:
     @classmethod
     def create(cls, char: DamageInstanceAvatar, skills: List[DamageInstanceSkill]):
```

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/AvatarBase.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/AvatarBase.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/RelicBase.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/RelicBase.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/SkillBase.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/SkillBase.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/WeaponBase.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/WeaponBase.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Base/model.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Base/model.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Excel/SkillData.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Excel/SkillData.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Excel/weapon_effect.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Excel/weapon_effect.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Relic/Relic.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Relic/Relic.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Role.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Role.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/Weapon/Weapon.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/Weapon/Weapon.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/damage/utils.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/damage/utils.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/AvatarPromotionConfig.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/AvatarPromotionConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/EquipmentPromotionConfig.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/EquipmentPromotionConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/RelicMainAffixConfig.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/RelicMainAffixConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/RelicSubAffixConfig.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/RelicSubAffixConfig.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/light_cone_ranks.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/light_cone_ranks.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/model.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/model.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/excel/read_excel.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/excel/read_excel.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/exception.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/exception.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/SR_MAP_PATH.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/SR_MAP_PATH.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/AvatarRelicScore.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/AvatarRelicScore.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2AbilityProperty_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2EnName_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/EquipmentID2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/ItemId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/Property2Name.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/Property2Name.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/Property2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2MainAffixGroup_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicId2SetId_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/RelicSetSkill_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/SetId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2DamageType_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2EnName_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Rarity_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarId2Star_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/avatarRankSkillUp_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/char_alias.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/char_alias.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/characterSkillTree_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/rankId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2AttackType_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2Name_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/data/skillId2Type_mapping_2.1.0.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/map/model/RelicSetSkill.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/map/model/RelicSetSkill.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/mihomo/models.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/mihomo/models.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/mihomo/requests.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/mihomo/requests.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/mono/Character.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/mono/Character.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/starrail_damage_cal/to_data.py` & `starrail_damage_cal-1.6.0/starrail_damage_cal/to_data.py`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/test/test.json` & `starrail_damage_cal-1.6.0/test/test.json`

 * *Files identical despite different names*

### Comparing `starrail_damage_cal-1.5.5/test/test_get_char.py` & `starrail_damage_cal-1.6.0/test/test_get_char.py`

 * *Files identical despite different names*

