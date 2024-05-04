# Comparing `tmp/pyvserv-1.0.4.tar.gz` & `tmp/pyvserv-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvserv-1.0.4.tar", last modified: Wed Apr 24 16:22:50 2024, max compression
+gzip compressed data, was "pyvserv-1.0.6.tar", last modified: Sat May  4 15:30:18 2024, max compression
```

## Comparing `pyvserv-1.0.4.tar` & `pyvserv-1.0.6.tar`

### file list

```diff
@@ -1,144 +1,160 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.4/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-04-24 16:22:50.264470 pyvserv-1.0.4/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    17156 2024-04-10 00:53:07.000000 pyvserv-1.0.4/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.208470 pyvserv-1.0.4/pyvclient/
--rw-rw-r--   0 peterglen  (1000) users      (100)       14 2024-04-15 07:22:33.000000 pyvserv-1.0.4/pyvclient/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.232470 pyvserv-1.0.4/pyvclient/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    13937 2024-04-15 06:50:03.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_acc.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12079 2024-04-15 06:49:27.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_akey.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13072 2024-04-15 06:49:28.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_bigget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14945 2024-04-15 06:49:29.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_cd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24511 2024-04-15 06:49:30.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_cli.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11941 2024-04-15 06:49:31.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fdel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11688 2024-04-15 06:49:31.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12082 2024-04-15 06:49:32.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_file.html
--rw-r--r--   0 peterglen  (1000) users      (100)    18815 2024-04-15 06:49:33.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11794 2024-04-15 06:49:34.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fput.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12743 2024-04-15 06:49:35.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_gethelp.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13095 2024-04-15 06:49:36.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_hello.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10536 2024-04-10 00:54:07.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_id.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14864 2024-04-15 06:49:38.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ihost.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12497 2024-04-15 06:49:39.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_login.html
--rw-r--r--   0 peterglen  (1000) users      (100)    13464 2024-04-15 06:49:41.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ls.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12238 2024-04-15 06:49:40.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_lsd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:42.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_mkdir.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12205 2024-04-15 06:49:42.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_pass.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10253 2024-04-15 06:49:43.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ping.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14879 2024-04-15 06:49:44.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_qr.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16745 2024-04-15 06:49:45.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rabs.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16354 2024-04-15 06:49:46.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rcheck.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14273 2024-04-15 06:49:47.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rcount.html
--rw-r--r--   0 peterglen  (1000) users      (100)    32879 2024-04-15 06:57:46.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_replic.html
--rw-r--r--   0 peterglen  (1000) users      (100)    17860 2024-04-15 06:49:49.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rget.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16101 2024-04-15 06:49:50.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rlist.html
--rw-r--r--   0 peterglen  (1000) users      (100)    24463 2024-04-15 06:49:51.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:52.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rmdir.html
--rw-r--r--   0 peterglen  (1000) users      (100)    18495 2024-04-15 06:49:53.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rput.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14769 2024-04-15 06:49:54.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_sess.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16015 2024-04-15 06:50:05.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_sess_tout.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11681 2024-04-15 06:49:55.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_throt.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10607 2024-04-15 06:50:04.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_tout.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11574 2024-04-15 06:49:56.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uadd.html
--rw-r--r--   0 peterglen  (1000) users      (100)    14358 2024-04-15 06:49:57.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uchpass.html
--rw-r--r--   0 peterglen  (1000) users      (100)    11365 2024-04-15 06:49:58.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_udel.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12115 2024-04-15 06:49:59.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uena.html
--rw-r--r--   0 peterglen  (1000) users      (100)    16680 2024-04-15 06:50:00.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uini.html
--rw-r--r--   0 peterglen  (1000) users      (100)    20642 2024-04-15 06:50:01.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uman.html
--rw-r--r--   0 peterglen  (1000) users      (100)    12963 2024-04-15 06:50:02.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ver.html
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.4/pyvclient/loadtest.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3848 2024-04-06 08:48:29.000000 pyvserv-1.0.4/pyvclient/pyvcli_akey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4743 2024-04-09 14:23:35.000000 pyvserv-1.0.4/pyvclient/pyvcli_bigget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5567 2024-04-06 08:47:43.000000 pyvserv-1.0.4/pyvclient/pyvcli_cd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     9985 2024-04-11 22:53:59.000000 pyvserv-1.0.4/pyvclient/pyvcli_cli.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3784 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fdel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3503 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3976 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_file.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6078 2024-04-10 01:59:10.000000 pyvserv-1.0.4/pyvclient/pyvcli_fman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3639 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3156 2024-04-09 05:49:52.000000 pyvserv-1.0.4/pyvclient/pyvcli_gethelp.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3409 2024-04-09 05:40:35.000000 pyvserv-1.0.4/pyvclient/pyvcli_hello.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2432 2024-04-05 22:02:34.000000 pyvserv-1.0.4/pyvclient/pyvcli_id.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6166 2024-04-12 22:44:34.000000 pyvserv-1.0.4/pyvclient/pyvcli_ihost.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3988 2024-04-06 08:49:18.000000 pyvserv-1.0.4/pyvclient/pyvcli_login.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4960 2024-04-06 08:50:29.000000 pyvserv-1.0.4/pyvclient/pyvcli_ls.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4076 2024-04-06 08:50:00.000000 pyvserv-1.0.4/pyvclient/pyvcli_lsd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_mkdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3776 2024-04-06 08:50:51.000000 pyvserv-1.0.4/pyvclient/pyvcli_pass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.4/pyvclient/pyvcli_ping.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4099 2024-04-09 05:32:53.000000 pyvserv-1.0.4/pyvclient/pyvcli_qr.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4992 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rabs.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4816 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rcheck.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3850 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rcount.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    13786 2024-04-15 11:47:19.000000 pyvserv-1.0.4/pyvclient/pyvcli_replic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5462 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4659 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rlist.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     8530 2024-04-10 01:58:55.000000 pyvserv-1.0.4/pyvclient/pyvcli_rman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rmdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5788 2024-04-12 12:45:56.000000 pyvserv-1.0.4/pyvclient/pyvcli_rput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6137 2024-04-05 13:27:04.000000 pyvserv-1.0.4/pyvclient/pyvcli_sess.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3548 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_throt.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3353 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uadd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5689 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uchpass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3192 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_udel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3867 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uena.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4818 2024-04-14 07:07:11.000000 pyvserv-1.0.4/pyvclient/pyvcli_uini.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6972 2024-04-10 01:56:40.000000 pyvserv-1.0.4/pyvclient/pyvcli_uman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3171 2024-04-09 05:24:42.000000 pyvserv-1.0.4/pyvclient/pyvcli_ver.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.244470 pyvserv-1.0.4/pyvcommon/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:55.000000 pyvserv-1.0.4/pyvcommon/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    12254 2024-04-15 07:57:44.000000 pyvserv-1.0.4/pyvcommon/comline.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.4/pyvcommon/crysupp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.4/pyvcommon/genstrerr.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    17642 2024-04-08 08:14:28.000000 pyvserv-1.0.4/pyvcommon/pyclisup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.4/pyvcommon/pycrypt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6778 2024-04-11 23:55:27.000000 pyvserv-1.0.4/pyvcommon/pydata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    29729 2024-04-13 16:24:30.000000 pyvserv-1.0.4/pyvcommon/pyservsup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.4/pyvcommon/pysyslog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.4/pyvcommon/pyv2fa.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10878 2024-04-22 16:13:09.000000 pyvserv-1.0.4/pyvcommon/pyvhash.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.4/pyvcommon/pywrap.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9529 2024-04-15 10:48:15.000000 pyvserv-1.0.4/pyvcommon/support.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.248470 pyvserv-1.0.4/pyvgui/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:37.000000 pyvserv-1.0.4/pyvgui/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.248470 pyvserv-1.0.4/pyvgui/guilib/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:46.000000 pyvserv-1.0.4/pyvgui/guilib/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14679 2024-04-15 14:58:07.000000 pyvserv-1.0.4/pyvgui/guilib/mainwin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.4/pyvgui/guilib/mainwinserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13042 2024-04-16 02:33:20.000000 pyvserv-1.0.4/pyvgui/guilib/mainwintally.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    25146 2024-04-24 15:14:24.000000 pyvserv-1.0.4/pyvgui/guilib/mainwinvote.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10767 2024-04-21 14:12:22.000000 pyvserv-1.0.4/pyvgui/guilib/pgcal.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.4/pyvgui/guilib/pgui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.4/pyvgui/guilib/pymenu.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    13331 2024-04-24 16:00:43.000000 pyvserv-1.0.4/pyvgui/guilib/recsel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3104 2024-04-03 07:29:15.000000 pyvserv-1.0.4/pyvgui/pyvcpanel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2682 2024-04-03 07:32:33.000000 pyvserv-1.0.4/pyvgui/pyvservui.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3089 2024-04-03 07:47:23.000000 pyvserv-1.0.4/pyvgui/pyvtally.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2893 2024-04-24 13:07:58.000000 pyvserv-1.0.4/pyvgui/pyvvote.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvserv.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)     3498 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)      640 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/requires.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/top_level.txt
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.256470 pyvserv-1.0.4/pyvserver/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:41.000000 pyvserv-1.0.4/pyvserver/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.260470 pyvserv-1.0.4/pyvserver/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)   171300 2024-04-15 06:32:07.000000 pyvserv-1.0.4/pyvserver/docs/pyvfunc.html
--rw-r--r--   0 peterglen  (1000) users      (100)    76482 2024-04-15 06:32:05.000000 pyvserv-1.0.4/pyvserver/docs/pyvreplic.html
--rw-r--r--   0 peterglen  (1000) users      (100)    68036 2024-04-15 06:32:04.000000 pyvserv-1.0.4/pyvserver/docs/pyvserv.html
--rw-r--r--   0 peterglen  (1000) users      (100)    35380 2024-04-15 06:32:06.000000 pyvserv-1.0.4/pyvserver/docs/pyvstate.html
--rw-rw-r--   0 peterglen  (1000) users      (100)    67566 2024-04-15 10:22:32.000000 pyvserv-1.0.4/pyvserver/pyvfunc.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    23259 2024-04-15 06:31:36.000000 pyvserv-1.0.4/pyvserver/pyvreplic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    22417 2024-04-15 05:56:51.000000 pyvserv-1.0.4/pyvserver/pyvserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14128 2024-04-15 10:48:53.000000 pyvserv-1.0.4/pyvserver/pyvstate.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvtools/
--rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:20.000000 pyvserv-1.0.4/pyvtools/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvtools/docs/
--rw-r--r--   0 peterglen  (1000) users      (100)    16315 2024-04-23 13:55:15.000000 pyvserv-1.0.4/pyvtools/docs/pyvgenkey.html
--rw-r--r--   0 peterglen  (1000) users      (100)    10283 2024-04-23 13:55:14.000000 pyvserv-1.0.4/pyvtools/docs/pyvgenkeys.html
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.4/pyvtools/pyvgenkey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2508 2024-04-09 08:30:16.000000 pyvserv-1.0.4/pyvtools/pyvgenkeys.py
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-24 16:22:50.264470 pyvserv-1.0.4/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     4908 2024-04-24 16:22:17.000000 pyvserv-1.0.4/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.6/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 15:30:18.155934 pyvserv-1.0.6/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17156 2024-04-10 00:53:07.000000 pyvserv-1.0.6/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.131934 pyvserv-1.0.6/pyvclient/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       14 2024-04-15 07:22:33.000000 pyvserv-1.0.6/pyvclient/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.139934 pyvserv-1.0.6/pyvclient/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    13937 2024-04-15 06:50:03.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_acc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12079 2024-04-15 06:49:27.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_akey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13072 2024-04-15 06:49:28.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_bigget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14945 2024-04-15 06:49:29.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_cd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24511 2024-04-15 06:49:30.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_cli.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11941 2024-04-15 06:49:31.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fdel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11688 2024-04-15 06:49:31.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12082 2024-04-15 06:49:32.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_file.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18815 2024-04-15 06:49:33.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11794 2024-04-15 06:49:34.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_fput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12743 2024-04-15 06:49:35.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_gethelp.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13095 2024-04-15 06:49:36.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_hello.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10536 2024-04-10 00:54:07.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_id.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14864 2024-04-15 06:49:38.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ihost.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12497 2024-04-15 06:49:39.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_login.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13464 2024-04-15 06:49:41.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ls.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12238 2024-04-15 06:49:40.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_lsd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:42.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_mkdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12205 2024-04-15 06:49:42.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_pass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10253 2024-04-15 06:49:43.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ping.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14879 2024-04-15 06:49:44.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_qr.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16745 2024-04-15 06:49:45.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rabs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16354 2024-04-15 06:49:46.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rcheck.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14273 2024-04-15 06:49:47.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rcount.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32879 2024-04-15 06:57:46.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_replic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17860 2024-04-15 06:49:49.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16101 2024-04-15 06:49:50.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rlist.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24463 2024-04-15 06:49:51.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:52.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rmdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18495 2024-04-15 06:49:53.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_rput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14769 2024-04-15 06:49:54.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_sess.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16015 2024-04-15 06:50:05.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_sess_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11681 2024-04-15 06:49:55.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_throt.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10607 2024-04-15 06:50:04.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11574 2024-04-15 06:49:56.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uadd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14358 2024-04-15 06:49:57.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uchpass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11365 2024-04-15 06:49:58.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_udel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12115 2024-04-15 06:49:59.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uena.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16680 2024-04-15 06:50:00.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uini.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    20642 2024-04-15 06:50:01.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_uman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12963 2024-04-15 06:50:02.000000 pyvserv-1.0.6/pyvclient/docs/pyvcli_ver.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.6/pyvclient/loadtest.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3848 2024-04-06 08:48:29.000000 pyvserv-1.0.6/pyvclient/pyvcli_akey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4743 2024-04-09 14:23:35.000000 pyvserv-1.0.6/pyvclient/pyvcli_bigget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5567 2024-04-06 08:47:43.000000 pyvserv-1.0.6/pyvclient/pyvcli_cd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     9985 2024-04-11 22:53:59.000000 pyvserv-1.0.6/pyvclient/pyvcli_cli.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3784 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fdel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3503 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3976 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_file.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6078 2024-04-10 01:59:10.000000 pyvserv-1.0.6/pyvclient/pyvcli_fman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3639 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_fput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3156 2024-04-09 05:49:52.000000 pyvserv-1.0.6/pyvclient/pyvcli_gethelp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3409 2024-04-09 05:40:35.000000 pyvserv-1.0.6/pyvclient/pyvcli_hello.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2432 2024-04-05 22:02:34.000000 pyvserv-1.0.6/pyvclient/pyvcli_id.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6166 2024-04-12 22:44:34.000000 pyvserv-1.0.6/pyvclient/pyvcli_ihost.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3988 2024-04-06 08:49:18.000000 pyvserv-1.0.6/pyvclient/pyvcli_login.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4960 2024-04-06 08:50:29.000000 pyvserv-1.0.6/pyvclient/pyvcli_ls.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4076 2024-04-06 08:50:00.000000 pyvserv-1.0.6/pyvclient/pyvcli_lsd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_mkdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3776 2024-04-06 08:50:51.000000 pyvserv-1.0.6/pyvclient/pyvcli_pass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.6/pyvclient/pyvcli_ping.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4099 2024-04-09 05:32:53.000000 pyvserv-1.0.6/pyvclient/pyvcli_qr.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4992 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rabs.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4816 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rcheck.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3850 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rcount.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    13786 2024-04-15 11:47:19.000000 pyvserv-1.0.6/pyvclient/pyvcli_replic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5462 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4659 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rlist.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     8530 2024-04-10 01:58:55.000000 pyvserv-1.0.6/pyvclient/pyvcli_rman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_rmdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5788 2024-04-12 12:45:56.000000 pyvserv-1.0.6/pyvclient/pyvcli_rput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6137 2024-04-05 13:27:04.000000 pyvserv-1.0.6/pyvclient/pyvcli_sess.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3548 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_throt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3353 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uadd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5689 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uchpass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3192 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_udel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3867 2024-04-09 05:45:08.000000 pyvserv-1.0.6/pyvclient/pyvcli_uena.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4818 2024-04-14 07:07:11.000000 pyvserv-1.0.6/pyvclient/pyvcli_uini.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6972 2024-04-10 01:56:40.000000 pyvserv-1.0.6/pyvclient/pyvcli_uman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3171 2024-04-09 05:24:42.000000 pyvserv-1.0.6/pyvclient/pyvcli_ver.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvcommon/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:55.000000 pyvserv-1.0.6/pyvcommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12254 2024-04-15 07:57:44.000000 pyvserv-1.0.6/pyvcommon/comline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.6/pyvcommon/crysupp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.6/pyvcommon/genstrerr.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17642 2024-04-08 08:14:28.000000 pyvserv-1.0.6/pyvcommon/pyclisup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.6/pyvcommon/pycrypt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6778 2024-04-11 23:55:27.000000 pyvserv-1.0.6/pyvcommon/pydata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29729 2024-05-04 15:30:03.000000 pyvserv-1.0.6/pyvcommon/pyservsup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.6/pyvcommon/pysyslog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.6/pyvcommon/pyv2fa.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10878 2024-04-22 16:13:09.000000 pyvserv-1.0.6/pyvcommon/pyvhash.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.6/pyvcommon/pywrap.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9529 2024-04-15 10:48:15.000000 pyvserv-1.0.6/pyvcommon/support.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvgui/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:37.000000 pyvserv-1.0.6/pyvgui/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.143934 pyvserv-1.0.6/pyvgui/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    11912 2024-05-03 10:03:11.000000 pyvserv-1.0.6/pyvgui/docs/pyvcpanel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11223 2024-05-03 10:03:07.000000 pyvserv-1.0.6/pyvgui/docs/pyvservui.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11883 2024-05-03 10:03:10.000000 pyvserv-1.0.6/pyvgui/docs/pyvtally.html
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.147934 pyvserv-1.0.6/pyvgui/guilib/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:46.000000 pyvserv-1.0.6/pyvgui/guilib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    19985 2024-05-03 08:59:03.000000 pyvserv-1.0.6/pyvgui/guilib/config.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1718 2024-05-01 16:45:09.000000 pyvserv-1.0.6/pyvgui/guilib/entry_color.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    32884 2024-05-03 08:34:42.000000 pyvserv-1.0.6/pyvgui/guilib/mainballot.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14685 2024-05-03 09:05:10.000000 pyvserv-1.0.6/pyvgui/guilib/mainwin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    28844 2024-05-03 08:21:52.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinpeople.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13140 2024-05-02 17:09:41.000000 pyvserv-1.0.6/pyvgui/guilib/mainwintally.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    33945 2024-05-03 08:44:59.000000 pyvserv-1.0.6/pyvgui/guilib/mainwinvote.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12769 2024-05-01 11:17:04.000000 pyvserv-1.0.6/pyvgui/guilib/passdlg.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10836 2024-04-29 14:32:40.000000 pyvserv-1.0.6/pyvgui/guilib/pgcal.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.6/pyvgui/guilib/pgui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.6/pyvgui/guilib/pymenu.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    30364 2024-05-03 07:01:14.000000 pyvserv-1.0.6/pyvgui/guilib/recsel.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     6002 2024-05-01 10:13:15.000000 pyvserv-1.0.6/pyvgui/pyvballot.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4314 2024-04-30 13:08:04.000000 pyvserv-1.0.6/pyvgui/pyvballot.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3108 2024-05-03 09:01:56.000000 pyvserv-1.0.6/pyvgui/pyvcpanel.py
+-rw-r--r--   0 peterglen  (1000) users      (100)    14408 2024-05-01 09:57:52.000000 pyvserv-1.0.6/pyvgui/pyvpeople.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4320 2024-05-01 07:37:40.000000 pyvserv-1.0.6/pyvgui/pyvpeople.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2687 2024-05-03 09:28:18.000000 pyvserv-1.0.6/pyvgui/pyvservui.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3093 2024-05-02 17:03:45.000000 pyvserv-1.0.6/pyvgui/pyvtally.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     9831 2024-04-26 07:01:28.000000 pyvserv-1.0.6/pyvgui/pyvvote.png
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4316 2024-04-30 06:47:34.000000 pyvserv-1.0.6/pyvgui/pyvvote.py
+-rw-r--r--   0 peterglen  (1000) users      (100)     8794 2024-04-26 07:12:36.000000 pyvserv-1.0.6/pyvgui/pyvvote_sub.png
+-rw-r--r--   0 peterglen  (1000) users      (100)    80291 2024-04-17 01:51:25.000000 pyvserv-1.0.6/pyvgui/vote.png
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvserv.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)     3855 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)      732 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/requires.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-05-04 15:30:18.000000 pyvserv-1.0.6/pyvserv.egg-info/top_level.txt
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.151934 pyvserv-1.0.6/pyvserver/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:41.000000 pyvserv-1.0.6/pyvserver/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.151934 pyvserv-1.0.6/pyvserver/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)   171300 2024-04-15 06:32:07.000000 pyvserv-1.0.6/pyvserver/docs/pyvfunc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    76482 2024-04-15 06:32:05.000000 pyvserv-1.0.6/pyvserver/docs/pyvreplic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    68036 2024-04-15 06:32:04.000000 pyvserv-1.0.6/pyvserver/docs/pyvserv.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    35380 2024-04-15 06:32:06.000000 pyvserv-1.0.6/pyvserver/docs/pyvstate.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)    67566 2024-04-15 10:22:32.000000 pyvserv-1.0.6/pyvserver/pyvfunc.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    23259 2024-04-15 06:31:36.000000 pyvserv-1.0.6/pyvserver/pyvreplic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    22417 2024-04-15 05:56:51.000000 pyvserv-1.0.6/pyvserver/pyvserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14128 2024-04-15 10:48:53.000000 pyvserv-1.0.6/pyvserver/pyvstate.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvtools/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:20.000000 pyvserv-1.0.6/pyvtools/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-05-04 15:30:18.155934 pyvserv-1.0.6/pyvtools/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    16315 2024-05-03 10:03:06.000000 pyvserv-1.0.6/pyvtools/docs/pyvgenkey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10283 2024-05-03 10:03:05.000000 pyvserv-1.0.6/pyvtools/docs/pyvgenkeys.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.6/pyvtools/pyvgenkey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2508 2024-04-09 08:30:16.000000 pyvserv-1.0.6/pyvtools/pyvgenkeys.py
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-05-04 15:30:18.155934 pyvserv-1.0.6/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5787 2024-05-04 15:28:16.000000 pyvserv-1.0.6/setup.py
```

### Comparing `pyvserv-1.0.4/LICENSE` & `pyvserv-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/PKG-INFO` & `pyvserv-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.4
+Version: 1.0.6
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvserv-1.0.4/README.md` & `pyvserv-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_acc.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_acc.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_akey.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_akey.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_bigget.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_bigget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_cd.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_cd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_cli.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_cli.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_fdel.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_fdel.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_fget.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_fget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_file.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_file.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_fman.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_fman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_fput.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_fput.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_gethelp.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_gethelp.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_hello.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_hello.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_id.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_id.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_ihost.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_ihost.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_login.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_login.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_ls.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_ls.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_lsd.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_lsd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_mkdir.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_mkdir.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_pass.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_pass.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_ping.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_ping.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_qr.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_qr.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rabs.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rabs.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rcheck.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rcheck.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rcount.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rcount.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_replic.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_replic.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rget.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rget.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rlist.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rlist.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rman.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rmdir.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rmdir.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_rput.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_rput.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_sess.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_sess.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_sess_tout.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_sess_tout.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_throt.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_throt.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_tout.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_tout.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_uadd.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_uadd.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_uchpass.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_uchpass.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_udel.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_udel.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_uena.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_uena.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_uini.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_uini.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_uman.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_uman.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/docs/pyvcli_ver.html` & `pyvserv-1.0.6/pyvclient/docs/pyvcli_ver.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/loadtest.py` & `pyvserv-1.0.6/pyvclient/loadtest.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_akey.py` & `pyvserv-1.0.6/pyvclient/pyvcli_akey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_bigget.py` & `pyvserv-1.0.6/pyvclient/pyvcli_bigget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_cd.py` & `pyvserv-1.0.6/pyvclient/pyvcli_cd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_cli.py` & `pyvserv-1.0.6/pyvclient/pyvcli_cli.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_fdel.py` & `pyvserv-1.0.6/pyvclient/pyvcli_fdel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_fget.py` & `pyvserv-1.0.6/pyvclient/pyvcli_fget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_file.py` & `pyvserv-1.0.6/pyvclient/pyvcli_file.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_fman.py` & `pyvserv-1.0.6/pyvclient/pyvcli_fman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_fput.py` & `pyvserv-1.0.6/pyvclient/pyvcli_fput.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_gethelp.py` & `pyvserv-1.0.6/pyvclient/pyvcli_gethelp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_hello.py` & `pyvserv-1.0.6/pyvclient/pyvcli_hello.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_id.py` & `pyvserv-1.0.6/pyvclient/pyvcli_id.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_ihost.py` & `pyvserv-1.0.6/pyvclient/pyvcli_ihost.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_login.py` & `pyvserv-1.0.6/pyvclient/pyvcli_login.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_ls.py` & `pyvserv-1.0.6/pyvclient/pyvcli_ls.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_lsd.py` & `pyvserv-1.0.6/pyvclient/pyvcli_lsd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_mkdir.py` & `pyvserv-1.0.6/pyvclient/pyvcli_mkdir.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_pass.py` & `pyvserv-1.0.6/pyvclient/pyvcli_pass.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_ping.py` & `pyvserv-1.0.6/pyvclient/pyvcli_ping.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_qr.py` & `pyvserv-1.0.6/pyvclient/pyvcli_qr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rabs.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rabs.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rcheck.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rcheck.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rcount.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rcount.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_replic.py` & `pyvserv-1.0.6/pyvclient/pyvcli_replic.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rget.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rget.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rlist.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rlist.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rman.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rmdir.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rmdir.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_rput.py` & `pyvserv-1.0.6/pyvclient/pyvcli_rput.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_sess.py` & `pyvserv-1.0.6/pyvclient/pyvcli_sess.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_throt.py` & `pyvserv-1.0.6/pyvclient/pyvcli_throt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_uadd.py` & `pyvserv-1.0.6/pyvclient/pyvcli_uadd.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_uchpass.py` & `pyvserv-1.0.6/pyvclient/pyvcli_uchpass.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_udel.py` & `pyvserv-1.0.6/pyvclient/pyvcli_udel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_uena.py` & `pyvserv-1.0.6/pyvclient/pyvcli_uena.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_uini.py` & `pyvserv-1.0.6/pyvclient/pyvcli_uini.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_uman.py` & `pyvserv-1.0.6/pyvclient/pyvcli_uman.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvclient/pyvcli_ver.py` & `pyvserv-1.0.6/pyvclient/pyvcli_ver.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/comline.py` & `pyvserv-1.0.6/pyvcommon/comline.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/crysupp.py` & `pyvserv-1.0.6/pyvcommon/crysupp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/genstrerr.py` & `pyvserv-1.0.6/pyvcommon/genstrerr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pyclisup.py` & `pyvserv-1.0.6/pyvcommon/pyclisup.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pycrypt.py` & `pyvserv-1.0.6/pyvcommon/pycrypt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pydata.py` & `pyvserv-1.0.6/pyvcommon/pydata.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pyservsup.py` & `pyvserv-1.0.6/pyvcommon/pyservsup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 #from Crypto.Hash import SHA512
 from Crypto.Hash import SHA256
 from Crypto import Random
 
 # Globals and configurables
 
 # Update it here from setup
