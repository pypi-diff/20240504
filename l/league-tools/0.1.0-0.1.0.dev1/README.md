# Comparing `tmp/league_tools-0.1.0.tar.gz` & `tmp/league_tools-0.1.0.dev1.tar.gz`

## Comparing `league_tools-0.1.0.tar` & `league_tools-0.1.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.1.0/1.json
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0/requirements.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.1.0/requirements.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/__init__.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/base.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/index.py
--rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/BIN.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/BNK.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/WAD.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/WPK.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/__init__.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/section/BKHD.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/section/DATA.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/section/DIDX.py
--rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/section/HIRC.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/formats/section/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/tools/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/tools/Binary/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.1.0/league_tools/tools/Binary/reader.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.1.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.1.0/README.md
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 league_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    44982 2020-02-02 00:00:00.000000 league_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    17209 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/1.json
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements-dev.lock
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/requirements.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/__init__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/base.py
+-rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/index.py
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/BIN.py
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/BNK.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/WAD.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/WPK.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/__init__.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/BKHD.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/DATA.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/DIDX.py
+-rw-r--r--   0        0        0    15754 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/HIRC.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/formats/section/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/Binary/__init__.py
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/tools/Binary/reader.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/utils/__init__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/league_tools/utils/type_hints.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0    44987 2020-02-02 00:00:00.000000 league_tools-0.1.0.dev1/PKG-INFO
```

### Comparing `league_tools-0.1.0/1.json` & `league_tools-0.1.0.dev1/1.json`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/base.py` & `league_tools-0.1.0.dev1/league_tools/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/2/27 19:36
-# @Update  : 2024/5/4 16:50
+# @Update  : 2024/5/5 2:16
 # @Detail  : 块 基类
 
 import os
 import subprocess
 from dataclasses import dataclass
 from io import BytesIO
+from pathlib import Path
 from typing import Union
 
 from league_tools.tools import BinaryReader
 
 
 class SectionNoId:
     def __init__(self, data: Union[BinaryReader, BytesIO, bytes, str, os.PathLike]):
@@ -100,39 +101,40 @@
         :param data: 数据
         :param path: 文件路径
         :param wem: 如果转码是否保留wem文件
         :param vgmstream_cli: vgmstream_cli程序用来转码
         :return:
         """
         assert data, '不存在文件数据, 请调用DATA.get_file后, 在进行保存.'
+        path = Path(path)
+
+        wem_path = path.with_suffix('.wem')
 
-        file, ext = os.path.splitext(path)
-        wem_path = f'{file}.wem'
         with open(wem_path, 'wb+') as f:
             f.write(data)
 
-        if ext != '.wem':
-            if vgmstream_cli:
-                subprocess.run([
-                    vgmstream_cli,
-                    f'{wem_path}',
-                    '-o'
-                    f'{path}'
-                ],
-                    stdout=subprocess.DEVNULL,
-                    timeout=999999999
-                )
-                if not wem:
-                    os.remove(wem_path)
+        if (path.suffix != '.wem') and vgmstream_cli:
+            subprocess.run([
+                vgmstream_cli,
+                str(wem_path),
+                '-o',
+                str(path)
+            ],
+                stdout=subprocess.DEVNULL,
+                timeout=999999999
+            )
+            if not wem:
+                wem_path.unlink()
         del data
 
     def __iter__(self):
         return [self.id, self.offset, self.length]
 
     def __dict__(self):
         return dict(id=self.id, offset=self.offset, length=self.length)
 
     def __repr__(self):
         return f'File_Id: {self.id}, ' \
                f'File_Length: {self.length},' \
                f'File_Name: {self.filename}'
 
+
```

### Comparing `league_tools-0.1.0/league_tools/index.py` & `league_tools-0.1.0.dev1/league_tools/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/2/27 18:28
-# @Update  : 2024/5/4 16:50
+# @Update  : 2024/5/5 2:43
 # @Detail  : 
 
 # References : http://wiki.xentax.com/index.php/Wwise_SoundBank_(*.bnk)#HIRC_section
 
 import logging
-import os
 from collections import OrderedDict, defaultdict
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from pathlib import Path
 from typing import List, Optional, Union
 
 from loguru import logger
 
 from league_tools.base import WemFile
 from league_tools.formats.BIN import BIN, StringHash
 from league_tools.formats.BNK import BNK, HIRC
 from league_tools.formats.WPK import WPK
 from league_tools.tools.Binary import BinaryReader
