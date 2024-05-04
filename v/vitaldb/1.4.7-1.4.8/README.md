# Comparing `tmp/vitaldb-1.4.7-py3-none-any.whl.zip` & `tmp/vitaldb-1.4.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 56762 bytes, number of entries: 9
+Zip file size: 56814 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat   103238 b- defN 23-Nov-03 00:10 vitaldb/__init__.py
 -rw-rw-rw-  2.0 fat     4653 b- defN 23-Jul-02 09:38 vitaldb/api.py
 -rw-rw-rw-  2.0 fat     3305 b- defN 23-Jun-16 07:55 vitaldb/dataset.py
--rw-rw-rw-  2.0 fat    89138 b- defN 24-Jan-10 04:17 vitaldb/utils.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Jan-10 04:17 vitaldb-1.4.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      520 b- defN 24-Jan-10 04:17 vitaldb-1.4.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jan-10 04:17 vitaldb-1.4.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Jan-10 04:17 vitaldb-1.4.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      682 b- defN 24-Jan-10 04:17 vitaldb-1.4.7.dist-info/RECORD
-9 files, 202721 bytes uncompressed, 55604 bytes compressed:  72.6%
+-rw-rw-rw-  2.0 fat    89543 b- defN 24-May-04 01:12 vitaldb/utils.py
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      520 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      682 b- defN 24-May-04 01:49 vitaldb-1.4.8.dist-info/RECORD
+9 files, 203126 bytes uncompressed, 55656 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vitaldb/dataset.py
 Comment: 
 
 Filename: vitaldb/utils.py
 Comment: 
 
-Filename: vitaldb-1.4.7.dist-info/LICENSE
+Filename: vitaldb-1.4.8.dist-info/LICENSE
 Comment: 
 
-Filename: vitaldb-1.4.7.dist-info/METADATA
+Filename: vitaldb-1.4.8.dist-info/METADATA
 Comment: 
 
-Filename: vitaldb-1.4.7.dist-info/WHEEL
+Filename: vitaldb-1.4.8.dist-info/WHEEL
 Comment: 
 
-Filename: vitaldb-1.4.7.dist-info/top_level.txt
+Filename: vitaldb-1.4.8.dist-info/top_level.txt
 Comment: 
 
-Filename: vitaldb-1.4.7.dist-info/RECORD
+Filename: vitaldb-1.4.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vitaldb/utils.py