-version = "1.0.4"
+VERSION = "1.0.6"
 
 # Actions
 USER_AUTH  = 0;  USER_ADD = 1;   USER_DEL = 2;   USER_CHPASS = 3;
 USER_CHMOD = 4;
 
 # Permissions
 PERM_NONE = 0;  PERM_INI = 1;   PERM_ADMIN = 2;   PERM_DIS = 4;
```

### Comparing `pyvserv-1.0.4/pyvcommon/pysyslog.py` & `pyvserv-1.0.6/pyvcommon/pysyslog.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pyv2fa.py` & `pyvserv-1.0.6/pyvcommon/pyv2fa.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pyvhash.py` & `pyvserv-1.0.6/pyvcommon/pyvhash.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/pywrap.py` & `pyvserv-1.0.6/pyvcommon/pywrap.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvcommon/support.py` & `pyvserv-1.0.6/pyvcommon/support.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvgui/guilib/mainwin.py` & `pyvserv-1.0.6/pyvgui/guilib/mainwin.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
 from pyvguicom import pgbox
 from pyvguicom import pgsimp
-from pyvguicom import sutil
 from pyvguicom import pggui
+from pyvguicom import pgutils
 
 from pymenu import  *
 from pgui import  *
 
 from pyvcommon import pydata, pyservsup,  crysupp
 from pydbase import twinchain
 
