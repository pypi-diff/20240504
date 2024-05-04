# Comparing `tmp/jy_lib-0.7.2.tar.gz` & `tmp/jy_lib-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.7.2.tar` & `jy_lib-0.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2083 2024-01-01 02:29:02.554641 jy_lib-0.7.2/.gitignore
--rw-r--r--   0        0        0      285 2024-01-01 02:29:02.554755 jy_lib-0.7.2/.pypirc
--rw-r--r--   0        0        0     1073 2024-01-01 02:29:02.555085 jy_lib-0.7.2/LICENSE
--rw-r--r--   0        0        0      573 2024-04-21 14:22:14.414420 jy_lib-0.7.2/Pipfile
--rw-r--r--   0        0        0    40838 2024-01-01 02:29:02.555480 jy_lib-0.7.2/Pipfile.lock
--rw-r--r--   0        0        0       10 2024-01-01 02:29:02.555572 jy_lib-0.7.2/README.md
--rw-r--r--   0        0        0      469 2024-01-01 02:29:02.555665 jy_lib-0.7.2/README_Project.md
--rw-r--r--   0        0        0      518 2024-04-29 13:37:38.658367 jy_lib-0.7.2/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2024-01-01 02:29:02.555927 jy_lib-0.7.2/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2024-01-01 02:29:02.556043 jy_lib-0.7.2/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2024-01-01 02:29:02.556135 jy_lib-0.7.2/jy_lib/base.py
--rw-r--r--   0        0        0    11460 2024-04-26 13:44:43.888654 jy_lib-0.7.2/jy_lib/cache.py
--rw-r--r--   0        0        0    11967 2024-04-29 13:37:23.357311 jy_lib-0.7.2/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-04-27 14:14:12.824508 jy_lib-0.7.2/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2024-01-01 02:29:02.556414 jy_lib-0.7.2/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2024-01-01 02:29:02.556554 jy_lib-0.7.2/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-04-21 14:22:14.416027 jy_lib-0.7.2/jy_lib/date.py
--rw-r--r--   0        0        0      931 2024-01-01 02:29:02.556726 jy_lib-0.7.2/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-04-26 13:44:43.889079 jy_lib-0.7.2/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-04-21 14:22:14.416177 jy_lib-0.7.2/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2024-01-01 02:29:02.556936 jy_lib-0.7.2/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-04-21 14:22:14.416596 jy_lib-0.7.2/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2024-01-01 02:29:02.557127 jy_lib-0.7.2/jy_lib/nav.py
--rw-r--r--   0        0        0     2194 2024-04-29 13:37:23.357463 jy_lib-0.7.2/jy_lib/reader.py
--rw-r--r--   0        0        0    18478 2024-04-21 14:22:14.416811 jy_lib-0.7.2/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22173 2024-04-26 13:44:43.889377 jy_lib-0.7.2/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-04-21 14:22:14.417332 jy_lib-0.7.2/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2024-01-01 02:29:02.557631 jy_lib-0.7.2/jy_lib/time.py
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557712 jy_lib-0.7.2/publish-jypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557791 jy_lib-0.7.2/publish-pypi.sh
--rw-r--r--   0        0        0       67 2024-01-01 02:29:02.557873 jy_lib-0.7.2/publish-test.sh
--rw-r--r--   0        0        0      639 2024-04-21 14:22:14.417488 jy_lib-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      117 2024-04-21 14:22:14.417721 jy_lib-0.7.2/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     2083 2024-05-04 10:16:37.911987 jy_lib-0.7.3/.gitignore
+-rw-r--r--   0        0        0      285 2024-05-04 10:16:37.912391 jy_lib-0.7.3/.pypirc
+-rw-r--r--   0        0        0     1073 2024-05-04 10:16:37.912678 jy_lib-0.7.3/LICENSE
+-rw-r--r--   0        0        0      573 2024-05-04 10:16:37.912981 jy_lib-0.7.3/Pipfile
+-rw-r--r--   0        0        0    40838 2024-05-04 10:16:37.913598 jy_lib-0.7.3/Pipfile.lock
+-rw-r--r--   0        0        0       10 2024-05-04 10:16:37.914070 jy_lib-0.7.3/README.md
+-rw-r--r--   0        0        0      469 2024-05-04 10:16:37.914438 jy_lib-0.7.3/README_Project.md
+-rw-r--r--   0        0        0      518 2024-05-04 10:20:58.713262 jy_lib-0.7.3/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2024-05-04 10:16:37.915485 jy_lib-0.7.3/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2024-05-04 10:16:37.915923 jy_lib-0.7.3/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2024-05-04 10:16:37.916235 jy_lib-0.7.3/jy_lib/base.py
+-rw-r--r--   0        0        0    14155 2024-05-04 10:16:37.916568 jy_lib-0.7.3/jy_lib/cache.py
+-rw-r--r--   0        0        0    11966 2024-05-04 10:16:37.916925 jy_lib-0.7.3/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-05-04 10:16:37.917240 jy_lib-0.7.3/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2024-05-04 10:16:37.917634 jy_lib-0.7.3/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2024-05-04 10:16:37.918037 jy_lib-0.7.3/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-05-04 10:16:37.918334 jy_lib-0.7.3/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2024-05-04 10:16:37.918666 jy_lib-0.7.3/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5916 2024-05-04 10:16:37.918991 jy_lib-0.7.3/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-05-04 10:16:37.919292 jy_lib-0.7.3/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2024-05-04 10:16:37.919587 jy_lib-0.7.3/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-05-04 10:16:37.919884 jy_lib-0.7.3/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2024-05-04 10:16:37.920296 jy_lib-0.7.3/jy_lib/nav.py
+-rw-r--r--   0        0        0     2194 2024-05-04 10:16:37.920783 jy_lib-0.7.3/jy_lib/reader.py
+-rw-r--r--   0        0        0    18478 2024-05-04 10:16:37.921224 jy_lib-0.7.3/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22173 2024-05-04 10:16:37.921846 jy_lib-0.7.3/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-05-04 10:16:37.922441 jy_lib-0.7.3/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2024-05-04 10:16:37.922948 jy_lib-0.7.3/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923293 jy_lib-0.7.3/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923609 jy_lib-0.7.3/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923903 jy_lib-0.7.3/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-05-04 10:16:37.924216 jy_lib-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-05-04 10:16:37.924494 jy_lib-0.7.3/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.3/PKG-INFO
```

### Comparing `jy_lib-0.7.2/.gitignore` & `jy_lib-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/LICENSE` & `jy_lib-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/Pipfile` & `jy_lib-0.7.3/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/Pipfile.lock` & `jy_lib-0.7.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/__init__.py` & `jy_lib-0.7.3/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
```

### Comparing `jy_lib-0.7.2/jy_lib/auth_client.py` & `jy_lib-0.7.3/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/bank.py` & `jy_lib-0.7.3/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/base.py` & `jy_lib-0.7.3/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/cache.py` & `jy_lib-0.7.3/jy_lib/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import inspect
 import lz4.frame
 import math
 import os
 import pickle
 import re
 import sqlite3