+from league_tools.utils.type_hints import StrPath
 
 
 def get_audio_id_by_songs(event_str, event_id, songs):
     """
     根据ID在Sound列表(迭代器)生成资源ID列表
     :param event_str:
     :param event_id:
@@ -154,26 +155,26 @@
                 res.extend(
                     get_audio_hash_by_rs_containers(string.string, reference_id, hirc.rs_containers, hirc.sounds)
                 )
 
     return res
 
 
-def get_audio_files(audio_file: Union[str, bytes, os.PathLike], get_data=True, hash_table: Optional[List[int]] = None) \
+def get_audio_files(audio_file: StrPath, get_data=True, hash_table: Optional[List[int]] = None) \
         -> List[WemFile]:
     """
     提供音频文件, 返回文件列表
     :param audio_file: 音频文件(bnk、wpk)
     :param get_data: 是否获取音频文件数据
     :param hash_table: 哈希表
     :return:
     """
 
-    if isinstance(audio_file, str) or isinstance(audio_file, os.PathLike):
-        audio_ext = os.path.splitext(audio_file)[-1]
+    if isinstance(audio_file, StrPath):
+        audio_ext = Path(audio_file).suffix
     elif isinstance(audio_file, bytes):
         br = BinaryReader(audio_file)
         head = br.customize('<4s')
         audio_ext = '.wpk' if head == b'r3d2' else '.bnk'
     else:
         return []
 
@@ -201,22 +202,22 @@
 
     if get_data:
         data_call()
 
     return audio_files
 
 
-def get_event_hashtable(bin_file: Union[str, List[StringHash]], event_file):
+def get_event_hashtable(bin_file: Union[StrPath, List[StringHash]], event_file):
     """
     根据皮肤bin文件以及音频事件, 提取事件哈希表
     :param bin_file: bin文件
     :param event_file: bnk event文件
     :return:
     """
-    if isinstance(bin_file, str):
+    if isinstance(bin_file, StrPath):
         b1 = BIN(bin_file)
         # 获取事件哈希表
         read_strings = b1.hash_tables.copy()
     else:
         read_strings = bin_file.copy()
     # 解析事件文件
     event = BNK(event_file)
@@ -261,15 +262,15 @@
     sort_keys = sorted(ret.keys())
     order_ret = OrderedDict()
     for key in sort_keys:
         order_ret[key] = sorted(ret[key])
     return order_ret
 
 
-def extract_not_classified(audio_file, out_dir, ext=None, wem=False, vgmstream_cli=None, worker=None):
+def extract_not_classified(audio_file: StrPath, out_dir: StrPath, ext=None, wem=False, vgmstream_cli=None, worker=None):
     """
     无需分类直接提取文件
     :param audio_file: 音频文件, 可以是bnk和wpk文件
     :param out_dir: 输出文件夹
     :param ext: 转码所需后缀名
     :param wem: 转码后是否保留wem文件, 默认删除
     :param vgmstream_cli: 转码所需程序vgmstream