@@ -349,15 +349,15 @@
                 aa = self.replog_fp.readline()
                 if not aa:
                     break
                 aa = aa.strip()
                 #print(aa)
                 bb = aa.split()
                 self.tree2.append([bb[0], bb[1], bb[2], " ".join(bb[3:]) ])
-                sutil.usleep(10)
+                pgutils.usleep(10)
                 got = True
 
             if got:
                 self.tree2.sel_last()
                 self.led3.set_color("00ff00")
                 GLib.timeout_add(400, self.led_off, self.led3, "#888888")
 
@@ -380,15 +380,15 @@
                 aa = self.log_fp.readline()
                 if not aa:
                     break
                 aa = aa.strip()
                 #print(aa)
                 bb = aa.split()
                 self.tree1.append([bb[0], bb[1], bb[2], " ".join(bb[3:]) ])
-                sutil.usleep(10)
+                pgutils.usleep(10)
                 got = True
 
             if got:
                 self.tree1.sel_last()
                 self.led1.set_color("00ff00")
                 GLib.timeout_add(400, self.led_off, self.led1, "#888888")
```

### Comparing `pyvserv-1.0.4/pyvgui/guilib/mainwinserv.py` & `pyvserv-1.0.6/pyvgui/guilib/mainwinserv.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvgui/guilib/mainwintally.py` & `pyvserv-1.0.6/pyvgui/guilib/mainwintally.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
 from gi.repository import Pango
 
 from pyvguicom import pgbox
 from pyvguicom import pgsimp
-from pyvguicom import sutil
+#from pyvguicom import sutil
 from pyvguicom import pggui
 
 from pymenu import  *
 from pgui import  *
 
 from pyvcommon import pydata, pyservsup,  crysupp
 from pydbase import twinchain
@@ -77,20 +77,21 @@
 
         self.connect("destroy", self.OnExit)
         self.connect("key-press-event", self.key_press_event)
         self.connect("button-press-event", self.button_press_event)
 
         self.oldtally = [0,0,0,0,0,0,0,0,0,0,0,]
 
+        numofcols = 8
         self.tally = []
-        for aa in range(11):
+        for aa in range(numofcols):
             self.tally.append(0)
 
         self.untally = []
-        for aa in range(11):
+        for aa in range(numofcols):
             self.untally.append(0)
 
         try:
             self.set_icon_from_file("icon.png")
         except:
             pass
 
@@ -176,37 +177,37 @@
             cntf += 1
 
         hbox3.pack_start(self.tree1s, True, True, 6)
         vbox.pack_start(hbox3, True, True, 2)
 
         self.tallyarr = []
         hbox5 = Gtk.HBox()
-        for aa in range(10):
+        for aa in range(numofcols):
             vbox_1 = Gtk.VBox()
-            vbox_1.pack_start(Gtk.Label("Tally %s" % aa), 1, 1, 2)
+            vbox_1.pack_start(Gtk.Label("Tally %s" % (aa+1)), 1, 1, 2)
             self.tallyarr.append(Gtk.Label("0"))
             vbox_1.pack_start(self.tallyarr[aa], 1, 1, 2)
             hbox5.pack_start(vbox_1, 1, 1,2)
         vbox.pack_start(hbox5, False, 0, 2)
 
         self.untallyarr = []
         hbox6 = Gtk.HBox()
-        for aa in range(10):
+        for aa in range(numofcols):
             vbox_1 = Gtk.VBox()
-            vbox_1.pack_start(Gtk.Label("Un %s" % aa), 1, 1, 2)
+            vbox_1.pack_start(Gtk.Label("Un %s" % (aa+1)), 1, 1, 2)
             self.untallyarr.append(Gtk.Label("0"))
             vbox_1.pack_start(self.untallyarr[aa], 1, 1, 2)
             hbox6.pack_start(vbox_1, 1, 1,2)
         vbox.pack_start(hbox6, False, 0, 2)
 
         self.sumarr = []
         hbox7 = Gtk.HBox()
-        for aa in range(10):
+        for aa in range(numofcols):
             vbox_1 = Gtk.VBox()
-            vbox_1.pack_start(Gtk.Label("Sum %s" % aa), 1, 1, 2)
+            vbox_1.pack_start(Gtk.Label("Sum %s" % (aa+1)), 1, 1, 2)
             self.sumarr.append(Gtk.Label("0"))
             vbox_1.pack_start(self.sumarr[aa], 1, 1, 2)
             hbox7.pack_start(vbox_1, 1, 1,2)
         vbox.pack_start(hbox7, False, 0, 2)
 
         vbox.pack_start(hbox4, False, 0, 6)
 
@@ -286,23 +287,23 @@
                     #print("dec", dec)
                     decpay  = pb.decode_data(dec['payload'])[0]
                     pay = decpay['PayLoad']
                     #print("pay:", pay)
                     actstr = ["register", "unregister", "cast", "uncast", ]
                     if pay['Action'] == 'cast':
                         idx = int(decpay['PayLoad']['Vote'])
-                        if idx >= 11:
+                        if idx >= numofcols:
                             print("bad vote value", idx)
-                        self.tally[ idx % 11 ] += 1
+                        self.tally[ idx % numofcols ] += 1
 
                     if pay['Action'] == 'uncast':
                         idx = int(decpay['PayLoad']['Vote'])
-                        if idx >= 11:
+                        if idx >= numofcols:
                             print("bad unvote value", idx)
-                        self.untally[ idx % 11 ] += 1
+                        self.untally[ idx % numofcols ] += 1
                     arrx = [dec['header']]
                     for aaa in self.fields[1:]:
                         try:
                             arrx.append(str(pay[aaa]))
                         except:
                             print("Incomplete:", pay)
                     try:
```

### Comparing `pyvserv-1.0.4/pyvgui/guilib/mainwinvote.py` & `pyvserv-1.0.6/pyvgui/guilib/mainwinpeople.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 
-import os, sys, getopt, signal, random, time
-import string, warnings, uuid, datetime
+import os, sys, getopt, signal, random, time, base64
+import string, warnings, uuid, datetime, struct, io
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 from gi.repository import GLib
 from gi.repository import GObject
@@ -22,22 +22,24 @@
 from pyvguicom import pggui
 from pyvguicom import pgentry
 from pyvguicom import pgutils
 
 from pymenu import  *
 from pgui import  *
 
-import recsel, pgcal
+import recsel, pgcal, config, passdlg
 
 from pyvcommon import pydata, pyservsup,  pyvhash, crysupp
 
 from pydbase import twincore, twinchain
 
 import pyvpacker
 
+from Crypto.Cipher import AES
+
 alllett =   string.ascii_lowercase + string.ascii_uppercase
 
 def randascii(lenx):
 
     ''' Spew a lot of chars, simulate txt by add ' ' an '\n' '''
 
     strx = ""
@@ -50,32 +52,28 @@
         if random.randint(0x00, 12) == 10:
             strx += " "
     return strx
 
 def simname(lenx):
     strx = ""
     lenz = len(alllett)-1
-
     spidx = random.randint(0, lenx - 4)
     ridx = random.randint(0, len(string.ascii_uppercase)-1)
     strx += string.ascii_uppercase[ridx]
     for aa in range(spidx):
         ridx = random.randint(0, len(string.ascii_lowercase)-1)
         rr = string.ascii_lowercase[ridx]
         strx += str(rr)
-
     strx += " "
     ridx = random.randint(0, len(string.ascii_uppercase)-1)
     strx += string.ascii_uppercase[ridx]
-
     for aa in range(lenx - spidx):
         ridx = random.randint(0, len(string.ascii_lowercase)-1)
         rr = string.ascii_lowercase[ridx]
         strx += str(rr)
-
     return strx
 
 def randisodate():
     dd = datetime.datetime.now()
     dd = dd.replace(microsecond=0)
     return dd.isoformat()
 
@@ -91,39 +89,51 @@
 
     return dd.strftime("%Y/%m/%d")
 
 # ------------------------------------------------------------------------
 
 class MainWin(Gtk.Window):
 
-    def __init__(self):
+    def __init__(self, globals):
 
         Gtk.Window.__init__(self, Gtk.WindowType.TOPLEVEL)
 
-        try:
-            pixbuf = Gtk.IconTheme.get_default().load_icon("weather-storm", 32, 0)
-            self.set_icon(pixbuf)
-        except:
+        #print("globals", globals.myhome)
 
-            icon = os.path.join(os.path.dirname(__file__), "weather-storm.png")
-            ic = Gtk.Image(); ic.set_from_file(icon)
+        self.powers     = 0
+        self.conf       = globals.conf
+        self.conf.iconf  = os.path.dirname(globals.conf.me) + os.sep + "pyvpeople.png"
+        self.conf.iconf2 = os.path.dirname(globals.conf.me) + os.sep + "pyvvote_sub.png"
+        self.conf.siteid = globals.siteid
+        try:
+            #print("iconf", self.conf.iconf)
+            ic = Gtk.Image(); ic.set_from_file(self.conf.iconf)
             self.set_icon(ic.get_pixbuf())
+        except:
+            pass
 
         self.start_anal = False
-        self.core = None
-        self.in_timer = False
+        #self.core = None
         self.cnt = 0
         self.old_sss = 1
-        self.status_cnt = 0
-        self.set_title("PyVServer Voter Entry")
+        self.set_title("PyVServer Client Entry")
         self.set_position(Gtk.WindowPosition.CENTER_ALWAYS)
         self.packer = pyvpacker.packbin()
         self.vcore = twincore.TwinCore("voters.pydb", 0)
+        self.acore = twincore.TwinCore("audit.pydb", 0)
+        self.authcore = twincore.TwinCore("auth.pydb", 0)
+
+        # We let the core carry vars; make sure they do not collide
+        self.vcore.packer = self.packer
+        self.vcore.hashname  = os.path.splitext(self.vcore.fname)[0] + ".hash.id"
+        self.vcore.hashname2 = os.path.splitext(self.vcore.fname)[0] + ".hash.name"
+
         self.exit_flag = 0
         self.stop = True
+
         #ic = Gtk.Image(); ic.set_from_stock(Gtk.STOCK_DIALOG_INFO, Gtk.ICON_SIZE_BUTTON)
         #window.set_icon(ic.get_pixbuf())
 
         www = Gdk.Screen.width(); hhh = Gdk.Screen.height();
 
         disp2 = Gdk.Display()
         disp = disp2.get_default()
@@ -135,15 +145,15 @@
         www = geo.width; hhh = geo.height
         xxx = geo.x;     yyy = geo.y
 
         # Resort to old means of getting screen w / h
         if www == 0 or hhh == 0:
             www = Gdk.screen_width(); hhh = Gdk.screen_height();
 
-        self.set_default_size(6*www/8, 6*hhh/8)
+        #self.set_default_size(6*www/8, 6*hhh/8)
 
         self.dat_dict = {}
         self.dat_dict_org = {}
 
         #if www / hhh > 2:
         #    self.set_default_size(5*www/8, 5*hhh/8)
         #else:
@@ -156,15 +166,40 @@
 
         try:
             self.set_icon_from_file("icon.png")
         except:
             pass
 
         vbox = Gtk.VBox()
-        hbox4 = Gtk.HBox()
+
+        hbox4a = Gtk.HBox()
+        butt2a = Gtk.Button.new_with_mnemonic(" Config_ure ")
+        butt2a.connect("clicked", self.config_dlg)
+        hbox4a.pack_start(Gtk.Label("   "), 0, 0, 0)
+
+        if globals.conf.testx:
+            #lab3 = Gtk.Label(" | ");
+            #hbox4a.pack_start(lab3, 0, 0, 0)
+            butt2 = Gtk.Button.new_with_mnemonic(" Te_zt generate data")
+            butt2.connect("clicked", self.test_data)
+            hbox4a.pack_start(butt2, 0, 0, 2)
+            #lab2 = Gtk.Label(" | ");
+            #hbox4a.pack_start(lab2, 0, 0, 0)
+
+        hbox4a.pack_start(Gtk.Label("   "), 1, 1, 0)
+        hbox4a.pack_start(butt2a, False, 0, 2)
+
+        butt2 = Gtk.Button.new_with_mnemonic(" Ne_w entry ")
+        butt2.connect("clicked", self.new_data)
+        hbox4a.pack_start(butt2, False, 0, 2)
+
+        butt2 = Gtk.Button.new_with_mnemonic(" Dele_te entry ")
+        butt2.connect("clicked", self.del_data)
+        hbox4a.pack_start(butt2, False, 0, 2)
+        hbox4a.pack_start(Gtk.Label("   "), 0, 0, 2)
 
         merge = Gtk.UIManager()
         #self.mywin.set_data("ui-manager", merge)
 
         aa = create_action_group(self)
         merge.insert_action_group(aa, 0)
         self.add_accel_group(merge.get_accel_group())
@@ -181,94 +216,41 @@
         #self.tbar = merge.get_widget("/ToolBar");
         #self.tbar.show()
         #bbox = Gtk.VBox()
         #bbox.pack_start(self.mbar, 0,0, 0)
         #bbox.pack_start(self.tbar, 0,0, 0)
         #vbox.pack_start(bbox, False, 0, 0)
 
+        hbox4 = Gtk.HBox()
         lab1 = Gtk.Label("   ");
         hbox4.pack_start(lab1, 0, 0, 0)
-        lab2a = Gtk.Label(" Initializing ");
+        lab2a = Gtk.Label(" Initializing ...");
         hbox4.pack_start(lab2a, 1, 1, 0)
         lab2a.set_xalign(0)
-        lab2a.set_size_request(300, -1)
+        lab2a.set_size_request(150, -1)
 
-        self.status = lab2a
-        self.status_cnt = 1
+        self.status = recsel.Status()
 
         lab1 = Gtk.Label(" ");
         hbox4.pack_start(lab1, 1, 1, 0)
 