+import threading
 import time
 from typing import Any, Set, List, Tuple, Dict
 
 
 class Cache:
     """持久化TTL缓存"""
 
@@ -20,50 +21,54 @@
         caller_frame = current_frame.f_back
         caller_file = caller_frame.f_code.co_filename
         if not path:
             path: str = f'_{os.path.splitext(os.path.basename(caller_file))[0]}.db3'
         self.path: str = os.path.join(os.path.dirname(caller_file), path)
         self.default_dataset: str = 'DEFAULT'
         self.compress_min_size: int = max(64, len(lz4.frame.compress(b'\x00')))
-        self.conn = sqlite3.connect(self.path)
+        self.conn = sqlite3.connect(self.path, check_same_thread=False)
+        self.lock = threading.RLock()
         # self.conn.execute('PRAGMA auto_vacuum = FULL')
         self.datasets: Set[str] = self.get_tables()
         self.upgrade_tables()
 
     def get_tables(self) -> Set[str]:
         """获取所有数据集"""
-        cursor = self.conn.cursor()
-        r = cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
-        return {row[0] for row in r.fetchall()}
+        with self.lock:
+            cursor = self.conn.cursor()
+            r = cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
+            return {row[0] for row in r.fetchall()}
 
     def upgrade_tables(self):
         """升级表到最新版本"""