```diff
@@ -7,39 +7,39 @@
 import tempfile
 import numpy as np
 import pandas as pd
 from copy import deepcopy
 from urllib import parse, request
 from struct import pack, unpack_from, Struct
 
-unpack_b = Struct('<b').unpack_from
-unpack_w = Struct('<H').unpack_from
-unpack_s = Struct('<h').unpack_from
-unpack_f = Struct('<f').unpack_from
-unpack_d = Struct('<d').unpack_from
-unpack_dw = Struct('<L').unpack_from
-pack_b = Struct('<b').pack
-pack_w = Struct('<H').pack
-pack_s = Struct('<h').pack
-pack_f = Struct('<f').pack
-pack_d = Struct('<d').pack
-pack_dw = Struct('<L').pack
+_unpack_b = Struct('<b').unpack_from
+_unpack_w = Struct('<H').unpack_from
+_unpack_s = Struct('<h').unpack_from
+_unpack_f = Struct('<f').unpack_from
+_unpack_d = Struct('<d').unpack_from
+_unpack_dw = Struct('<L').unpack_from
+_pack_b = Struct('<b').pack
+_pack_w = Struct('<H').pack
+_pack_s = Struct('<h').pack
+_pack_f = Struct('<f').pack
+_pack_d = Struct('<d').pack
+_pack_dw = Struct('<L').pack
 
 
-def unpack_str(buf, pos):
-    strlen = unpack_dw(buf, pos)[0]
+def _unpack_str(buf, pos):
+    strlen = _unpack_dw(buf, pos)[0]
     pos += 4
     val = buf[pos:pos + strlen].decode('utf-8', 'ignore')
     pos += strlen
     return val, pos
 
 
-def pack_str(s):
+def _pack_str(s):
     sutf = s.encode('utf-8')
-    return pack_dw(len(sutf)) + sutf
+    return _pack_dw(len(sutf)) + sutf
 
 
 # open dataset trks
 dftrks = None
 
 class Device:
     def __init__(self, name, typename='', port=''):
@@ -444,14 +444,16 @@
             self.load_csv(ipath, track_names, exclude, interval)
         elif ext == '.hea':
             self.load_wfdb(ipath, track_names, header_only, exclude)
         elif ext == '.parquet':
             if header_only:
                 raise NotImplementedError
             self.load_parquet(ipath, track_names, exclude)
+        else:
+            self.load_vital(ipath, track_names, header_only, exclude, maxlen)
 
 
     def __repr__(self):
         return f'VitalFile(\'{self.ipath}\', \'{self.get_track_names()}\')'
 
     def get_samples(self, track_names, interval, return_datetime=False, return_timestamp=False):
         """Get track samples.
@@ -507,24 +509,25 @@
         elif dtfrom < 946684800:
             dtfrom = self.dtstart + dtfrom
 
         if dtend is None:
             dtend = self.dtend
         elif dtend < 0:
             dtend = self.dtend + dtend
-        elif dtend < 946684800:
-            dtend = self.dtstart + dtend
+        # elif dtend < 946684800:
+        #     dtend = self.dtstart + dtend
 
         if dtend < dtfrom:
             return
 
         for dtname, trk in self.trks.items():
             new_recs = []
             for rec in trk.recs:
-                if dtfrom <= rec['dt'] <= dtend:
+                rec_dtend = rec['dt'] + len(rec['val']) / trk.srate
+                if dtfrom <= rec['dt'] <= dtend or dtfrom <= rec_dtend <= dtend:
                     new_recs.append(rec)
             self.trks[dtname].recs = new_recs
         self.dtstart = dtfrom
         self.dtend = dtend
         return self
         
 
@@ -652,14 +655,17 @@
         if isinstance(dtnames, str):
             dtnames = [dtnames]
         for dtname in dtnames:
             self.del_track(dtname)
     
     del_tracks = remove_tracks
 
+    def add_device(self, dname, typename='', port=''):
+        self.devs[dname] = Device(dname, typename, port)
+
     def add_track(self, dtname, recs, srate=0, unit='', mindisp=0, maxdisp=0, after=None, col=None):
         if len(recs) == 0:
             return
 
         if 'val' not in recs[0] or 'dt' not in recs[0]:
             return
 
@@ -988,42 +994,42 @@
         :param opath: file path to save.
         """
         f = gzip.GzipFile(opath, 'wb', compresslevel=compresslevel)
 
         # save header
         if not f.write(b'VITA'):  # check sign
             return False
-        if not f.write(pack_dw(3)):  # version
+        if not f.write(_pack_dw(3)):  # version
             return False
-        if not f.write(pack_w(26)):  # header len
+        if not f.write(_pack_w(26)):  # header len
             return False
-        if not f.write(pack_s(self.dgmt)):  # dgmt = ut - localtime
+        if not f.write(_pack_s(self.dgmt)):  # dgmt = ut - localtime
             return False
-        if not f.write(pack_dw(0)):  # instance id
+        if not f.write(_pack_dw(0)):  # instance id
             return False
-        if not f.write(pack_dw(0)):  # program version
+        if not f.write(_pack_dw(0)):  # program version
             return False
-        if not f.write(pack_d(self.dtstart)):  # dtstart
+        if not f.write(_pack_d(self.dtstart)):  # dtstart
             return False
-        if not f.write(pack_d(self.dtend)):  # dtend
+        if not f.write(_pack_d(self.dtend)):  # dtend
             return False
 
         # save devinfos
         did = 0
         dname_dids = {}
         for dname, dev in self.devs.items():
             if dname == '': 
                 continue
             
             # issue did
             did += 1
             dname_dids[dname] = did
 
-            ddata = pack_dw(did) + pack_str(dev.type) + pack_str(dev.name) + pack_str(dev.port)
-            if not f.write(pack_b(9) + pack_dw(len(ddata)) + ddata):
+            ddata = _pack_dw(did) + _pack_str(dev.type) + _pack_str(dev.name) + _pack_str(dev.port)
+            if not f.write(_pack_b(9) + _pack_dw(len(ddata)) + ddata):
                 return False
 
         # save trkinfo
         tid = 0
         dtname_tids = {}
         for dtname, trk in self.trks.items():
             # issue tid
@@ -1045,41 +1051,41 @@
                     reclen += 4 + fmtlen * len(rec['val'])
                 elif trk.type == 2:  # num
                     fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
                     reclen += fmtlen
                 elif trk.type == 5:  # str
                     reclen += 8 + len(rec['val'].encode('utf-8'))
             
-            ti = pack_w(tid) + pack_b(trk.type) + pack_b(trk.fmt) + pack_str(trk.name) \
-                + pack_str(trk.unit) + pack_f(trk.mindisp) + pack_f(trk.maxdisp) \
-                + pack_dw(trk.col) + pack_f(trk.srate) + pack_d(trk.gain) + pack_d(trk.offset) \
-                + pack_b(trk.montype) + pack_dw(did) + pack_dw(reclen)
-            if not f.write(pack_b(0) + pack_dw(len(ti)) + ti):
+            ti = _pack_w(tid) + _pack_b(trk.type) + _pack_b(trk.fmt) + _pack_str(trk.name) \
+                + _pack_str(trk.unit) + _pack_f(trk.mindisp) + _pack_f(trk.maxdisp) \
+                + _pack_dw(trk.col) + _pack_f(trk.srate) + _pack_d(trk.gain) + _pack_d(trk.offset) \
+                + _pack_b(trk.montype) + _pack_dw(did) + _pack_dw(reclen)
+            if not f.write(_pack_b(0) + _pack_dw(len(ti)) + ti):
                 return False
 
         # save recs
         for dtname, trk in self.trks.items():
             tid = dtname_tids[dtname]
             for rec in trk.recs:
-                rdata = pack_w(10) + pack_d(rec['dt']) + pack_w(tid)  # infolen + dt + tid (= 12 bytes)
+                rdata = _pack_w(10) + _pack_d(rec['dt']) + _pack_w(tid)  # infolen + dt + tid (= 12 bytes)
                 if trk.type == 1:  # wav
-                    rdata += pack_dw(len(rec['val'])) + rec['val'].tobytes()
+                    rdata += _pack_dw(len(rec['val'])) + rec['val'].tobytes()
                 elif trk.type == 2:  # num
                     fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
                     rdata += pack(fmtcode, rec['val'])
                 elif trk.type == 5:  # str
-                    rdata += pack_dw(0) + pack_str(rec['val'])
-                if not f.write(pack_b(1) + pack_dw(len(rdata)) + rdata):
+                    rdata += _pack_dw(0) + _pack_str(rec['val'])
+                if not f.write(_pack_b(1) + _pack_dw(len(rdata)) + rdata):
                     return False
 
         # save trk order
         if len(self.order) > 0:
             tids = np.array([dtname_tids[dtname] for dtname in self.order], dtype=np.dtype('H'))
-            cdata = pack_b(5) + pack_w(len(tids)) + tids.tobytes()
-            if not f.write(pack_b(6) + pack_dw(len(cdata)) + cdata):
+            cdata = _pack_b(5) + _pack_w(len(tids)) + tids.tobytes()
+            if not f.write(_pack_b(6) + _pack_dw(len(cdata)) + cdata):
                 return False
 
         f.close()
         return True
 
     def get_dt(self, year, month, day, hour=0, minute=0, second=0.0):
         """ get unix timestamp based on the file's timezone
@@ -1128,15 +1134,15 @@
                     vals = rec['val'].astype(np.float32)
                     if trk.fmt > 2:  # 1: float, 2: double
                         vals *= trk.gain
                         vals += trk.offset
                     row['wval'] = vals.tobytes()
                     row['nval'] = trk.srate
                 elif trk.type == 2:  # num
-                    # row['val'] = pack_f(np.float32(rec['val']))
+                    # row['val'] = _pack_f(np.float32(rec['val']))
                     row['nval'] = rec['val']
                 elif trk.type == 5:  # str
                     row['sval'] = rec['val']
                 rows.append(row)
 
         df = pd.DataFrame(rows)
         if 'nval' in df:
@@ -1278,15 +1284,15 @@
                 self.trks[dtname] = trk
 
             # reading records
             trk = self.trks[dtname]
             rec = {'dt': row['dt']}
             if trk.type == 1:  # wav
                 rec['val'] = np.frombuffer(row['wval'], dtype=np.float32)
-                # rec['val'] = np.array(Struct('<{}f'.format(len(row['wval']) // 4)).unpack_from(row['wval'], 0), dtype=np.float32)
+                # rec['val'] = np.array(Struct('<{}f'.format(len(row['wval']) // 4))._unpack_from(row['wval'], 0), dtype=np.float32)
                 # TODO: dtend may be incorrect
             elif trk.type == 2:  # num
                 rec['val'] = row['nval']
             elif trk.type == 5:  # str
                 rec['val'] = row['sval']
             else:
                 continue
@@ -1547,97 +1553,97 @@
         if f.read(4) != b'VITA':  # check sign
             return False
 
         f.read(4)  # file version
         buf = f.read(2)
         if buf == b'':
             return False
-        headerlen = unpack_w(buf, 0)[0]
+        headerlen = _unpack_w(buf, 0)[0]
         header = f.read(headerlen)  # read header
-        self.dgmt = unpack_s(header, 0)[0]  # dgmt = ut - localtime
+        self.dgmt = _unpack_s(header, 0)[0]  # dgmt = ut - localtime
         if headerlen >= 26:
-            self.dtstart = unpack_d(header, 10)[0]
-            self.dtend = unpack_d(header, 18)[0]
+            self.dtstart = _unpack_d(header, 10)[0]
+            self.dtend = _unpack_d(header, 18)[0]
 
         # how many bytes to skip the records in this track
         tid_reclens = {}  # tid -> reclen
 
         # parse body
         try:
             tid_dtnames = {}  # tid -> dtname for this file
             did_dnames = {}  # did -> dname for this file
             while True:
                 buf = f.read(5)
                 if buf == b'':
                     break
                 pos = 0
 
-                packet_type = unpack_b(buf, pos)[0]; pos += 1
-                packet_len = unpack_dw(buf, pos)[0]; pos += 4
+                packet_type = _unpack_b(buf, pos)[0]; pos += 1
+                packet_len = _unpack_dw(buf, pos)[0]; pos += 4
                 if packet_len > 1000000: # maximum packet size should be < 1MB
                     break
                 
                 buf = f.read(packet_len)
                 if buf == b'':
                     break
                 pos = 0
 
                 if packet_type == 9:  # devinfo
-                    did = unpack_dw(buf, pos)[0]; pos += 4
-                    devtype, pos = unpack_str(buf, pos)
-                    name, pos = unpack_str(buf, pos)
+                    did = _unpack_dw(buf, pos)[0]; pos += 4
+                    devtype, pos = _unpack_str(buf, pos)
+                    name, pos = _unpack_str(buf, pos)
                     port = ''
                     if len(buf) > pos + 4:  # port is optional
-                        port, pos = unpack_str(buf, pos)
+                        port, pos = _unpack_str(buf, pos)
                     if not name:
                         name = devtype
                     self.devs[name] = Device(name, devtype, port)
                     did_dnames[did] = name
                 elif packet_type == 0:  # trkinfo
                     did = col = 0
                     montype = 0
                     unit = ''
                     gain = offset = srate = mindisp = maxdisp = 0.0
-                    tid = unpack_w(buf, pos)[0]; pos += 2
-                    trktype = unpack_b(buf, pos)[0]; pos += 1
-                    fmt = unpack_b(buf, pos)[0]; pos += 1
+                    tid = _unpack_w(buf, pos)[0]; pos += 2
+                    trktype = _unpack_b(buf, pos)[0]; pos += 1
+                    fmt = _unpack_b(buf, pos)[0]; pos += 1
                     if trktype == 1 or trktype == 2:
                         if fmt not in FMT_TYPE_LEN: 
                             continue
-                    tname, pos = unpack_str(buf, pos)
+                    tname, pos = _unpack_str(buf, pos)
 
                     if packet_len > pos:
-                        unit, pos = unpack_str(buf, pos)
+                        unit, pos = _unpack_str(buf, pos)
                     if packet_len > pos:
-                        mindisp = unpack_f(buf, pos)[0]
+                        mindisp = _unpack_f(buf, pos)[0]
                         pos += 4
                     if packet_len > pos:
-                        maxdisp = unpack_f(buf, pos)[0]
+                        maxdisp = _unpack_f(buf, pos)[0]
                         pos += 4
                     if packet_len > pos:
-                        col = unpack_dw(buf, pos)[0]
+                        col = _unpack_dw(buf, pos)[0]
                         pos += 4
                     if packet_len > pos:
-                        srate = unpack_f(buf, pos)[0]
+                        srate = _unpack_f(buf, pos)[0]
                         pos += 4
                     if packet_len > pos:
-                        gain = unpack_d(buf, pos)[0]
+                        gain = _unpack_d(buf, pos)[0]
                         pos += 8
                     if packet_len > pos:
-                        offset = unpack_d(buf, pos)[0]
+                        offset = _unpack_d(buf, pos)[0]
                         pos += 8
                     if packet_len > pos:
-                        montype = unpack_b(buf, pos)[0]
+                        montype = _unpack_b(buf, pos)[0]
                         pos += 1
                     if packet_len > pos:
-                        did = unpack_dw(buf, pos)[0]
+                        did = _unpack_dw(buf, pos)[0]
                         pos += 4
                     reclen = 0
                     if packet_len > pos:
-                        reclen = unpack_dw(buf, pos)[0]
+                        reclen = _unpack_dw(buf, pos)[0]
                         pos += 4
 
                     dname = ''
                     if did and did in did_dnames:
                         dname = did_dnames[did]
                         dtname = dname + '/' + tname
                     else:
@@ -1669,17 +1675,17 @@
                     
                     tid_dtnames[tid] = dtname
                     self.trks[dtname] = Track(tname, trktype, fmt=fmt, unit=unit, srate=srate, mindisp=mindisp, maxdisp=maxdisp, col=col, montype=montype, gain=gain, offset=offset, dname=dname)
                 elif packet_type == 1:  # rec
                     if len(buf) < pos + 12:
                         continue
 
-                    infolen = unpack_w(buf, pos)[0]; pos += 2
-                    dt = unpack_d(buf, pos)[0]; pos += 8
-                    tid = unpack_w(buf, pos)[0]; pos += 2
+                    infolen = _unpack_w(buf, pos)[0]; pos += 2
+                    dt = _unpack_d(buf, pos)[0]; pos += 8
+                    tid = _unpack_w(buf, pos)[0]; pos += 2
                     pos = 2 + infolen
 
                     if tid not in tid_dtnames:  # tid not to read
                         if tid in tid_reclens:
                             if tid_reclens[tid] > 5 + packet_len:
                                 f.seek(tid_reclens[tid] - (5 + packet_len), 1)
                         continue
@@ -1705,15 +1711,15 @@
 
                     fmtlen = 4
                     rec_dtend = dt
                     if trk.type == 1:  # wav
                         fmtcode, fmtlen = FMT_TYPE_LEN[trk.fmt]
                         if len(buf) < pos + 4:
                             continue
-                        nsamp = unpack_dw(buf, pos)[0]; pos += 4
+                        nsamp = _unpack_dw(buf, pos)[0]; pos += 4
                         if len(buf) < pos + nsamp * fmtlen:
                             continue
                         samps = np.ndarray((nsamp,), buffer=buf, offset=pos, dtype=np.dtype(fmtcode)); pos += nsamp * fmtlen
                         trk.recs.append({'dt': dt, 'val': samps})
                         if trk.srate > 0:
                             rec_dtend = dt + len(samps) / trk.srate
                             if rec_dtend > self.dtend:
@@ -1724,23 +1730,23 @@
                             continue
                         val = unpack_from(fmtcode, buf, pos)[0]; pos += fmtlen
                         trk.recs.append({'dt': dt, 'val': val})
                     elif trk.type == 5:  # str
                         pos += 4  # skip
                         if len(buf) < pos + 4:
                             continue
-                        s, pos = unpack_str(buf, pos)
+                        s, pos = _unpack_str(buf, pos)
                         trk.recs.append({'dt': dt, 'val': s})
                 elif packet_type == 6:  # cmd
-                    cmd = unpack_b(buf, pos)[0]; pos += 1
+                    cmd = _unpack_b(buf, pos)[0]; pos += 1
                     if cmd == 6:  # reset events
                         if 'EVENT' in self.trks:
                             self.trks['EVENT'].recs = []
                     elif cmd == 5:  # trk order
-                        cnt = unpack_w(buf, pos)[0]
+                        cnt = _unpack_w(buf, pos)[0]
                         pos += 2
                         tids = np.ndarray((cnt,), buffer=buf, offset=pos, dtype=np.dtype('H'))
                         self.order = []
                         for tid in tids:
                             if tid in tid_dtnames:
                                 self.order.append(tid_dtnames[tid])
                         pos += cnt * 2
```