-        lab2 = Gtk.Label(" | ");
-        hbox4.pack_start(lab2, 0, 0, 0)
-
-        butt2 = Gtk.Button.new_with_mnemonic(" Te_zt ")
-        butt2.connect("clicked", self.test_data)
-        hbox4.pack_start(butt2, False, 0, 4)
-
-        lab3 = Gtk.Label(" | ");
-        hbox4.pack_start(lab3, 0, 0, 0)
-
-        butt2 = Gtk.Button.new_with_mnemonic(" Dele_te entry ")
-        butt2.connect("clicked", self.del_data)
-        hbox4.pack_start(butt2, False, 0, 4)
-
-        butt2 = Gtk.Button.new_with_mnemonic(" Ne_w entry ")
-        butt2.connect("clicked", self.new_data)
-        hbox4.pack_start(butt2, False, 0, 4)
+        butt1 = Gtk.Button.new_with_mnemonic(" _Save entry ")
+        butt1.connect("clicked", self.save_data)
+        hbox4.pack_start(butt1, False, 0, 2)
 
         butt3 = Gtk.Button.new_with_mnemonic(" Lo_ad entry ")
         butt3.connect("clicked", self.load_data)
-        hbox4.pack_start(butt3, False, 0, 4)
-
-        butt1 = Gtk.Button.new_with_mnemonic(" _Save entry ")
-        butt1.connect("clicked", self.save_data)
-        hbox4.pack_start(butt1, False, 0, 4)
+        hbox4.pack_start(butt3, False, 0, 2)
 
-        butt2 = Gtk.Button.new_with_mnemonic(" E_xit ")
+        butt2 = Gtk.Button.new_with_mnemonic("     E_xit    ")
         butt2.connect("clicked", self.OnExit, self)
-        hbox4.pack_start(butt2, False, 0, 4)
+        hbox4.pack_start(butt2, False, 0, 2)
 
         lab2 = Gtk.Label("   ");  hbox4.pack_start(lab2, 0, 0, 0)
 
-        #hbox2 = Gtk.HBox()
-        #lab3 = Gtk.Label("");  hbox2.pack_start(lab3, 0, 0, 0)
-        #lab4 = Gtk.Label("");  hbox2.pack_start(lab4, 0, 0, 0)
-        #vbox.pack_start(hbox2, False, 0, 0)
-
-        #self.edit1 = pgsimp.SimpleEdit();
-
-        # This is what is coming in:
-        #{'Default': 'None', 'Vote': 4,
-        #'UID': '64839bff-fae7-11ee-bb58-0fa03c52389e',
-        #'SubVote': 6, 'TUID': '64839c00-fae7-11ee-bb58-0fa03c52389e',
-        # 'Action': 'register', 'RUID': '64839c01-fae7-11ee-bb58-0fa03c52389e',
-        #  'Test': 'test'}
-
-        # Field names (set positional displays except header)
-        self.fields = \
-        ("Header", "Action", "Vote", "SubVote", "UID", "RUID",
-            "TUID", )
-        #  "Test", "Default")
-
-        tt = type(""); fff = []
-        for ccc in range(len(self.fields)):
-            fff.append(tt)
-        self.model = Gtk.TreeStore(*fff)
-
-        #self.tree1s, self.tree1 = self.wrap(Gtk.TreeView(self.model))
-        #self.cells = []; cntf = 0
-        #for aa in self.fields:
-        #    col = Gtk.TreeViewColumn(aa, self.cellx(cntf), text=cntf)
-        #    col.set_resizable(True)
-        #    self.tree1.append_column(col)
-        #    cntf += 1
-        #hbox3.pack_start(self.tree1s, True, True, 6)
-
-        #sg = Gtk.SizeGroup(Gtk.SizeGroupMode.HORIZONTAL)
         gridx = Gtk.Grid()
         gridx.set_column_spacing(6)
         gridx.set_row_spacing(6)
 
         #gridx.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaaaa"))
 
         rowcnt = 0
@@ -288,82 +270,92 @@
         tp3 = ("Location of birth: ", "lob", "Location: City / Country", None)
         tp4 = ("Nick Name: ", "nick", "Enter nick name / Alias if available", None)
         lab3, lab4 = pgentry.gridquad(gridx, 0, rowcnt, tp3, tp4)
         self.dat_dict['lob'] = lab3
         self.dat_dict['nick'] = lab4
         rowcnt += 1
 
-        gridx.attach(self.vspacer(8), 0, rowcnt, 1, 1)
+        gridx.attach(pggui.ySpacer(8), 0, rowcnt, 1, 1)
         rowcnt += 1
 
-        tp3x = ("UUID: ", "uuid", "Generate VOTER UID by pressing button", None)
+        tp3x = ("User / Client UUID: ", "uuid", "Generate Client UID by pressing button", None)
         butt1 = Gtk.Button.new_with_mnemonic("Gene_rate")
         lab3x = pgentry.griddouble(gridx, 0, rowcnt, tp3x, butt1)
-        butt1.connect("clicked", self.pressed_uuid, lab3x)
+        butt1.connect("clicked", self.load_uuid, lab3x)
         self.dat_dict['uuid'] = lab3x
         rowcnt += 1
 
-        tp4x = ("GUID: ", "guid", "Load GROUP UID by pressing button", None)
-        butt2 = Gtk.Button.new_with_mnemonic("Loa_d")
+        tp4x = ("Site UUID: ", "guid", "Group / Site UID", None)
+        butt2 = Gtk.Button.new_with_mnemonic("Load")
         lab4x = pgentry.griddouble(gridx, 0, rowcnt, tp4x, butt2)
-        butt2.connect("clicked", self.load_uuid, lab4x)
+        butt2.connect("clicked", self.load_site_uuid, lab4x)
         self.dat_dict['guid'] = lab4x
         rowcnt += 1
-        gridx.attach(self.vspacer(8), 0, rowcnt, 1, 1)
+
+        tp6x = ("Operator UUID: ", "guid", "Operator UUID", None)
+        butt2 = Gtk.Button.new_with_mnemonic("Load")
+        lab6x = pgentry.griddouble(gridx, 0, rowcnt, tp6x, butt2)
+        butt2.connect("clicked", self.load_op_uuid, lab6x)
+        self.dat_dict['ouid'] = lab6x
+        rowcnt += 1
+        gridx.attach(pggui.ySpacer(8), 0, rowcnt, 1, 1)
         rowcnt += 1
 
         tp3a = ("Address Line 1: ", "addr1", "Address line one. (Number, Street)", None)
-        tp4a = ("Address Line 2: ", "addr2", "Addressline two. (if applicable)", None)
+        tp4a = ("Address Line 2: ", "addr2", "Address line two. (if applicable)", None)
         lab5, lab6 = pgentry.gridquad(gridx, 0, rowcnt, tp3a, tp4a)
         self.dat_dict['addr1'] = lab5
         self.dat_dict['addr2'] = lab6
         rowcnt += 1
 
         tp5 = ("City: ", "city", "City or Township", None)
-        tp6 = ("State / Territory: ", "county", "County or Teritory or Borough", None)
+        tp6 = ("State / Territory: ", "county", "State / County / Teritory / Borough", None)
         lab7, lab8 = pgentry.gridquad(gridx, 0, rowcnt, tp5, tp6)
         self.dat_dict['city'] = lab7
         self.dat_dict['terr'] = lab8
         rowcnt += 1
 
         tp7 = ("Zip: ", "zip", "Zip code or Postal code", None)
-        tp8 = ("Country: ", "country", "Coutry of residence", None)
+        tp8 = ("Country: ", "country", "Country of residence", None)
         lab9, lab10 = pgentry.gridquad(gridx, 0, rowcnt, tp7, tp8)
         self.dat_dict['zip'] = lab9
         self.dat_dict['country'] = lab10
         rowcnt += 1
 
         tp7a = ("Phone: ", "phone", "Phone or text number. ", None)
         tp8a = ("Email: ", "email", "Primary Email", None)
         lab11, lab12 = pgentry.gridquad(gridx, 0, rowcnt, tp7a, tp8a)
         self.dat_dict['phone'] = lab11
         self.dat_dict['email'] = lab12
         rowcnt += 1
 
-        tp7b = ("Phone: (secondary)", "phone2", "Secondary phone or text number. ", None)
+        tp7b = ("Phone: (Secondary)", "phone2", "Secondary phone or text number. ", None)
         tp8b = ("Email: (Secondary)", "email2", "Secondary Email, if available: Ex: whatsapp", None)
         lab13, lab14 = pgentry.gridquad(gridx, 0, rowcnt, tp7b, tp8b)
         self.dat_dict['phone2'] = lab13
         self.dat_dict['email2'] = lab14
         rowcnt += 1
 
+        butt2o = Gtk.Button.new_with_mnemonic("Load")
         tp9b = ("Now: (date of entry)"," ",  "Autofilled, date of entry", None)
         tp10b = ("Operator:", " ", "Operator, who entered this record.", None)
-        lab15, lab16 = pgentry.gridquad(gridx, 0, rowcnt, tp9b, tp10b)
+        lab15, lab16 = pgentry.gridquad(gridx, 0, rowcnt, tp9b, tp10b, butt2o)
+        butt2o.connect("clicked", self.load_op_name, lab16, lab15)
+
         self.dat_dict['now'] = lab15
         self.dat_dict['oper'] = lab16
         rowcnt += 1
 
         tp6x = ("Notes: ", "", "Text for Notes. Press Shift Enter to advance", None)
         lab6x = pgentry.gridsingle(gridx, 0, rowcnt, tp6x)
         self.dat_dict['notes'] = lab6x
         rowcnt += 1
 
-        gridx.attach(self.vspacer(8), 0, rowcnt, 1, 1)
-        rowcnt += 1
+        #gridx.attach(pggui.ySpacer(8), 0, rowcnt, 1, 1)
+        #rowcnt += 1
 
         #tp7b = ("Vote:" , "", "Voting entity. ", None)
         #tp8b = ("Secondary Vote", "", "Secondary Entity", None)
         #lab13, lab14 = gridquad(gridx, 0, rowcnt, tp7b, tp8b, butt)
         #self.dat_dict['vote'] = lab13
         #self.dat_dict['vote2'] = lab14
         #rowcnt += 1
@@ -377,40 +369,78 @@
         #hboxtop = Gtk.HBox()
         #hboxtop.pack_start(Gtk.Label(" "),  0, 0, 2)
         #hboxtop.pack_start(Gtk.Label("Not all enrties are required: "),  0, 0, 6)
         #hboxtop.pack_start(Gtk.Label(" "),  1, 1, 2)
         ##hboxtop.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaa44"))
         #vbox.pack_start(hboxtop, 0, 0, 0)
 
+        #pggui.set_testmode(1)
+        vbox.pack_start(pggui.ySpacer(4), 0, 0, 0)
+
+        #sumx.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaaaa"))
+        sumx.pack_start(Gtk.Label("   "), 0, 0, 0)
+        sumx.pack_start(gridx, 1, 1, 0)
         sumx.pack_start(Gtk.Label("   "), 0, 0, 0)
-        sumx.pack_start(gridx, 0, 0, 0)
-        sumx.pack_start(Gtk.Label("   "), 1, 1, 0)
+
+        #vbox.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaaff"))
 
         vbox.pack_start(sumx, 1, 1, 2)
         #sumx.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaa88"))
 
-        #fill = Gtk.VBox()
-        #vbox.pack_start(fill, 0, 0, 2)
-
-        #hbox3 = Gtk.HBox()
-        #hbox3.pack_start(Gtk.Label("q"),1,1,0)
-        #hbox3.modify_bg(Gtk.StateType.NORMAL, Gdk.color_parse("#aaaaaa"))
-        #vbox.pack_start(hbox3, 0, 0, 2)
-
-        vbox.pack_start(hbox4, False, 0, 4)
+        vbox.pack_start(hbox4a, False, 0, 2)
+        vbox.pack_start(hbox4, False, 0, 2)
 
         self.add(vbox)
         self.show_all()
+        self.en_dis_all(False)
+
+        GLib.timeout_add(100, self.start_pass_dlg, 0)
+
+    def config_dlg(self, arg2):
+        #print("config_dlg")
+        #print("pass pow:", self.powers)
+        if self.powers != "Yes":
+            pggui.message("Only Admin can Configure.")
+        else:
+            config.ConfigDlg(self.vcore, self.acore, self.authcore, self.conf)
+
+    def start_pass_dlg(self, arg2):
 
-        GLib.timeout_add(1000, self.timer)
+        authcnt = 0
+        while True:
+            if authcnt > 3:
+                pggui.message("Too May tries, exiting.")
+                sys.exit(1)
+            ret = passdlg.auth_initial(self.authcore, self.packer, self.conf)
+            #print("ret:", ret)
+            if not ret[0]:
+                authcnt += 1
+                continue
+            if ret[1][2] != "Enabled":
+                authcnt += 1
+                msg = "Cannot log in, user '%s' is disbled " % ret[1][0]
+                self.status.set_status_text(msg)
+                pggui.message(msg)
+                continue
+            # Success
+            self.operator = ret[1][0]
+            self.powers   = ret[1][4]
+            self.ouid     = ret[1][5]
+            #print("pow", self.powers, self.operator, self.ouid)
+            self.status.set_status_text("Authenticated '%s'" % ret[1][0])
+            self.en_dis_all(True)
+            recsel.audit(self.acore, self.packer, "Successful Login", ret[1][0])
+            break
+
+        self.set_focus(self.dat_dict['name'])
 
-    def vspacer(self, sp):
-        hbox = Gtk.HBox()
-        hbox.set_size_request(sp, sp)
-        return hbox
+    def en_dis_all(self, flag):
+
+        for aa in self.dat_dict.keys():
+            self.dat_dict[aa].set_sensitive(flag)
 
     def is_changed(self):
         ccc = False
         for aa in self.dat_dict.keys():
             if self.dat_dict_org[aa] != self.dat_dict[aa].get_text():
                 ccc = True
         return ccc
@@ -440,32 +470,49 @@
         #print("res:", result)
 
         #result[1][1] += 1
 
         arg2.set_text(str(result[1][0]) + "/" + str(result[1][1]) + \
                             "/" + str(result[1][2]))
 
-    def pressed_uuid(self, arg, arg2):
+    def load_op_name(self, arg, arg2, arg3):
         if arg2.get_text() != "":
-            msg = "Already has a UUID; Cannot set."
+            msg = "Already has operator; Cannot set."
             pggui.message(msg)
-            self.status.set_text(msg)
-            self.status_cnt = 5
+            self.status.set_status_text(msg)
             return
-        arg2.set_text(str(uuid.uuid1()))
+        arg2.set_text(self.operator)
+        #if arg3.get_text() == "":
+        dd = datetime.datetime.now()
+        dd = dd.replace(microsecond=0)
+        arg3.set_text(dd.isoformat())
 
     def load_uuid(self, arg, arg2):
         if arg2.get_text() != "":
             msg = "Already has a GUID; Cannot set."
             pggui.message(msg)