-        updated: bool = False
-        for dataset in self.datasets:
-            cursor = self.conn.cursor()
-            r = cursor.execute(f"PRAGMA table_info({dataset});")
-            cols: List[str] = [x[1] for x in r.fetchall()]
-            if 'encoding' not in cols:
-                self.conn.execute(f'ALTER TABLE `{dataset}` ADD COLUMN `encoding` INTEGER;')
-                self.conn.execute(f'UPDATE `{dataset}` SET `encoding` = 5;')
-                updated |= True
-        if updated:
-            self.conn.commit()
+        with self.lock:
+            updated: bool = False
+            for dataset in self.datasets:
+                cursor = self.conn.cursor()
+                r = cursor.execute(f"PRAGMA table_info({dataset});")
+                cols: List[str] = [x[1] for x in r.fetchall()]
+                if 'encoding' not in cols:
+                    self.conn.execute(f'ALTER TABLE `{dataset}` ADD COLUMN `encoding` INTEGER;')
+                    self.conn.execute(f'UPDATE `{dataset}` SET `encoding` = 5;')
+                    updated |= True
+            if updated:
+                self.conn.commit()
 
     def create_table(self, dataset: str) -> None:
         """创建数据集"""
-        assert not re.findall(r'\s', dataset)
-        self.conn.execute(f"""CREATE TABLE IF NOT EXISTS `{dataset}` (
-            `key` TEXT PRIMARY KEY NOT NULL,
-            `value` BLOB,
-            `encoding` INTEGER NOT NULL,
-            `expired_at` REAL NOT NULL
-        )""")
-        self.conn.execute(f"""CREATE INDEX IF NOT EXISTS expired_at ON `{dataset}` (`expired_at`)""")
-        self.conn.commit()
+        with self.lock:
+            assert not re.findall(r'\s', dataset)
+            self.conn.execute(f"""CREATE TABLE IF NOT EXISTS `{dataset}` (
+                `key` TEXT PRIMARY KEY NOT NULL,
+                `value` BLOB,
+                `encoding` INTEGER NOT NULL,
+                `expired_at` REAL NOT NULL
+            )""")
+            self.conn.execute(f"""CREATE INDEX IF NOT EXISTS expired_at ON `{dataset}` (`expired_at`)""")
+            self.conn.commit()
 
     def encode_value(self, value: Any) -> Tuple[Any, int]:
         """数据编码"""
         if value is None:
             return value, 0     # 原始数据
         elif isinstance(value, bool):
             return value, 64
@@ -125,157 +130,204 @@
             case 68:
                 return int(value)
             case _:
                 raise ValueError(encoding)
 
     def set(self, dataset: str = None, key: str = '', value: Any = None, expire: float = math.inf) -> None:
         """设置键值"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        assert isinstance(key, str), 'key必须是字符串'
-        assert key, 'key不能为空'
-        if dataset not in self.datasets:
-            self.create_table(dataset=dataset)
-            self.datasets.clear()
-            self.datasets.update(self.get_tables())
-        payload, encoding = self.encode_value(value=value)
-        sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
-        self.conn.execute(sql, (key, payload, encoding, time.time() + expire))
-        self.conn.commit()
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            assert isinstance(key, str), 'key必须是字符串'
+            assert key, 'key不能为空'
+            if dataset not in self.datasets:
+                self.create_table(dataset=dataset)
+                self.datasets.clear()
+                self.datasets.update(self.get_tables())
+            payload, encoding = self.encode_value(value=value)
+            sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
+            self.conn.execute(sql, (key, payload, encoding, time.time() + expire))
+            self.conn.commit()
+
+    def rename(self, dataset: str = None, key: str = '', new_key: str = '') -> None:
+        """重命名键值"""
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            assert isinstance(key, str), 'key必须是字符串'
+            assert key, 'key不能为空'
+            assert isinstance(new_key, str), 'new_key必须是字符串'
+            assert new_key, 'new_key不能为空'
+            if key == new_key:
+                return
+            if dataset not in self.datasets:
+                self.create_table(dataset=dataset)
+                self.datasets.clear()
+                self.datasets.update(self.get_tables())
+            sql: str = f"""UPDATE `{dataset}` SET `key` = ? WHERE `key` = ?"""
+            self.conn.execute(sql, (new_key, key))
+            self.conn.commit()
 
     def update(self, dataset: str = None, items: Dict[str, Any] = None, expire: float = math.inf) -> None:
         """批量设置键值"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        assert isinstance(items, dict), 'items必须是字典'