@@ -279,25 +280,25 @@
     if ext and ext != 'wem' and not vgmstream_cli:
         raise TypeError('如需转码需要提供 vgmstream_cli 参数.')
 
     audio_files = get_audio_files(audio_file)
 
     with ThreadPoolExecutor(max_workers=worker) as executor:
         future_to_path = {
-            executor.submit(file.save_file, os.path.join(out_dir, file.filename or f'{file.id}.wem'), wem,
+            executor.submit(file.save_file, Path(out_dir).joinpath(file.filename or f'{file.id}.wem'), wem,
                             vgmstream_cli): file for file in audio_files}
         for future in as_completed(future_to_path):
             path = future_to_path[future]
             try:
                 future.result()
             except Exception as exc:
                 logger.error(f'提取文件出错: {exc}, 出错文件: {path}')
 
 
-def extract_audio(bin_file: Union[str, List[StringHash]], event_file, audio_file, out_dir, ext=None,
+def extract_audio(bin_file: Union[StrPath, List[StringHash]], event_file, audio_file, out_dir, ext=None,
                   vgmstream_cli=None,
                   wem=True):
     """
     通过皮肤信息文件以及事件、资源文件, 提取音频文件, 支持转码
     :param bin_file: 皮肤信息bin文件或直接提供事件哈希表
     :param event_file: 皮肤事件bnk文件
     :param audio_file: 音频文件wpk或bnk文件
@@ -319,36 +320,34 @@
     file_ids = [file.id for file in audio_files]
     no_event = list(set(file_ids).difference(set(event_ids)))
     no_event_files = [file for file in audio_files if file.id in no_event]
 
     for file in no_event_files:
         name = file.filename or f'{file.id}.wem'
         if ext:
-            name = f'{os.path.splitext(name)[0]}.{ext}'
+            name = Path(name).stem + '.' + ext
         logging.debug(f'No Event, File: {file.id}')
-        file.save_file(os.path.join(out_dir, name), wem, vgmstream_cli=vgmstream_cli)
-        
+        file.save_file(Path(out_dir).joinpath(name), wem, vgmstream_cli=vgmstream_cli)
+
     # 去重
     temp = {}
     for eh in event_hashes:
         for file in audio_files:
             if eh.hash == file.id:
                 name = file.filename or f'{file.id}.wem'
                 if ext:
-                    name = f'{os.path.splitext(name)[0]}.{ext}'
+                    name = f'{Path(name).stem}.{ext}'
 
-                _dir = os.path.join(out_dir, eh.string)
-                if not os.path.exists(_dir):
-                    os.makedirs(_dir)
+                _dir = Path(out_dir).joinpath(eh.string)
+                _dir.mkdir(parents=True, exist_ok=True)
 
                 if file.id not in temp:
-                    temp.update({file.id: os.path.join(_dir, name)})
+                    temp.update({file.id: _dir.joinpath(name)})
                     logging.debug(f'Event: {eh.string}, File: {name}')
-                    file.save_file(os.path.join(_dir, name), wem, vgmstream_cli=vgmstream_cli)
+                    file.save_file(_dir.joinpath(name), wem, vgmstream_cli=vgmstream_cli)
 
                 else:
                     # 创建链接
                     try:
-                        os.symlink(temp[file.id], os.path.join(_dir, name))
+                        temp[file.id].symlink_to(_dir.joinpath(name))
                     except FileExistsError:
                         pass
-
```

### Comparing `league_tools-0.1.0/league_tools/formats/BIN.py` & `league_tools-0.1.0.dev1/league_tools/formats/BIN.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/BNK.py` & `league_tools-0.1.0.dev1/league_tools/formats/BNK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/WAD.py` & `league_tools-0.1.0.dev1/league_tools/formats/WAD.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # -*- coding: utf-8 -*-
 # @Author  : Virace
 # @Email   : Virace@aliyun.com
 # @Site    : x-item.com
 # @Software: PyCharm
 # @Create  : 2021/3/2 22:36
-# @Update  : 2024/5/4 16:50
+# @Update  : 2024/5/5 2:21
 # @Detail  : 文件结构来源于以下两个库
 
 # https://github.com/Pupix/lol-wad-parser/tree/master/lib
 # https://github.com/CommunityDragon/CDTB/blob/master/cdragontoolbox/wad.py
 
 import gzip
 import os
 from dataclasses import dataclass
+from pathlib import Path
 from typing import AnyStr, Callable, Dict, List, Union
 
 import xxhash
 import zstd
 from loguru import logger
 
 from league_tools.base import SectionNoId
 from league_tools.tools import BinaryReader
+from league_tools.utils.type_hints import StrPath
 
 
 @dataclass
 class WADSection:
     """
         pathHash: parser.uint64(),
         offset: parser.uint(),
@@ -88,15 +90,16 @@
 
     @staticmethod
     def get_hash(path: str):
         xx = xxhash.xxh64()
         xx.update(path.lower().encode('utf-8'))
         return int(xx.hexdigest(), 16)
 
-    def _extract(self, file, file_path, raw=False):
+    def _extract(self, file, file_path: StrPath, raw: bool = False):
+        file_path = Path(file_path)
         self._data.seek(file.offset, 0)
         this = self._data.bytes(file.compressed_file_size)
         # https://github.com/Pupix/lol-wad-parser/blob/2de5a9dafb77b7165b568316d5c1b1f8b5e898f2/lib/extract.js#L11
         # https://github.com/CommunityDragon/CDTB/blob/2663610ed10a2f5fdeeadc5860abca275bcd6af6/cdragontoolbox/wad.py#L82
         if file.type == 0:
             data = this
         elif file.type == 1:
@@ -112,24 +115,23 @@
             data = zstd.decompress(this)
         else:
             raise ValueError(f"不支持的文件类型: {file.type}")
 
         if raw:
             return data
         else:
-            file_dir = os.path.dirname(file_path)
-            if not os.path.exists(file_dir):
-                os.makedirs(file_dir)
+            if not file_path.parent.exists():
+                file_path.parent.mkdir(parents=True, exist_ok=True)
 
             logger.debug(f'提取文件: {file_path}')
             with open(file_path, 'wb+') as f:
                 f.write(data)
             return file_path
 
-    def extract(self, paths: List[str], out_dir: Union[AnyStr, Callable] = '', raw=False) -> List:
+    def extract(self, paths: List[StrPath], out_dir: Union[AnyStr, Callable] = '', raw=False) -> List:
         """
         提供需要解包的文件路径, 解包wad文件
         :param paths: 文件路径列表, 例如['assets/characters/aatrox/skins/base/aatrox.skn']
         :param out_dir: 输出文件夹
         :param raw: 源数据
         :return:
         """
@@ -141,15 +143,15 @@
             t = False
             for file in self.files:
                 if path_hash == file.path_hash:
                     t = True
                     if isinstance(out_dir, Callable):
                         file_path = out_dir(path)
                     else:
-                        file_path = os.path.join(out_dir, os.path.normpath(path))
+                        file_path = Path(out_dir) / Path(path).as_posix()
                     ret.append(self._extract(file, file_path, raw))
             if raw and not t:
                 # 源数据模式保证文件顺序与paths相同
                 ret.append(None)
         return ret
 
     def extract_hash(self, hashtable: Dict[str, str], out_dir: str = '') -> List:
@@ -160,12 +162,12 @@
         :return:
         """
 
         ret = []
         for file in self.files:
             if (s := str(file.path_hash)) in hashtable:
                 path = hashtable[s]
-                file_path = os.path.join(out_dir, os.path.normpath(path))
+                file_path = Path(out_dir) / Path(path).as_posix()
                 self._extract(file, file_path)
                 ret.append(file_path)
         return ret
```

### Comparing `league_tools-0.1.0/league_tools/formats/WPK.py` & `league_tools-0.1.0.dev1/league_tools/formats/WPK.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/section/BKHD.py` & `league_tools-0.1.0.dev1/league_tools/formats/section/BKHD.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/section/DATA.py` & `league_tools-0.1.0.dev1/league_tools/formats/section/DATA.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/section/DIDX.py` & `league_tools-0.1.0.dev1/league_tools/formats/section/DIDX.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/formats/section/HIRC.py` & `league_tools-0.1.0.dev1/league_tools/formats/section/HIRC.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/league_tools/tools/Binary/reader.py` & `league_tools-0.1.0.dev1/league_tools/tools/Binary/reader.py`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/.gitignore` & `league_tools-0.1.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/LICENSE` & `league_tools-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/README.md` & `league_tools-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `league_tools-0.1.0/pyproject.toml` & `league_tools-0.1.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "league-tools"
-version = "0.1.0"
+version = "0.1.0dev1"
 description = "WAD、BIN、BNK、WPK文件简单处理"
 authors = [{ name = "Virace", email = "Virace@aliyun.com" }]
 keywords = ["league", "wad", "bnk"]
 dependencies = [
     "xxhash>=3.4.1",
     "loguru>=0.7.2",
     "zstd>=1.5.5.1",
```

### Comparing `league_tools-0.1.0/PKG-INFO` & `league_tools-0.1.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: league-tools
-Version: 0.1.0
+Version: 0.1.0.dev1
 Summary: WAD、BIN、BNK、WPK文件简单处理
 Project-URL: homepage, https://github.com/Virace/py-bnk-extract
 Project-URL: repository, https://github.com/Virace/py-bnk-extract
 Project-URL: Bug Tracker, https://github.com/Virace/py-bnk-extract/issues
 Author-email: Virace <Virace@aliyun.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