-            self.status.set_text(msg)
-            self.status_cnt = 5
+            self.status.set_status_text(msg)
             return
         arg2.set_text(str(uuid.uuid1()))
 
+    def load_op_uuid(self, arg, arg2):
+        if arg2.get_text() != "":
+            msg = "Already has a OUID; Cannot set."
+            pggui.message(msg)
+            self.status.set_status_text(msg)
+            return
+        arg2.set_text(self.ouid)
+
+    def load_site_uuid(self, arg, arg2):
+        if arg2.get_text() != "":
+            msg = "Already has a Site UUID; Cannot set."
+            pggui.message(msg)
+            self.status.set_status_text(msg)
+            return
+        arg2.set_text(str(self.conf.siteid))
 
     def cellx(self, idx):
         cell = Gtk.CellRendererText()
 
         #if centered[idx]:
         #    cell.set_property("alignment", Pango.Alignment.CENTER)
         #    cell.set_property("align-set", True)
@@ -521,130 +568,140 @@
         ''' Reset flags for changed dict '''
 
         for aa in self.dat_dict.keys():
             self.dat_dict_org[aa] = self.dat_dict[aa].get_text()
 
     def del_data(self, arg):
 
+        ''' Delete currently active data '''
+
         nnn = self.dat_dict['name'].get_text()
         if not nnn:
             msg = "Empty record, cannot delete."
-            self.status.set_text(msg)
-            self.status_cnt = 4
+            self.status.set_status_text(msg)
             pggui.message(msg)
             return
         msg = "This will delete: '%s'. \nAre you sure?" % nnn
-        self.status.set_text(msg)
-        self.status_cnt = 4
-        ret = self.yesno(msg)
+        self.status.set_status_text(msg)
+        ret = pggui.yes_no(msg, default="No")
         if ret != Gtk.ResponseType.YES:
             return True
         ddd = self.dat_dict['uuid'].get_text()
-        #print("deleting:", ddd)
-        try:
-            dat = self.vcore.del_rec_bykey(ddd)
-            #print("dat:", dat)
-        except:
-            dat = []
-            print(sys.exc_info())
-            pass
-        self.status.set_text("Record '%s' deleted." % nnn)
-        self.status_cnt = 4
+        # Find it via index
+        ddd2 = recsel.search_index(self.vcore, self.vcore.hashname, ddd, recsel.hashid)
+        for aa in ddd2:
+            #print("deleting:", ddd2)
+            try:
+                rrr = self.vcore.get_rec(aa)
+                ret = self.vcore.del_rec(aa)
+                #print(aa, "del ret:", ret)
+                recsel.audit(self.acore, self.packer, "Deleted Record", rrr[1])
+                self.status.set_status_text("Record '%s' deleted." % nnn)
+            except:
+                print(sys.exc_info())
+
         # Clear, reset
         self.clear_data()
         self.reset_changed()
 
     def new_data(self, arg):
 
         # See if previous one saved
         ccc = False
         for aa in self.dat_dict.keys():
             if self.dat_dict_org[aa] != self.dat_dict[aa].get_text():
                 ccc = True
         if ccc:
             msg = "Unsaved data. Are you sure you want to abandon it?"
-            self.status.set_text(msg)
-            self.status_cnt = 4
-            ret = self.yesno(msg)
+            self.status.set_status_text(msg)
+            ret = pggui.yes_no(msg, default="No")
             if ret != Gtk.ResponseType.YES:
                 return True
 
         # Clear, reset
         for aa in self.dat_dict.keys():
             self.dat_dict[aa].set_text("")
 
         # Fill in defaults
         dd = datetime.datetime.now()
         dd = dd.replace(microsecond=0)
         self.dat_dict['now'].set_text(dd.isoformat())
         self.dat_dict['uuid'].set_text(str(uuid.uuid1()))
+        self.dat_dict['guid'].set_text(str(self.conf.siteid))
+        self.dat_dict['ouid'].set_text(str(self.ouid))
+        self.dat_dict['oper'].set_text(str(self.operator))
 
         self.reset_changed()
+        self.set_focus(self.dat_dict['name'])
 
     def load_data(self, arg):
 
         # See if previous one saved
         ccc = False
         for aa in self.dat_dict.keys():
             if self.dat_dict_org[aa] != self.dat_dict[aa].get_text():
                 ccc = True
         if ccc:
-            msg = "Please save current data before loading a new one."
-            self.status.set_text(msg)
-            self.status_cnt = 4
-            pggui.message(msg)
+            msg = "Please save data before loading a new record.\n" \
+                  "Current changes would be discarded. Are you sure?"
+            self.status.set_status_text(msg)
+            pggui.yes_no(msg, default="No")
             return
 
         # Clear, reset
         for aa in self.dat_dict.keys():
             self.dat_dict[aa].set_text("")
-
         self.reset_changed()
 
-        sss = recsel.RecSel(self.vcore)
+        sss = recsel.RecSelDlg(self.vcore, self.acore, self.conf)
         if sss.response != Gtk.ResponseType.ACCEPT:
             return
-
-        print("sss.res:", sss.res)
-
+        #print("sss.res:", sss.res)
         try:
-            dat = self.vcore.retrieve(sss.res[0][3])
+            # Slow ...
+            #dat = self.vcore.retrieve(sss.res[0][3])
+            # New data: abs. position added
+            #print("get_rec", int(sss.res[0][4]))
+            dat = self.vcore.get_rec(int(sss.res[0][4]))
         except:
             dat = []
             print(sys.exc_info())
             pass
         if not dat:
             msg = "No data selected."
             #print(msg)
-            self.status.set_text(msg)
-            self.status_cnt = 5
+            self.status.set_status_text(msg)
             pggui.message(msg)
             return
-
         #print("dat:", dat)
-        dec = self.packer.decode_data(dat[0][1])[0]
+        try:
+            # dec array[0] if retrieve
+            #dec = self.packer.decode_data(dat[1])[0]
+            # dec array if get_rec
+            dec = self.packer.decode_data(dat[1])[0]
+        except:
+            dec = {}
+            pass
         #print("dec:", dec)
         for aa in dec.keys():
             self.dat_dict[aa].set_text(dec[aa])
-
         # Mark as non changed
         self.reset_changed()
 
     def test_data(self, arg1):
 
         #print("test started")
         self.stop = not self.stop
         while True:
             if self.exit_flag:
                 self.reset_changed()
                 break
             if self.stop:
                 self.reset_changed()
-                self.status.set_text("Test Stopped")
-                self.status_cnt = 4
+                self.status.set_status_text("Test Stopped")
                 break
             for aa in self.dat_dict.keys():
                 # Handle differences
                 if aa == 'uuid':
                    self.dat_dict[aa].set_text(str(uuid.uuid1()) )
                 elif aa == 'name':
                    self.dat_dict[aa].set_text(simname(random.randint(12, 22)))
@@ -659,103 +716,110 @@
                 else:
                     self.dat_dict[aa].set_text(pgutils.randstr(random.randint(6, 22)))
             sleepx = 20
             pgutils.usleep(sleepx)
             self.save_data(0)
             self.clear_data()
 
+    def autofill(self, idxname, newid):
+        try:
+            uuu = uuid.UUID(self.dat_dict[idxname].get_text())
+        except:
+            self.dat_dict[idxname].set_text(str(newid))
+
     def save_data(self, arg1):
 
         # See if changed
         if not self.is_changed():
             msg = "Nothing changed, cannot save."
-            self.status.set_text(msg)
-            self.status_cnt = 4
+            self.status.set_status_text(msg)
             pggui.message(msg)
             return
 
         if not self.dat_dict['name'].get_text():
-            msg = "Must have a voter name."
-            self.status.set_text(msg)
-            self.status_cnt = 4
+            msg = "Must have a FULL name."
+            self.status.set_status_text(msg)
             self.set_focus(self.dat_dict['name'])
             pggui.message(msg)
             return
 
-        if not self.dat_dict['dob'].get_text():
-            msg = "Must have a voter date of birth."
-            self.status.set_text(msg)
-            self.status_cnt = 4
+        dob = self.dat_dict['dob'].get_text()
+        if not dob or len(dob.split("/")) < 3:
+            msg = "Must have a valid Client date of birth. (yyyy/mm/dd)"
+            self.status.set_status_text(msg)
             self.set_focus(self.dat_dict['dob'])
             pggui.message(msg)
             return
 
-        try:
-            uuu = uuid.UUID(self.dat_dict['uuid'].get_text())
-        except:
-            #print("Gen UUID", sys.exc_info())
-            msg = "Cannot save without a valid UUID"
-            self.status.set_text(msg)
-            self.status_cnt = 4
-            pggui.message(msg)
-            return
+        # Commemorate event by setting a fresh date
+        #if  self.dat_dict['now'].get_text() == "":
+        dd = datetime.datetime.now().replace(microsecond=0)
+        self.dat_dict['now'].set_text(dd.isoformat())
+
+        # This we can generate, but the user better know about it
+        # Wed 01.May.2024 Auto generated
+        self.autofill('uuid', uuid.uuid1())
+
+        # Autofill what we can
+        self.autofill('guid', self.conf.siteid)
+        self.autofill('ouid', self.ouid)
+        self.autofill('oper', self.operator)
 
         ddd = {}
         for aa in self.dat_dict.keys():
             ddd[aa] = self.dat_dict[aa].get_text()
 
         #print("Save_data", ddd)
         enc = self.packer.encode_data("", ddd)
         #print("enc:", enc)
+        uuu = self.dat_dict['uuid'].get_text()
+
+        # Add index
+        def callb(c2, id2):
+            # Replicate fields from local data
+            dddd = [uuu, enc.encode()]
+            #print("dddd:", dddd)
+            try:
+                recsel.append_index(c2, self.vcore.hashname,  recsel.hashid, dddd)
+            except:
+                print("exc save callb hash", sys.exc_info())
+            try:
+                recsel.append_index(c2, self.vcore.hashname2, recsel.hashname, dddd)
+            except:
+                print("exc save callb name", sys.exc_info())
 
         try:
-            ret = self.vcore.save_data(self.dat_dict['uuid'].get_text(), enc)
+            self.vcore.postexec = callb
+            ret = self.vcore.save_data(uuu, enc)
         except:
             pass
             print("save", sys.exc_info())
+        finally:
+            self.vcore.postexec = None
 
-        self.status.set_text("Entry '%s' saved." % self.dat_dict['name'].get_text())
-        self.status_cnt = 4
+        self.status.set_status_text("Entry '%s' saved." % self.dat_dict['name'].get_text())
 
         for aa in self.dat_dict.keys():
             self.dat_dict_org[aa] = self.dat_dict[aa].get_text()
 
-    def timer(self):
-
-        #print("Called timer")
-        if self.in_timer:
-            return True
-        in_timer = True
-        self.cnt += 1
-        if self.status_cnt:
-            self.status_cnt -= 1
-            if not self.status_cnt:
-                self.status.set_text("Idle.")
-        in_timer = False
-        return True
-
-    def set_status_text(self, text):
-        self.status.set_text(text)
-        self.status_cnt = 4
-
     def main(self):
         Gtk.main()
 
     def  OnExit(self, arg, srg2 = None):
 
         ccc = False
         for aa in self.dat_dict.keys():
             if self.dat_dict_org[aa] != self.dat_dict[aa].get_text():
                 ccc = True
         if ccc:
             msg = "Unsaved data. Are you sure you want to abandon it?"
-            self.status.set_text(msg)
+            self.status.set_status_text(msg)
             self.status_cnt = 4
-            ret = self.yesno(msg)
-            #print("yesno:", ret)
+            ret = pggui.yes_no(msg, default="No")
+            #print("yes_no:", ret)
             if ret != Gtk.ResponseType.YES:
                 return True
             else:
                 #print("Abandoning", self.dat_dict['name'].get_text())
                 pass
 
         self.exit_all()
```

### Comparing `pyvserv-1.0.4/pyvgui/guilib/pgcal.py` & `pyvserv-1.0.6/pyvgui/guilib/pgcal.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
 
 from pyvguicom import pgbox
+from pyvguicom import pggui
 
 def PopCal(ddd):
 
     ''' Open calendar dialog. While technically this is not a class,
         we attach state vars to the dialog class, pretending it is.
     '''
 
@@ -50,17 +51,19 @@
     dialog.cal.connect("button-press-event", cal_butt, dialog)
 
     dialog.entry = Gtk.Entry()
     dialog.entry.connect("key-press-event", entry_key, dialog)
     dialog.entry.connect("key-release-event", entry_key, dialog)
 
     # Adjust for zero based
-    dialog.cal.select_month(int(ddd[1])-1, int(ddd[0]))
-    dialog.cal.select_day(int(ddd[2]))
-
+    try:
+        dialog.cal.select_month(int(ddd[1])-1, int(ddd[0]))
+        dialog.cal.select_day(int(ddd[2]))
+    except:
+        pass
     helpx = Gtk.Label(  \
         "Day --      \tLeft-Arrow            \tDay ++    \t     \tRight-Arrow\n"
         "Week --     \tUp-Arrow              \tWeek ++   \t     \tUp-Arrow\n"
         "Month --    \tCtrl-Left-Arrow       \tMonth ++  \t     \tCtrl-Right-Arrow\n"
         "Year --     \tAlt-Left-Arrow        \tYear ++   \t     \tAlt-Right-Arrow\n"
         "Decade --   \tAlt-S   \t  \t   \t   \tDecade ++ \t     \tAlt-A")
 
@@ -70,17 +73,17 @@
     hbox3.pack_start(lab2, 0, 0, 2)
     hbox3.pack_start(dialog.entry, 1, 1, 2)
     hbox3.pack_start(Gtk.Label(" Entered text sets date as well. "), 0, 0, 2)
 
     dialog.pbox.pack_start(helpx, 1, 1, 0)
 
     dialog.pbox.pack_start(dialog.cal, 1, 1, 0)
-    dialog.pbox.pack_start(pgbox.xSpacer(8), 0, 0, 0)
+    dialog.pbox.pack_start(pggui.xSpacer(8), 0, 0, 0)
     dialog.pbox.pack_start(hbox3, 0, 0, 0)
-    dialog.pbox.pack_start(pgbox.xSpacer(8), 0, 0, 0)
+    dialog.pbox.pack_start(pggui.xSpacer(8), 0, 0, 0)
 
     dialog.abox = dialog.get_action_area()
 
     buttnow = Gtk.Button.new_with_mnemonic("Go to to_day")
     buttnow.connect("clicked", pynow, dialog.cal)
     dialog.abox.pack_start(buttnow, 0, 0, 0)