-        if not items:
-            return
-        for key in items.keys():
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            assert isinstance(items, dict), 'items必须是字典'
+            if not items:
+                return
+            for key in items.keys():
+                assert isinstance(key, str), 'key必须是字符串'
+                assert key, 'key不能为空'
+            if dataset not in self.datasets:
+                self.create_table(dataset=dataset)
+                self.datasets.clear()
+                self.datasets.update(self.get_tables())
+            ps: List[Tuple] = []
+            now = time.time()
+            for key, value in items.items():
+                payload, encoding = self.encode_value(value=value)
+                ps.append((key, payload, encoding, now + expire))
+            sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
+            self.conn.executemany(sql, ps)
+            self.conn.commit()
+
+    def add(self, dataset: str = None, key: str = '', value: Any = None, expire: float = math.inf) -> None:
+        """添加值到集合中"""
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
             assert isinstance(key, str), 'key必须是字符串'
             assert key, 'key不能为空'
-        if dataset not in self.datasets:
-            self.create_table(dataset=dataset)
-            self.datasets.clear()
-            self.datasets.update(self.get_tables())
-        ps: List[Tuple] = []
-        now = time.time()
-        for key, value in items.items():
-            payload, encoding = self.encode_value(value=value)
-            ps.append((key, payload, encoding, now + expire))
-        sql: str = f"""REPLACE INTO `{dataset}` (`key`, `value`, `encoding`, `expired_at`) VALUES(?,?,?,?)"""
-        self.conn.executemany(sql, ps)
-        self.conn.commit()
+            rs: Set = self.get(dataset=dataset, key=key) or set()
+            try:
+                hash(value)
+                rs.add(value)
+            except TypeError:
+                rs.update(value)
+            self.set(dataset=dataset, key=key, value=rs, expire=expire)
 
     def delete(self, dataset: str = None, key: str | List[str] = None) -> None:
         """删除键值对"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        assert key, 'key不能为空'
-        if isinstance(key, str):
-            key: List[str] = [key]
-        elif isinstance(key, list):
-            for k in key:
-                assert isinstance(k, str), 'key列表元素必须是字符串'
-                assert k, 'key列表元素不能为空'
-        else:
-            raise ValueError('key必须是字符串或字符串列表')
-        if dataset in self.datasets:
-            placeholders: str = ', '.join(['?'] * len(key))
-            sql: str = f"""DELETE FROM `{dataset}` WHERE `key` IN ({placeholders})"""
-            self.conn.execute(sql, key)
-            self.conn.commit()
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            assert key, 'key不能为空'
+            if isinstance(key, str):
+                key: List[str] = [key]
+            elif isinstance(key, list):
+                for k in key:
+                    assert isinstance(k, str), 'key列表元素必须是字符串'
+                    assert k, 'key列表元素不能为空'
+            else:
+                raise ValueError('key必须是字符串或字符串列表')
+            if dataset in self.datasets:
+                placeholders: str = ', '.join(['?'] * len(key))
+                sql: str = f"""DELETE FROM `{dataset}` WHERE `key` IN ({placeholders})"""
+                self.conn.execute(sql, key)
+                self.conn.commit()
 
     def get(self, dataset: str = None, key: str = '') -> Any | None:
         """获取键值"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        assert isinstance(key, str), 'key必须是字符串'