## Comparing `vitaldb-1.4.7.dist-info/LICENSE` & `vitaldb-1.4.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vitaldb-1.4.7.dist-info/METADATA` & `vitaldb-1.4.8.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitaldb
-Version: 1.4.7
+Version: 1.4.8
 Summary: VitalDB Python Libray
 Home-page: https://github.com/vitaldb/vitalutils
 Author: Hyung-Chul Lee
 Author-email: vital@snu.ac.kr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `vitaldb-1.4.7.dist-info/RECORD` & `vitaldb-1.4.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 vitaldb/__init__.py,sha256=q-AbMSiCgHwv8c1hk2MKGpxVynKtrcJKzuOUHLw3on0,103238
 vitaldb/api.py,sha256=Kdmz9GGHSqLrgIPyZX_EnoR0ritjdCiRAWKtsIbpguc,4653
 vitaldb/dataset.py,sha256=qlwphbk8ayfdMdPsQtHZNHfXQPYQtx0yC5QVCn66tVw,3305
-vitaldb/utils.py,sha256=gR7y-H9kJERZBTRchfgZT24p2ejLFHqFJ-6L-305idw,89138
-vitaldb-1.4.7.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
-vitaldb-1.4.7.dist-info/METADATA,sha256=lh52SDRBQievavyrNcKmmDbOlMMFnPqp-5TNWp3TZBc,520
-vitaldb-1.4.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vitaldb-1.4.7.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
-vitaldb-1.4.7.dist-info/RECORD,,
+vitaldb/utils.py,sha256=twyahnydSE8kTAEOz6YZjTxzscmhQBzz16LgXvKE_-o,89543
+vitaldb-1.4.8.dist-info/LICENSE,sha256=h_p8qyePNkMbAgB4B_dsGwtNhTR3fSM38fGQIpTuodI,1085
+vitaldb-1.4.8.dist-info/METADATA,sha256=q6R5pN9jOVOAqmqFtGTl8IdeGUbGe5812CdhRsObb0s,520
+vitaldb-1.4.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+vitaldb-1.4.8.dist-info/top_level.txt,sha256=xJoTTkaIm_WeMoAfX0de2vl5Ns40HOLc0FX-dI2IoDw,8
+vitaldb-1.4.8.dist-info/RECORD,,
```