```

### Comparing `pyvserv-1.0.4/pyvgui/guilib/pgui.py` & `pyvserv-1.0.6/pyvgui/guilib/pgui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvgui/guilib/pymenu.py` & `pyvserv-1.0.6/pyvgui/guilib/pymenu.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvgui/guilib/recsel.py` & `pyvserv-1.0.6/pyvgui/guilib/passdlg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,425 +1,381 @@
 #!/usr/bin/env python
 
-''' Action Handler self for open records self '''
+''' Login and configure dialogs '''
 
 # pylint: disable=C0103
 
 import os
 import sys
 import datetime
+import time
+import uuid
+import io
+import struct
+import base64
+
+from Crypto.Cipher import AES
+from Crypto.Hash import SHA256
+from Crypto import Random
 
 import gi
 gi.require_version("Gtk", "3.0")
 from gi.repository import Gtk
 from gi.repository import Gdk
+from gi.repository import GLib
+from gi.repository import GdkPixbuf
 
 import pyvpacker
+from pydbase import twincore, twinchain
 
 from pyvguicom import pggui
 from pyvguicom import pgsel
 from pyvguicom import pgutils
+from pyvguicom import pgentry
 
 from pyvcommon import pyvhash
 
-''' Open voter self. We attach state vars to the self class
-'''
+COMMONKEY =  b"1234567890" * 4
 
-class RecSel(Gtk.Dialog):
+def     dbsalt(upass):
+
+    rstr = Random.new().read(4)
+    hstr = ""
+    for aa in rstr:
+        hstr += "%02x" % aa
+    hhh = SHA256.new();
+    hhh.update(bytes(upass, "utf-8") + bytes(hstr, "utf-8"))
+    #print(hstr)
+    ddd = hhh.hexdigest()
+    upass2 = ddd  + hstr
+    return upass2
+
+def    dbunsalt(upass, oldhash):
+
+    hstr = oldhash[-8:]
+    hhh = SHA256.new();
+    hhh.update(bytes(upass, "utf-8") + bytes(hstr, "utf-8"))
+    #print(hstr)
+    upass2 = hhh.hexdigest()  + hstr
+    return upass2
+
+def gen_def_data(uname, passx, flag):
+
+    dd = datetime.datetime.now().replace(microsecond=0)
+    uuuu = str(uuid.uuid1())
+    salt = dbsalt(passx)
+    ddd = [uname, "Full_Name",  "Enabled", dd.isoformat(), flag, uuuu, salt]
+
+    # Make sure it is not tempered with
+    hhh = SHA256.new();
+    hhh.update(bytes(str(ddd), "utf-8"))
+    ddd.append(hhh.hexdigest())
+
+    return ddd
+
+def auth_initial(authcore, packer, conf):
+
+    ret = [0, ]
+    datasize = authcore.getdbsize()
+    dlg = PassDlg(datasize == 0, conf)
+    #print(dlg.res)
+    if dlg.res[0] == Gtk.ResponseType.ACCEPT:
+        cipher = AES.new(COMMONKEY[:32], AES.MODE_CTR,
+                        use_aesni=True, nonce = COMMONKEY[-8:])
+        userx = cipher.decrypt(dlg.res[1]).decode()
+        cipher = AES.new(COMMONKEY[:32], AES.MODE_CTR,
+                        use_aesni=True, nonce = COMMONKEY[-8:])
+        decr = cipher.decrypt(dlg.res[2]).decode()
+        #print("userx", userx, "decr", decr)
+        if datasize == 0:
+            ret = addauth(authcore, packer, userx, decr, "Yes")
+        else:
+            ret = auth(authcore, packer, userx, decr)
+        #print("auth:", ret)
+        if ret[0] != 1:
+            pggui.message("Bad user or password")
+    else:
+        pggui.message("Must authenticate")
+
+    return ret
+
+def addauth(authcore, packer, uname, passx, flag):
+
+    ''' Replicate what the UI does, no tree update '''
+
+    #print("AddAuth:", "'" + uname + "'" , "'" + passx + "'")
+
+    # Assumng success in creation
+    ret = [1,]
+
+    salt = dbsalt(passx)
+    ddd = gen_def_data(uname, passx, flag)
+    try:
+        enc = packer.encode_data("", ddd)
+    except:
+        print("packer", sys.exc_info())
+        enc = ""
+        pass
+    authcore.save_data(ddd[5], enc)
+    ret.append(ddd)
+    return ret
+
+def auth(authcore, packer, uname, passx):
+
+    #print("Auth:", "'" + uname + "'" , "'" + passx + "'")
+
+    ret = [0,]
+    ddd2 = []; dec = {}
+    datasize = authcore.getdbsize()
+    for aa in range(datasize -1, -1, -1):
+        rrr = authcore.get_rec(aa)
+        if not rrr:
+            continue
+        try:
+            dec = packer.decode_data(rrr[1])[0]
+        except:
+            #print("Cannot decode:", rrr)
+            dec = [0]
+        try:
+            #print("dec:", dec)
+            if not dec[0] in ddd2:
+                ddd2.append(dec[0])
+                #print("dec", dec)
+                if uname == dec[0]:
+                    # Check:
+                    hhh = SHA256.new();
+                    hhh.update(bytes(str(dec[:-1]), "utf-8"))
+                    #print("sums:", hhh.hexdigest(), dec[-1])
+                    if hhh.hexdigest() != dec[-1]:
+                        print("Bad sum on:", dec[0], dec[6])
+                        continue
+                    unsaltx = dbunsalt(passx, dec[6])
+                    #print("auth", dec[0], dec[6], unsaltx)
+                    if unsaltx == dec[6]:
+                        ret[0] = 1
+                        ret.append(dec)
+                        break
+        except:
+            print("exc dec rec", dec)
+
+    return(ret)
+
+class PassDlg(Gtk.Dialog):
+
+    ''' Open password dialog.  '''
+
+    def __init__(self, firsttime, conf):
 
-    def __init__(self, vcore):
         super().__init__(self)
 
-        self.set_title("Open Record(s)")
-        self.add_buttons(   Gtk.STOCK_CANCEL, Gtk.ResponseType.REJECT,
-                            Gtk.STOCK_OK, Gtk.ResponseType.ACCEPT)
-
-        #self.set_default_response(Gtk.ResponseType.ACCEPT)
-        #self.set_position(Gtk.WindowPosition.CENTER)
-        self.set_size_request(800, 600)
+        self.set_title("Password prompt")
+        self.add_buttons(   Gtk.STOCK_OK, Gtk.ResponseType.ACCEPT,
+                            Gtk.STOCK_CANCEL, Gtk.ResponseType.REJECT)
+
+        self.set_modal(True)
+        self.set_skip_pager_hint(False)
+        self.set_skip_taskbar_hint(False)
+
+        ic = Gtk.Image(); ic.set_from_file(conf.iconf2)
+        self.set_icon(ic.get_pixbuf())
+
+        self.offs = 0
+        self.dirx = 1
+        self.overlay = Gtk.Overlay()
+        self.bg = Gtk.Image()
+        # Load file. Optionally scale it for window
+        self.bg.set_from_file(conf.iconf2)
+        try:
+            pix = self.bg.get_pixbuf()
+            #print("image", self.bg, pix)
+            www = pix.get_width();   hhh = pix.get_height()
+            #print("www", www, "hhh", hhh)
+            # Water mark it
+            self.pix2 = GdkPixbuf.Pixbuf.new(GdkPixbuf.Colorspace.RGB,
+                                   True, 8, www, hhh)
+            pix.composite(self.pix2, 0, 0, www, hhh, 0, 0, 1, 1,
+                                    GdkPixbuf.InterpType.NEAREST, 30)
+            self.bg.set_from_pixbuf(self.pix2)
+        except:
+            #print("Exc on load wartemark", sys.exc_info())
+            pass
+
+        self.overlay.add_overlay(self.bg)
+        self.set_default_response(Gtk.ResponseType.ACCEPT)
+        self.firsttime = firsttime
+        self.alt = False
         self.xmulti = []
-        self.vcore = vcore
         self.packer = pyvpacker.packbin()
         self.rec_cnt = 0
         self.scan_cnt = 0
         self.stop = False
         self.w_cursor = Gdk.Cursor(Gdk.CursorType.WATCH)
         self.sort_cnt = 0
-
+        #self.vbox3 = self.get_content_area()
         self.connect("key-press-event", self.area_key)
         self.connect("key-release-event", self.area_key)
+        self.connect("response", self.response_pre)
 
-        self.pbox = Gtk.HBox()
-        self.vbox.pack_start(self.pbox, 0, 0, 0)
-
-        simp = pgsel.LetterNumberSel(self.lettersel, "Mono 16", " ")
-        simp.set_tooltip_text("Click on selection or navigate " \
-                " to selection, press space to select")
-
-        self.vbox.pack_start(simp, 0, 0, 0)
-
-        self.vbox.pack_start(pggui.xSpacer(), 0, 0, 0)
-        label13 = Gtk.Label.new("Double click to select an entry.")
-        self.vbox.pack_start(label13, 0, 0, 0)
-        self.vbox.pack_start(pggui.xSpacer(), 0, 0, 0)
-
-        self.ts = Gtk.ListStore(str, str, str, str)
-        self.tview = self.create_ftree(self.ts)
+        self.vbox3 = Gtk.VBox()
+        self.vbox3.pack_start(pggui.ySpacer(8), 0, 0, 0)
 
-        scroll = Gtk.ScrolledWindow()
+        pbox = Gtk.HBox()
 
-        self.tview.connect("row-activated",  self.tree_sel)
-        scroll.add(self.tview)
-
-        frame2 = Gtk.Frame()
-        frame2.add(scroll)
-
-        hbox3 = Gtk.HBox()
-        label1 = Gtk.Label("   ")
-        hbox3.pack_start(label1, 0, 0, 0)
-        hbox3.pack_start(frame2, True, True, 0)
-        label2 = Gtk.Label("   ")
-        hbox3.pack_start(label2, 0, 0, 0)
-
-        self.vbox.pack_start(hbox3, True, True, 0)
-
-        label3  = Gtk.Label("  ")
-        self.vbox.pack_start(label3, 0, 0, 0)
-
-        self.abox = self.get_action_area()
+        if self.firsttime == 1:
+            vbox2 = Gtk.VBox()
+            lab1 = Gtk.Label.new("Please Enter Administrator password.")
+            pbox.pack_start(lab1, 1, 1, 0)
+            vbox2.pack_start(pbox, 0, 0, 0)
+
+            pbox2 = Gtk.HBox()
+            lab2 = Gtk.Label.new("After successful entry, this will be the master password ")
+            pbox2.pack_start(lab2, 1, 1, 0)
+            vbox2.pack_start(pbox2, 0, 0, 0)
+
+            pbox3 = Gtk.HBox()
+            lab3 = Gtk.Label.new("for administering the program. Please Make a note of this password.")
+            pbox3.pack_start(lab3, 1, 1, 0)
+            vbox2.pack_start(pbox3, 0, 0, 0)
+            self.vbox3.pack_start(vbox2, 0, 0, 0)
+
+        elif self.firsttime == 3:
+            vbox2 = Gtk.VBox()
+            lab1 = Gtk.Label.new("Please Enter New Admin password.")
+            pbox.pack_start(lab1, 1, 1, 0)
+            vbox2.pack_start(pbox, 0, 0, 0)
+
+        elif self.firsttime == 2:
+            vbox2 = Gtk.VBox()
+            lab1 = Gtk.Label.new("Please Enter New User password.")
+            pbox.pack_start(lab1, 1, 1, 0)
+            vbox2.pack_start(pbox, 0, 0, 0)
+        else:
+            lab1 = Gtk.Label.new("Please Enter User or Admin password.")
+            pbox.pack_start(lab1, 1, 1, 0)
+            self.vbox3.pack_start(pbox, 0, 0, 0)
+
+        self.vbox3.pack_start(pggui.ySpacer(8), 0, 0, 0)
+
+        gridx = Gtk.Grid()
+        gridx.set_column_spacing(6)
+        gridx.set_row_spacing(6)
+        rowcnt = 0
+        hbox4 = Gtk.HBox()
+
+        if self.firsttime == 3:
+            tp3x = ("New Admin Name: ", "name", "Enter admin name", None)
+        elif self.firsttime == 2:
+            tp3x = ("New User Name: ", "name", "Enter user name", None)
+        elif self.firsttime == 1:
+            tp3x = ("Master Admin Name: ", "name", "Enter admin name", None)
+        else:
+            tp3x = ("User Name: ", "name", "Enter user or admin name", None)
 
-        self.stopbutt = Gtk.Button("Stop Loading")
-        self.stopbutt.set_sensitive( False )
-        self.stopbutt.connect("clicked", self.stopload)
+        self.uname = pgentry.griddouble(gridx, 0, rowcnt, tp3x, None)
+        if conf.user:
+            self.uname.set_text(conf.user)
+        rowcnt += 1
+
+        tp4x = ("Password: ", "pass", "Enter Password", None)
+        self.passx = pgentry.griddouble(gridx, 0, rowcnt, tp4x, None)
+        self.passx.set_visibility(False)
+        if not self.firsttime:
+            self.passx.set_activates_default(True)
+            self.passx.noemit = True
+            if conf.apass:
+                self.passx.set_text(conf.apass)
+                self.set_focus(self.passx)
+        rowcnt += 1
+        if self.firsttime > 0:
+            tp5x = (" Veriy: ", "pass", "Enter Password to verify", None)
+            self.lab5x = pgentry.griddouble(gridx, 0, rowcnt, tp5x, None)
+            self.lab5x.set_activates_default(True)
+            self.lab5x.noemit = True
+            self.lab5x.set_visibility(False)
+        rowcnt += 1
+
+        #gridx.attach(pggui.ySpacer(8), 0, rowcnt, 1, 1)
+        #rowcnt += 1
+
+        hbox4.pack_start(pggui.xSpacer(), 1, 1, 4)
+        hbox4.pack_start(gridx, 0, 0, 4)
+        #hbox4.pack_start(pggui.xSpacer(), 1, 1, 4)
+
+        self.vbox3.pack_start(hbox4, 0, 0, 4)
+        self.vbox3.pack_start(\
+            Gtk.Label("Watermark animation is to assure authenticity."), 0, 0, 4)
 