-        assert key, 'key不能为空'
-        if dataset in self.datasets:
-            cursor = self.conn.cursor()
-            sql: str = f"""SELECT `value`, `encoding`, `expired_at` FROM `{dataset}` WHERE `key`=?"""
-            r = cursor.execute(sql, (key, ))
-            r = r.fetchone()
-            if r is None:
-                return r
-            else:
-                value, encoding, expired_at = r
-                if expired_at > time.time():
-                    return self.decode_value(value=value, encoding=encoding)
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            assert isinstance(key, str), 'key必须是字符串'
+            assert key, 'key不能为空'
+            if dataset in self.datasets:
+                cursor = self.conn.cursor()
+                sql: str = f"""SELECT `value`, `encoding`, `expired_at` FROM `{dataset}` WHERE `key`=?"""
+                r = cursor.execute(sql, (key, ))
+                r = r.fetchone()
+                if r is None:
+                    return r
                 else:
-                    self.delete(dataset=dataset, key=key)
-                    return None
+                    value, encoding, expired_at = r
+                    if expired_at > time.time():
+                        return self.decode_value(value=value, encoding=encoding)
+                    else:
+                        self.delete(dataset=dataset, key=key)
+                        return None
 
     def keys(self, dataset: str = None) -> List[str] | None:
         """列出所有键名"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        if dataset in self.datasets:
-            cursor = self.conn.cursor()
-            now: float = time.time()
-            sql: str = f"""SELECT `key`, `expired_at` FROM `{dataset}`"""
-            r = cursor.execute(sql)
-            result: List[str] = []
-            delete_keys: List[str] = []
-            for key, expired_at in r.fetchall():
-                if expired_at > now:
-                    result.append(key)
-                else:
-                    delete_keys.append(key)
-            if delete_keys:
-                self.delete(dataset=dataset, key=delete_keys)
-            return result
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            if dataset in self.datasets:
+                cursor = self.conn.cursor()
+                now: float = time.time()
+                sql: str = f"""SELECT `key`, `expired_at` FROM `{dataset}`"""
+                r = cursor.execute(sql)
+                result: List[str] = []
+                delete_keys: List[str] = []
+                for key, expired_at in r.fetchall():
+                    if expired_at > now:
+                        result.append(key)
+                    else:
+                        delete_keys.append(key)
+                if delete_keys:
+                    self.delete(dataset=dataset, key=delete_keys)
+                return result
 
     def items(self, dataset: str = None) -> Dict:
         """列出所有键值对"""
-        if not dataset:
-            dataset = self.default_dataset
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        if dataset in self.datasets:
-            cursor = self.conn.cursor()
-            now: float = time.time()
-            sql: str = f"""SELECT `key`, `value`, `encoding`, `expired_at` FROM `{dataset}`"""
-            r = cursor.execute(sql)
-            result: Dict[str, Any] = {}
-            delete_keys: List[str] = []
-            for key, value, encoding, expired_at in r.fetchall():
-                print([key, value, encoding, expired_at])
-                if expired_at > now:
-                    result[key] = self.decode_value(value=value, encoding=encoding)
-                else:
-                    delete_keys.append(key)
-            if delete_keys:
-                self.delete(dataset=dataset, key=delete_keys)
-            return result
+        with self.lock:
+            if not dataset:
+                dataset = self.default_dataset
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            if dataset in self.datasets:
+                cursor = self.conn.cursor()
+                now: float = time.time()
+                sql: str = f"""SELECT `key`, `value`, `encoding`, `expired_at` FROM `{dataset}`"""
+                r = cursor.execute(sql)
+                result: Dict[str, Any] = {}
+                delete_keys: List[str] = []
+                for key, value, encoding, expired_at in r.fetchall():
+                    print([key, value, encoding, expired_at])
+                    if expired_at > now:
+                        result[key] = self.decode_value(value=value, encoding=encoding)
+                    else:
+                        delete_keys.append(key)
+                if delete_keys:
+                    self.delete(dataset=dataset, key=delete_keys)
+                return result
 
     def drop_table(self, dataset: str):
         """删除数据集"""
-        assert isinstance(dataset, str), 'dataset必须是字符串'
-        assert dataset, 'dataset不能为空'
-        if dataset in self.datasets:
-            sql: str = f"""DROP TABLE IF EXISTS `{dataset}`"""
-            self.conn.execute(sql)
-            self.conn.commit()
-            self.datasets.discard(dataset)
+        with self.lock:
+            assert isinstance(dataset, str), 'dataset必须是字符串'
+            assert dataset, 'dataset不能为空'
+            if dataset in self.datasets:
+                sql: str = f"""DROP TABLE IF EXISTS `{dataset}`"""
+                self.conn.execute(sql)
+                self.conn.commit()
+                self.datasets.discard(dataset)
 
     def vacuum(self, force: bool = True):
-        key_vacuum_at: str = '__VACUUM__'
-        vacuum_at: int | None = self.get(key=key_vacuum_at)
-        if force or not vacuum_at or time.time() - vacuum_at >= 86400:
-            self.conn.execute('VACUUM')
-            self.set(key=key_vacuum_at, value=int(time.time()))
+        with self.lock:
+            key_vacuum_at: str = '__VACUUM__'
+            vacuum_at: int | None = self.get(key=key_vacuum_at)
+            if force or not vacuum_at or time.time() - vacuum_at >= 86400:
+                self.conn.execute('VACUUM')
+                self.set(key=key_vacuum_at, value=int(time.time()))
 
     def close(self):
-        self.conn.commit()
-        self.vacuum(force=False)
-        self.conn.close()
+        with self.lock:
+            self.conn.commit()
+            self.vacuum(force=False)
+            self.conn.close()
```

### Comparing `jy_lib-0.7.2/jy_lib/clickhouse.py` & `jy_lib-0.7.3/jy_lib/clickhouse.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,14 @@
             return
         assert height >= 0
         csv: bytes = csv.encode('utf-8')
         with ZstdStreamCompressor(size=len(csv), level=zstandard.STRATEGY_FAST) as sc:
             sc.update(data=csv)
             stream: io.BytesIO = sc.stream
         with KeyboardInterruptProtect():
-            logger.debug(f'[{table_name}]准备插入{height:12,d}条数据')
             r = requests.post(
                 url=self.url_http,
                 params=params,
                 data=stream.getvalue(),
                 headers={
                     'Content-Encoding': 'zstd',
                     'Accept-Encoding': 'zstd',
@@ -270,14 +269,15 @@
     def import_df(self, table_name: str, df: pl.DataFrame, pks: Tuple):
         """将polars.DataFrame导入ClickHouse,约束列为pks"""
         datetime_format: str = '%Y-%m-%d %H:%M:%S.%f'
         assert self.database_name
         assert pks and set(df.columns).issuperset(pks)
         # 按主键去重
         df = df.unique(subset=pks)
+        logger.debug(f'[{table_name}]准备插入{df.height:12,d}条数据')
         # 通常第1主键为symbol
         pk1: str = pks[0]
         idx1: int = df.columns.index(pk1)
         assert df.dtypes[idx1] == pl.String
         pk1_vs = df[pk1].unique()
         outputs: str = ', '.join([f'`{pk}`' for pk in pks])
         sql = f"SELECT {outputs} FROM `{table_name}` WHERE "
```

### Comparing `jy_lib-0.7.2/jy_lib/compressor.py` & `jy_lib-0.7.3/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/country.py` & `jy_lib-0.7.3/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/currency.py` & `jy_lib-0.7.3/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/date.py` & `jy_lib-0.7.3/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/decorator.py` & `jy_lib-0.7.3/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/exchange.py` & `jy_lib-0.7.3/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/interrupt_protect.py` & `jy_lib-0.7.3/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/lock.py` & `jy_lib-0.7.3/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/math.py` & `jy_lib-0.7.3/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/nav.py` & `jy_lib-0.7.3/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/reader.py` & `jy_lib-0.7.3/jy_lib/reader.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/smb_client.py` & `jy_lib-0.7.3/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/symbol.py` & `jy_lib-0.7.3/jy_lib/symbol.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/symbol_em.py` & `jy_lib-0.7.3/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/jy_lib/time.py` & `jy_lib-0.7.3/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.2/pyproject.toml` & `jy_lib-0.7.3/pyproject.toml`

 * *Files identical despite different names*