-        self.abox.pack_start(self.stopbutt, 1, 1, 0)
-        self.abox.reorder_child(self.stopbutt, 0)
+        self.overlay.add(self.vbox3)
+        self.vbox.pack_start(self.overlay, 1, 1, 1)
 
-        self.labsss = Gtk.Label("Awaiting filter selection ...")
-        self.abox.pack_start(self.labsss, 1, 1, 0)
-        self.abox.reorder_child(self.labsss, 0)
+        #self.set_size_request(640, 280)
 
+        #self.abox = self.get_action_area()
         self.show_all()
-        self.initial_pop()
-        #self.set_focus(self.tview)
-        self.response = self.run()
+        self.overlay.reorder_overlay(self.bg, 0)
 
         self.res = []
-        if self.response == Gtk.ResponseType.ACCEPT:
-            xmodel = self.ts
-            sel = self.tview.get_selection()
-            if not sel:
-                return
-            # Is multi selection?
-            iterx = xmodel.get_iter_first()
-            while True:
-                #print("iterate", xmodel.get_value(iterx, 0))
-                if not iterx:
-                    break
-                if sel.iter_is_selected(iterx):
-                    xstr = xmodel.get_value(iterx, 0)
-                    xstr2 = xmodel.get_value(iterx, 1)
-                    xstr3 = xmodel.get_value(iterx, 2)
-                    xstr4 = xmodel.get_value(iterx, 3)
-                    self.res.append((xstr, xstr2, xstr3, xstr4))
-                iterx = xmodel.iter_next(iterx)
-
-        #print ("response", self.response, "result", self.res)
-        self.destroy()
-
-    def stopload(self, butt):
-
-        ''' Flag stop '''
-        self.stop = True
-
-    def lettersel(self, letterx):
-
-        ''' Selection callback '''
-
-        #print(letterx)
-        pgutils.usleep(10)
-        self.populate(letterx)
-        pgutils.usleep(10)
-
-    def initial_pop(self):
-
-        ''' Fill in use instructions '''
-
-        piter = self.ts.append(row=None)
-        self.ts.set(piter, 0, "Select Appropriate filter.")
-        self.ts.set(piter, 1, "From TOP row")
-        self.ts.set(piter, 2, "Selecting 'All' may take a long time to load")
-
-    # ------------------------------------------------------------------------
-
-    def populate(self, filterx = ""):
+        GLib.timeout_add(1000, self.timer)
 
-        ''' populate tree '''
-
-        if len(filterx):
-            filterx = filterx.upper()
-        #print("pop", filterx)
-
-        self.stop = False
-
-        self.labsss.set_text("Loading ...")
-        self.stopbutt.set_sensitive(True)
-        self.get_window().set_cursor(self.w_cursor)
-        pgutils.usleep(5)
-
-        # Clear old contents:
-        while True:
-            root = self.ts.get_iter_first()
-            if not root:
-                break
-            try:
-                self.ts.remove(root)
-            except:
-                print("Exception on rm ts", sys.exc_info())
-
-        self.rec_cnt = 0
-        sss = self.vcore.getdbsize()
-
-        ddd2 = []
-        for aa in range(sss-1, -1, -1):
-            rrr = self.vcore.get_rec(aa)
-            if not rrr:
-                continue
-            #print("rrr:", rrr)
-            dec = self.packer.decode_data(rrr[1])[0]
-            #print("dec:", dec)
-            #print("dec:", dec['name'], dec['dob'], dec['uuid'])
-
-            if self.stop:
-                break
-
-            self.scan_cnt += 1
-            if self.scan_cnt % 1000 == 0:
-                self.labsss.set_text("Scanning:  %d/%d Loading: %d" %
-                            (sss, self.scan_cnt, self.rec_cnt))
-                self.get_window().set_cursor(self.w_cursor)
-                pgutils.usleep(5)
-
-            # See if it is filtered:
-            if filterx != "ALL":
-                if filterx != "":
-                    if len(dec['name']):
-                        if filterx[0] != dec['name'][0].upper():
-                            #print("Filtered", dec['name'])
-                            continue
-
-            uuu = rrr[0].decode()
-
-            # Wed 24.Apr.2024 load all, include history
-            # See if we have this already
-            #found = False
-            #for aaa in ddd2:
-            #    if aaa[2] == uuu:
-            #        found = True
-            #        break
-            #if found:
-            #    continue
-
-            #print("append:", dec)
-            ddd2.append((dec['name'], dec['now'], dec['dob'],  uuu))
-            self.rec_cnt += 1
-            if self.rec_cnt % 100 == 0:
-                if self.stop:
-                    break
-            sig = False
-            if filterx == "All":
-                if self.rec_cnt >= 10000:
-                    sig = True
-            else:
-                if self.rec_cnt >= 1000:
-                    sig = True
-            if sig:
-                msg = "Loaded 10000 records, stopping. \n" \
-                        "If your intended record is not included, please narrow filter."
-                pggui.message(msg)
-                self.set_focus(self.tview)
-                break
-
-        self.stopbutt.set_sensitive( False )
-
-        for aa in ddd2:
-            piter = self.ts.append(row=None)
-            #print("row", aa)
-            self.ts.set(piter, 0, aa[0])
-            self.ts.set(piter, 1, aa[1])
-            self.ts.set(piter, 2, aa[2])
-            self.ts.set(piter, 3, aa[3])
-
-        self.labsss.set_text("%s records." % self.rec_cnt)
-
-        self.get_window().set_cursor()
-
-        # --------------------------------------------------------------------
-
-    def compare(self, model, row1, row2, user_data):
-
-        ''' compare fields for sort '''
-
-        self.sort_cnt += 1
-        #if self.sort_cnt % 1000 == 0:
-        #    self.get_window().set_cursor(self.w_cursor)
-        #    pgutils.usleep(5)
-
-        sort_column, _ = model.get_sort_column_id()
-        value1 = model.get_value(row1, sort_column)
-        value2 = model.get_value(row2, sort_column)
-        #print(sort_column, value1, value2)
-        if value1 < value2:
-            return -1
-        elif value1 == value2:
-            return 0
-        else:
-            return 1
-
-    def ncompare(self, model, row1, row2, user_data):
-
-        ''' compare fields for sort '''
-
-        self.sort_cnt += 1
-        sort_column, _ = model.get_sort_column_id()
-        value1 = model.get_value(row1, sort_column)
-        value2 = model.get_value(row2, sort_column)
-        #print("n", sort_column, value1, value2, type(value1))
-
-        dd = datetime.datetime.now()
-        try:
-            dd2 = dd.strptime(value1, "%Y/%m/%d").timestamp()
-        except:
-            dd2 = 0
-        try:
-            dd3 = dd.strptime(value2, "%Y/%m/%d").timestamp()
-        except:
-            dd3 = 0
-
-        if int(dd2) < int(dd3):
-            return -1
-        elif int(dd2) == int(dd3):
-            return 0
+        response = self.run()
+        self.res.append(response)
+        if response == Gtk.ResponseType.ACCEPT:
+            # Transmittted encrypted from dialog
+            cipher = AES.new(COMMONKEY[:32], AES.MODE_CTR,
+                            use_aesni=True, nonce = COMMONKEY[-8:])
+            userx = cipher.encrypt(self.uname.get_text().encode())
+            self.res.append(userx)
+            cipher = AES.new(COMMONKEY[:32], AES.MODE_CTR,
+                            use_aesni=True, nonce = COMMONKEY[-8:])
+            cyph = cipher.encrypt(self.passx.get_text().encode())
+            self.res.append(cyph)
         else:
-            return 1
-
-    def dcompare(self, model, row1, row2, user_data):
+            self.res.append("")
+        self.destroy()
 
-        ''' compare fields for sort '''
+    def timer(self):
 
-        self.sort_cnt += 1
+        ''' Animate watermark '''
 
-        sort_column, _ = model.get_sort_column_id()
-        value1 = model.get_value(row1, sort_column)
-        value2 = model.get_value(row2, sort_column)
-        #print("n", sort_column, value1, value2, type(value1))
-        dd = datetime.datetime.now()
-        #YYYY-MM-DDTHH:MM
-        try:
-            dd2 = dd.strptime(value1, pyvhash.isostr).timestamp()
-        except:
-            print(sys.exc_info())
-            dd2 = 0
+        if self.offs > 10:
+            self.dirx = -1
+        if self.offs == 0:
+            self.dirx = 1
+        self.offs += self.dirx
         try:
-            dd3 = dd.strptime(value2, isostr).timestamp()
+            www =   self.pix2.get_width();   hhh = self.pix2.get_height()
+            pix3 = GdkPixbuf.Pixbuf.new(GdkPixbuf.Colorspace.RGB,
+                                   True, 8, www + self.offs, hhh + self.offs)
+            self.pix2.composite(pix3, + self.offs, + self.offs, www, hhh, self.offs, self.offs, 1, 1,
+                                    GdkPixbuf.InterpType.NEAREST, 255)
+            self.bg.set_from_pixbuf(pix3)
         except:
-            dd3 = 0
-
-        #print("dd 2/3", dd2, dd3)
-
-        if int(dd2) < int(dd3):
-            return -1
-        elif int(dd2) == int(dd3):
-            return 0
-        else:
-            return 1
-
-    def create_ftree(self, ts):
-
-        ''' worker function for tree creation '''
-
-        # create the tview using ts
-        tv = Gtk.TreeView(model=ts)
-
-        tv.set_search_column(0)
-        tv.set_headers_clickable(True)
-        #tv.set_enable_search(True)
-        ts.set_sort_func(0, self.compare, None)
-        ts.set_sort_func(1, self.dcompare, None)
-        ts.set_sort_func(2, self.ncompare, None)
-
-        # create a CellRendererText to render the data
-        cell = Gtk.CellRendererText()
-        tvcolumn = Gtk.TreeViewColumn('Name')
-        tvcolumn.set_min_width(240)
-        tvcolumn.pack_start(cell, True)
-        tvcolumn.add_attribute(cell, 'text', 0)
-        tvcolumn.set_sizing(Gtk.TreeViewColumnSizing.AUTOSIZE)
-        tvcolumn.set_sort_column_id(0)
-        tv.append_column(tvcolumn)
-
-        celld = Gtk.CellRendererText()
-        tvcolumn2 = Gtk.TreeViewColumn('Date of Entry')
-        tvcolumn2.set_min_width(100)
-        tvcolumn2.pack_start(celld, True)
-        tvcolumn2.add_attribute(celld, 'text', 1)
-        tvcolumn2.set_sizing(Gtk.TreeViewColumnSizing.AUTOSIZE)
-        tvcolumn2.set_sort_column_id(1)
-        tv.append_column(tvcolumn2)
-
-        cellx = Gtk.CellRendererText()
-        tvcolumn3 = Gtk.TreeViewColumn('Date of Birth')
-        tvcolumn3.set_min_width(100)
-        tvcolumn3.pack_start(cellx, True)
-        tvcolumn3.add_attribute(cellx, 'text', 2)
-        tvcolumn3.set_sizing(Gtk.TreeViewColumnSizing.AUTOSIZE)
-        tvcolumn3.set_sort_column_id(2)
-        tv.append_column(tvcolumn3)
-
-        cell2 = Gtk.CellRendererText()
-        tvcolumn2 = Gtk.TreeViewColumn('UUID')
-        tvcolumn2.set_min_width(100)
-        tvcolumn2.set_sizing(Gtk.TreeViewColumnSizing.AUTOSIZE)
-        tvcolumn2.set_sort_column_id(3)
-        tvcolumn2.pack_start(cell2, True)
-        tvcolumn2.add_attribute(cell2, 'text', 3)
-        tv.append_column(tvcolumn2)
-
-        #tv.get_selection().set_mode(Gtk.SelectionMode.MULTIPLE)
-
-        return tv
-
-    def tree_sel_row(self, xtree):
-        pass
-
-    def tree_sel(self, xtree, xiter, xpath):
-
-        #print ("tree_sel", xtree, xiter, xpath)
-        sel = xtree.get_selection()
-        xmodel, xpath = sel.get_selected_rows()
-        if xpath:
-            #for aa in xpath:
-            #    xiter2 = xmodel.get_iter(aa)
-            #    xstr = xmodel.get_value(xiter2, 0)
-            #    xstr2 = xmodel.get_value(xiter2, 1)
-            #    print("mul selstr: ", "'" + xstr + "'" )
-            selfx.response(Gtk.ResponseType.ACCEPT)
-
-    # If directory, change to it
-    def click_dir_action(self, xstr):
-        if xstr[0] == "[":
-            xstr = xstr[1:len(xstr)-1]
-        if os.path.isdir(xstr):
-            #print ("dir", xstr)
-            os.chdir(xstr)
-            return True
-
-        return False
+            pass
+        return True
 
-    # Call key handler
+    # Evaluate respoonse
+    def response_pre(self, arg2, arg3):
+        #print("response", arg2, arg3)
+        if arg3 == Gtk.ResponseType.ACCEPT:
+            if self.uname.get_text() == "":
+                self.set_focus(self.uname)
+                pggui.message("User name cannot be empty.")
+                self.stop_emission_by_name ("response")
+                return True
+            if self.passx.get_text() == "":
+                self.set_focus(self.passx)
+                pggui.message("Password name cannot be empty.")
+                self.stop_emission_by_name ("response")
+                return True
+            if self.firsttime:
+                if self.passx.get_text() != self.lab5x.get_text():
+                    self.set_focus(self.lab5x)
+                    pggui.message("Passwords must match.")
+                    self.stop_emission_by_name ("response")
+                    return True
 
     def area_key(self, area, event):
 
         #print("area_key", event.keyval)
 
         # Do key down:
         if  event.type == Gdk.EventType.KEY_PRESS:
```

### Comparing `pyvserv-1.0.4/pyvgui/pyvcpanel.py` & `pyvserv-1.0.6/pyvgui/pyvcpanel.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
     sys.path.append(os.path.join(base,  "..", "pyvgui"))
     sys.path.append(os.path.join(base,  "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-from pyvguicom import sutil
+from pyvguicom import pgutils
 # Get Parent of module root
-sf = os.path.dirname(sutil.__file__)
+sf = os.path.dirname(pgutils.__file__)
 sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
 #print("Load:", sys.path[-1])
 
 from pyvcommon import support, comline, pywrap
 from pyvcommon import pydata, pyservsup,  crysupp
 from pyvserver import pyvstate
```

### Comparing `pyvserv-1.0.4/pyvgui/pyvservui.py` & `pyvserv-1.0.6/pyvgui/pyvservui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 
 from __future__ import absolute_import
 from __future__ import print_function
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
@@ -26,17 +26,17 @@
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
     sys.path.append(os.path.join(base, "..", "pyvgui"))
     sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-from pyvguicom import sutil
+from pyvguicom import pgutils
 # Get Parent of module root
-sf = os.path.dirname(sutil.__file__)
+sf = os.path.dirname(pgutils.__file__)
 sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
 from pyvcommon import support, comline, pywrap
 from pyvcommon import pydata, pyservsup,  crysupp
 
 from guilib import mainwinserv
```

### Comparing `pyvserv-1.0.4/pyvgui/pyvtally.py` & `pyvserv-1.0.6/pyvgui/pyvtally.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
     sys.path.append(os.path.join(base,  "..", "pyvgui"))
     sys.path.append(os.path.join(base,  "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
-from pyvguicom import sutil
+from pyvguicom import pgutils
 # Get Parent of module root
-sf = os.path.dirname(sutil.__file__)
+sf = os.path.dirname(pgutils.__file__)
 sys.path.append(os.path.join(sf, "..", "pyvguicom"))
 
 #print("Load:", sys.path[-1])
 
 from pyvcommon import support, comline, pywrap
 from pyvcommon import pydata, pyservsup,  crysupp
 from pyvserver import pyvstate
```

### Comparing `pyvserv-1.0.4/pyvgui/pyvvote.py` & `pyvserv-1.0.6/pyvgui/pyvvote.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,58 +47,87 @@
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     ''' Display help '''
 
-    print()
+    print( "Voter adminstration utility. Add / Review / Delete voters.")
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 9999)")
-    print( "            -v        - Verbose")
-    print( "            -V        - Version")
-    print( "            -q        - Quiet")
-    print( "            -h        - Help")
-    print()
+    print( "            -v        - Verbose. Print more info.")
+    print( "            -u        - User Name. Defult: 'admin'")
+    print( "            -a        - Clear text password. For test only. Default: '1234'")
+    print( "            -V        - Print version number.")
+    print( "            -t        - Test mode. Extra buttons.")
+    print( "            -q        - Quiet. Less printing.")
+    print( "            -h        - Help (This screen)")
     sys.exit(0)
 
+    #print( "            -p        - Port to use (default: 6666)")
+
 # ------------------------------------------------------------------------
 def pversion():
 
     ''' Show vwersion info '''
 
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "debug=",   "pgdebug",  0,      None],      \
-    ["p:",  "port=",    "port",     9999,   None],      \
-    ["v",   "verbose",  "verbose",  0,      None],      \
-    ["q",   "quiet",    "quiet",    0,      None],      \
-    ["r:",  "dataroot=", "droot",   "pyvserver",     None],      \
-    ["V",   "version",  None,       None,   pversion],  \
-    ["h",   "help",     None,       None,   phelp]      \
+    ["d:",  "debug=",       "pgdebug",  0,              None],      \
+    ["p:",  "port=",        "port",     6666,           None],      \
+    ["v",   "verbose",      "verbose",  0,              None],      \
+    ["q",   "quiet",        "quiet",    0,              None],      \
+    ["u:",  "user=",        "user",     "admin",        None],      \
+    ["a:",  "pass=",        "apass",    "1234",         None],      \
+    ["t",   "testx",        "testx",    0,              None],      \
+    ["r:",  "dataroot=",    "droot",    "pyvclient",    None],      \
+    ["V",   "version",      None,       None,           pversion],  \
+    ["h",   "help",         None,       None,           phelp]      \
 
 conf = comline.ConfigLong(optarr)
 
 def mainfunct():
 
     ''' Main entry point '''
 
     #print("pyvcpanel started ...")
     args = conf.comline(sys.argv[1:])
     #print("args", args)
 
+    # To know where the icon file is
+    conf.me = __file__
+    #print(dir(conf))
+
     pyservsup.globals  = pyservsup.Global_Vars(__file__, conf.droot)
     pyservsup.globals.conf = conf
 
-    mw = mainwinvote.MainWin()
+    pyservsup.globals.softmkdir(pyservsup.globals.myhome)
+
+    # Change directory to the data dir
+    os.chdir(pyservsup.globals.myhome)
+    if conf.verbose:
+        print("cwd", os.getcwd())
+
+    # Patch passdir for client
+    pyservsup.globals.passdir   =  pyservsup.globals.myhome + ".pyvclient" + os.sep
+    pyservsup.globals.softmkdir(pyservsup.globals.passdir)
+    pyservsup.globals.passfile = pyservsup.globals.passdir + os.sep + pyservsup.globals._passfile
+
+    # Patch idfile for client
+    pyservsup.globals.idfile = pyservsup.globals.myhome + os.sep + "pyvclient.init"
+
+    # Create support objects
+    pyservsup.globals.config(pyservsup.globals.myhome, conf)
+
+    pyservsup.gl_passwd = pyservsup.Passwd()
+
+    mw = mainwinvote.MainWin(pyservsup.globals)
     mw.main()
     sys.exit(0)
 
 if __name__ == '__main__':
 
     mainfunct()
```

### Comparing `pyvserv-1.0.4/pyvserv.egg-info/PKG-INFO` & `pyvserv-1.0.6/pyvserv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.4
+Version: 1.0.6
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyvserv-1.0.4/pyvserv.egg-info/SOURCES.txt` & `pyvserv-1.0.6/pyvserv.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -92,23 +92,38 @@
 pyvcommon/pyservsup.py
 pyvcommon/pysyslog.py
 pyvcommon/pyv2fa.py
 pyvcommon/pyvhash.py
 pyvcommon/pywrap.py
 pyvcommon/support.py
 pyvgui/__init__.py
+pyvgui/pyvballot.png
+pyvgui/pyvballot.py
 pyvgui/pyvcpanel.py
+pyvgui/pyvpeople.png
+pyvgui/pyvpeople.py
 pyvgui/pyvservui.py
 pyvgui/pyvtally.py
+pyvgui/pyvvote.png
 pyvgui/pyvvote.py
+pyvgui/pyvvote_sub.png
+pyvgui/vote.png
+pyvgui/docs/pyvcpanel.html
+pyvgui/docs/pyvservui.html
+pyvgui/docs/pyvtally.html
 pyvgui/guilib/__init__.py
+pyvgui/guilib/config.py
+pyvgui/guilib/entry_color.py
+pyvgui/guilib/mainballot.py
 pyvgui/guilib/mainwin.py
+pyvgui/guilib/mainwinpeople.py
 pyvgui/guilib/mainwinserv.py
 pyvgui/guilib/mainwintally.py
 pyvgui/guilib/mainwinvote.py
+pyvgui/guilib/passdlg.py
 pyvgui/guilib/pgcal.py
 pyvgui/guilib/pgui.py
 pyvgui/guilib/pymenu.py
 pyvgui/guilib/recsel.py
 pyvserv.egg-info/PKG-INFO
 pyvserv.egg-info/SOURCES.txt
 pyvserv.egg-info/dependency_links.txt
```

### Comparing `pyvserv-1.0.4/pyvserv.egg-info/entry_points.txt` & `pyvserv-1.0.6/pyvserv.egg-info/entry_points.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 [console_scripts]
+pyvballot = pyvballot:mainfunct
 pyvcli_cli = pyvcli_cli:mainfunct
 pyvcli_fman = pyvcli_fman:mainfunct
 pyvcli_gethelp = pyvcli_gethelp:mainfunct
 pyvcli_hello = pyvcli_hello:mainfunct
 pyvcli_ihost = pyvcli_ihost:mainfunct
 pyvcli_qr = pyvcli_qr:mainfunct
 pyvcli_replic = pyvcli_replic:mainfunct
 pyvcli_rman = pyvcli_rman:mainfunct
 pyvcli_uini = pyvcli_uini:mainfunct
 pyvcli_uman = pyvcli_uman:mainfunct
 pyvcli_ver = pyvcli_ver:mainfunct
 pyvcpanel = pyvcpanel:mainfunct
 pyvgenkey = pyvgenkey:mainfunct
 pyvgenkeys = pyvgenkeys:mainfunct
+pyvpeople = pyvpeople:mainfunct
 pyvreplic = pyvreplic:mainfunct
 pyvserv = pyvserv:mainfunct
 pyvservui = pyvservui:mainfunct
 pyvtally = pyvtally:mainfunct
+pyvvote = pyvvote:mainfunct
```

### Comparing `pyvserv-1.0.4/pyvserver/docs/pyvfunc.html` & `pyvserv-1.0.6/pyvserver/docs/pyvfunc.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/docs/pyvreplic.html` & `pyvserv-1.0.6/pyvserver/docs/pyvreplic.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/docs/pyvserv.html` & `pyvserv-1.0.6/pyvserver/docs/pyvserv.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/docs/pyvstate.html` & `pyvserv-1.0.6/pyvserver/docs/pyvstate.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/pyvfunc.py` & `pyvserv-1.0.6/pyvserver/pyvfunc.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/pyvreplic.py` & `pyvserv-1.0.6/pyvserver/pyvreplic.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/pyvserv.py` & `pyvserv-1.0.6/pyvserver/pyvserv.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvserver/pyvstate.py` & `pyvserv-1.0.6/pyvserver/pyvstate.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvtools/docs/pyvgenkey.html` & `pyvserv-1.0.6/pyvtools/docs/pyvgenkey.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvtools/docs/pyvgenkeys.html` & `pyvserv-1.0.6/pyvtools/docs/pyvgenkeys.html`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvtools/pyvgenkey.py` & `pyvserv-1.0.6/pyvtools/pyvgenkey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/pyvtools/pyvgenkeys.py` & `pyvserv-1.0.6/pyvtools/pyvgenkeys.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.4/setup.py` & `pyvserv-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
           'Topic :: Software Development :: Servers',
         ]
 
 includex = ["*", "pyvgui/", "pyvgui/guilib/", "pyvclient/", "pyvserver/",
-                    "pyvcommon/", "pyvtools/", ]
+                    "pyvcommon/", "pyvtools/",]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # The shortlist of starter applications
 
 test_root = [\
@@ -48,37 +48,38 @@
 #print(test_scripts); #print(test_exec)
 
 # Get version number  from the server support file:
 fp = open("pyvcommon/pyservsup.py", "rt")
 vvv = fp.read(); fp.close()
 loc_vers =  '1.0.0'     # Default
 for aa in vvv.split("\n"):
-    idx = aa.find("version =")
+    idx = aa.find("VERSION =")
     if idx == 0:        # At the beginning of line
         try:
             loc_vers = aa.split()[2].replace('"', "")
             break
         except:
             pass
 #print("loc_vers:", loc_vers)
+#sys.exit(0)
 
 # Dependency list, generate separate for windows
 # Sat 06.Apr.2024 same for all
 try:
     import fcntl
     #deplist = ["pyvpacker", "pydbase", "pycryptodome",
     #                    "pyvecc", "pyvguicom", "readline"],
 
     # Thu 04.Apr.2024 abandoned readline; may install by hand
     deplist = ["pyvpacker", "pydbase", "pycryptodome",
                         "pyvecc", "pyvguicom", ],
 except:
     # No fnctl, windows
     deplist = ["pyvpacker", "pydbase", "pycryptodome",
-                        "pyvecc", "pyvguicom"],
+                        "pyvecc", "pyvguicom", ],
 
 doclist = []; droot = "pyvserver/docs/"
 doclistx = os.listdir(droot)
 for aa in doclistx:
     doclist.append("docs/" + aa)
 
 cdoclist = []; droot2 = "pyvclient/docs/"
@@ -96,36 +97,39 @@
 #print("find packages:", setuptools.find_packages(include=includex))
 #print("deplist:", deplist)
 #print("doclist:", doclist)
 #print("cdoclist:", cdoclist)
 #print("tdoclist:", tdoclist)
 #sys.exit(1)
 
+classx = [
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ]
+
 setuptools.setup(
     name="pyvserv",
     version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power secure server with blockchain backend.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pyvserv",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
+    classifiers=classx,
     packages=setuptools.find_packages(include=includex),
     include_package_data = True,
     scripts = [
                 "pyvserver/pyvserv.py",
                 "pyvserver/pyvreplic.py",
                 "pyvtools/pyvgenkey.py", "pyvtools/pyvgenkeys.py",
                 "pyvgui/pyvservui.py", "pyvgui/pyvcpanel.py",
-                "pyvgui/pyvtally.py",
+                "pyvgui/pyvtally.py",  "pyvgui/pyvvote.py",
+                "pyvgui/pyvpeople.py",  "pyvgui/pyvballot.py",
                 *test_scripts,
                 ],
     package_dir = {
                     'pyvgui':           'pyvgui',
                     'pyvgui/guilib':    'pyvgui/guilib',
                     'pyvcommon':        'pyvcommon',
                     'pyvserver':        'pyvserver',
@@ -133,23 +137,40 @@
                     'pyvtools':         'pyvtools',
                    },
 
     package_data = {    "pyvserver" :  doclist,
                         "pyvclient" : cdoclist,
                         "pyvtools"  : tdoclist,
                    },
+
+    data_files =  [
+                    ("pyvgui", [
+                                "pyvgui/pyvpeople.png",
+                                "pyvgui/pyvballot.png",
+                                "pyvgui/pyvvote.png",
+                                "pyvgui/vote.png",
+                                "pyvgui/pyvvote_sub.png"]),
+                    ("pyvgui/docs", [
+                                "pyvgui/docs/pyvtally.html",
+                                "pyvgui/docs/pyvcpanel.html",
+                                 "pyvgui/docs/pyvservui.html"]),
+                    ],
+
     python_requires='>=3',
     install_requires=deplist,
     entry_points={
         'console_scripts': [ "pyvserv=pyvserv:mainfunct",
                              "pyvreplic=pyvreplic:mainfunct",
                              "pyvgenkey=pyvgenkey:mainfunct",
                              "pyvgenkeys=pyvgenkeys:mainfunct",
                              "pyvservui=pyvservui:mainfunct",
                              "pyvcpanel=pyvcpanel:mainfunct",
                              "pyvtally=pyvtally:mainfunct",
+                             "pyvvote=pyvvote:mainfunct",
+                             "pyvpeople=pyvpeople:mainfunct",
+                             "pyvballot=pyvballot:mainfunct",
                              test_exec,
             ],
     },
 )
 
 # EOF
```

