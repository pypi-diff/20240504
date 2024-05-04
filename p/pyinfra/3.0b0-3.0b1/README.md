# Comparing `tmp/pyinfra-3.0b0.tar.gz` & `tmp/pyinfra-3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinfra-3.0b0.tar", last modified: Thu Jan 25 21:23:31 2024, max compression
+gzip compressed data, was "pyinfra-3.0b1.tar", last modified: Sat May  4 19:20:48 2024, max compression
```

## Comparing `pyinfra-3.0b0.tar` & `pyinfra-3.0b1.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.594740 pyinfra-3.0b0/
--rw-r--r--   0 nick       (501) staff       (20)     1527 2024-01-25 21:20:54.000000 pyinfra-3.0b0/CHANGELOG.md
--rw-r--r--   0 nick       (501) staff       (20)     1076 2021-01-18 10:52:39.000000 pyinfra-3.0b0/LICENSE.md
--rw-r--r--   0 nick       (501) staff       (20)       59 2024-01-23 20:10:51.000000 pyinfra-3.0b0/MANIFEST.in
--rw-r--r--   0 nick       (501) staff       (20)     5722 2024-01-25 21:23:31.594862 pyinfra-3.0b0/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     4526 2024-01-25 21:05:40.000000 pyinfra-3.0b0/README.md
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.567781 pyinfra-3.0b0/pyinfra/
--rw-r--r--   0 nick       (501) staff       (20)      535 2024-01-03 20:23:54.000000 pyinfra-3.0b0/pyinfra/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)       47 2020-01-22 18:18:30.000000 pyinfra-3.0b0/pyinfra/__main__.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.570556 pyinfra-3.0b0/pyinfra/api/
--rw-r--r--   0 nick       (501) staff       (20)      888 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/api/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     9688 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/arguments.py
--rw-r--r--   0 nick       (501) staff       (20)     2201 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/arguments_typed.py
--rw-r--r--   0 nick       (501) staff       (20)     7176 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/command.py
--rw-r--r--   0 nick       (501) staff       (20)     4221 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/config.py
--rw-r--r--   0 nick       (501) staff       (20)     1416 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/connect.py
--rw-r--r--   0 nick       (501) staff       (20)      544 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/connectors.py
--rw-r--r--   0 nick       (501) staff       (20)     2756 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/deploy.py
--rw-r--r--   0 nick       (501) staff       (20)     1445 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)    10283 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/facts.py
--rw-r--r--   0 nick       (501) staff       (20)    12394 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/host.py
--rw-r--r--   0 nick       (501) staff       (20)     7663 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/inventory.py
--rw-r--r--   0 nick       (501) staff       (20)    13225 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/operation.py
--rw-r--r--   0 nick       (501) staff       (20)    10921 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/operations.py
--rw-r--r--   0 nick       (501) staff       (20)    12526 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/state.py
--rw-r--r--   0 nick       (501) staff       (20)    11977 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/api/util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.572244 pyinfra-3.0b0/pyinfra/connectors/
--rw-r--r--   0 nick       (501) staff       (20)        0 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/connectors/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     3754 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/connectors/base.py
--rw-r--r--   0 nick       (501) staff       (20)     5963 2024-01-25 20:17:54.000000 pyinfra-3.0b0/pyinfra/connectors/chroot.py
--rw-r--r--   0 nick       (501) staff       (20)     8954 2024-01-25 19:39:08.000000 pyinfra-3.0b0/pyinfra/connectors/docker.py
--rw-r--r--   0 nick       (501) staff       (20)     8943 2024-01-25 19:38:03.000000 pyinfra-3.0b0/pyinfra/connectors/dockerssh.py
--rw-r--r--   0 nick       (501) staff       (20)     6937 2024-01-25 20:20:41.000000 pyinfra-3.0b0/pyinfra/connectors/local.py
--rw-r--r--   0 nick       (501) staff       (20)    20263 2024-01-25 16:41:16.000000 pyinfra-3.0b0/pyinfra/connectors/ssh.py
--rw-r--r--   0 nick       (501) staff       (20)     3683 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/connectors/ssh_util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.572700 pyinfra-3.0b0/pyinfra/connectors/sshuserclient/
--rw-r--r--   0 nick       (501) staff       (20)       44 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/connectors/sshuserclient/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     9720 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/connectors/sshuserclient/client.py
--rw-r--r--   0 nick       (501) staff       (20)     2721 2023-01-15 18:23:08.000000 pyinfra-3.0b0/pyinfra/connectors/sshuserclient/config.py
--rw-r--r--   0 nick       (501) staff       (20)     3541 2024-01-25 20:37:05.000000 pyinfra-3.0b0/pyinfra/connectors/terraform.py
--rw-r--r--   0 nick       (501) staff       (20)    11321 2024-01-24 20:17:59.000000 pyinfra-3.0b0/pyinfra/connectors/util.py
--rw-r--r--   0 nick       (501) staff       (20)     4697 2024-01-25 20:18:22.000000 pyinfra-3.0b0/pyinfra/connectors/vagrant.py
--rw-r--r--   0 nick       (501) staff       (20)     3394 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/context.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.577175 pyinfra-3.0b0/pyinfra/facts/
--rw-r--r--   0 nick       (501) staff       (20)      347 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      482 2024-01-23 20:10:49.000000 pyinfra-3.0b0/pyinfra/facts/apk.py
--rw-r--r--   0 nick       (501) staff       (20)     1999 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/apt.py
--rw-r--r--   0 nick       (501) staff       (20)     2266 2022-11-03 15:24:51.000000 pyinfra-3.0b0/pyinfra/facts/brew.py
--rw-r--r--   0 nick       (501) staff       (20)      490 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/bsdinit.py
--rw-r--r--   0 nick       (501) staff       (20)      531 2024-01-23 20:10:49.000000 pyinfra-3.0b0/pyinfra/facts/cargo.py
--rw-r--r--   0 nick       (501) staff       (20)      716 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/choco.py
--rw-r--r--   0 nick       (501) staff       (20)     1662 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/deb.py
--rw-r--r--   0 nick       (501) staff       (20)      862 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/dnf.py
--rw-r--r--   0 nick       (501) staff       (20)     1678 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/docker.py
--rw-r--r--   0 nick       (501) staff       (20)    11475 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/files.py
--rw-r--r--   0 nick       (501) staff       (20)      473 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/gem.py
--rw-r--r--   0 nick       (501) staff       (20)     1294 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/git.py
--rw-r--r--   0 nick       (501) staff       (20)     3729 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/gpg.py
--rw-r--r--   0 nick       (501) staff       (20)    11402 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/hardware.py
--rw-r--r--   0 nick       (501) staff       (20)     3374 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/iptables.py
--rw-r--r--   0 nick       (501) staff       (20)      668 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/launchd.py
--rw-r--r--   0 nick       (501) staff       (20)      337 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/lxd.py
--rw-r--r--   0 nick       (501) staff       (20)     5896 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/mysql.py
--rw-r--r--   0 nick       (501) staff       (20)      674 2022-11-03 15:24:51.000000 pyinfra-3.0b0/pyinfra/facts/npm.py
--rw-r--r--   0 nick       (501) staff       (20)     1350 2024-01-23 20:10:49.000000 pyinfra-3.0b0/pyinfra/facts/openrc.py
--rw-r--r--   0 nick       (501) staff       (20)     1001 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/pacman.py
--rw-r--r--   0 nick       (501) staff       (20)      702 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/pip.py
--rw-r--r--   0 nick       (501) staff       (20)      452 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/pkg.py
--rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/pkgin.py
--rw-r--r--   0 nick       (501) staff       (20)     4104 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/postgresql.py
--rw-r--r--   0 nick       (501) staff       (20)     1973 2022-10-24 10:12:32.000000 pyinfra-3.0b0/pyinfra/facts/rpm.py
--rw-r--r--   0 nick       (501) staff       (20)     4272 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/selinux.py
--rw-r--r--   0 nick       (501) staff       (20)    19794 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/server.py
--rw-r--r--   0 nick       (501) staff       (20)     1910 2022-10-24 10:12:32.000000 pyinfra-3.0b0/pyinfra/facts/snap.py
--rw-r--r--   0 nick       (501) staff       (20)     3367 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/systemd.py
--rw-r--r--   0 nick       (501) staff       (20)     1490 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/sysvinit.py
--rw-r--r--   0 nick       (501) staff       (20)      543 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/upstart.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.577587 pyinfra-3.0b0/pyinfra/facts/util/
--rw-r--r--   0 nick       (501) staff       (20)      521 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/util/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      730 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/util/databases.py
--rw-r--r--   0 nick       (501) staff       (20)     1090 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/facts/util/packaging.py
--rw-r--r--   0 nick       (501) staff       (20)     2561 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/util/win_files.py
--rw-r--r--   0 nick       (501) staff       (20)      591 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/vzctl.py
--rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/xbps.py
--rw-r--r--   0 nick       (501) staff       (20)      827 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/yum.py
--rw-r--r--   0 nick       (501) staff       (20)      766 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/facts/zypper.py
--rw-r--r--   0 nick       (501) staff       (20)     2751 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/local.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.588400 pyinfra-3.0b0/pyinfra/operations/
--rw-r--r--   0 nick       (501) staff       (20)      357 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/operations/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2049 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/apk.py
--rw-r--r--   0 nick       (501) staff       (20)    13526 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/apt.py
--rw-r--r--   0 nick       (501) staff       (20)     5040 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/brew.py
--rw-r--r--   0 nick       (501) staff       (20)     1578 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/bsdinit.py
--rw-r--r--   0 nick       (501) staff       (20)     1042 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/cargo.py
--rw-r--r--   0 nick       (501) staff       (20)     1453 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/choco.py
--rw-r--r--   0 nick       (501) staff       (20)     5550 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/dnf.py
--rw-r--r--   0 nick       (501) staff       (20)    52409 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/files.py
--rw-r--r--   0 nick       (501) staff       (20)     1070 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/gem.py
--rw-r--r--   0 nick       (501) staff       (20)    11543 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/git.py
--rw-r--r--   0 nick       (501) staff       (20)     8856 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/iptables.py
--rw-r--r--   0 nick       (501) staff       (20)     1164 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/launchd.py
--rw-r--r--   0 nick       (501) staff       (20)     1639 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/lxd.py
--rw-r--r--   0 nick       (501) staff       (20)    19141 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/mysql.py
--rw-r--r--   0 nick       (501) staff       (20)     1404 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/npm.py
--rw-r--r--   0 nick       (501) staff       (20)     1510 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/openrc.py
--rw-r--r--   0 nick       (501) staff       (20)     1672 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/pacman.py
--rw-r--r--   0 nick       (501) staff       (20)     5377 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/pip.py
--rw-r--r--   0 nick       (501) staff       (20)     2222 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/pkg.py
--rw-r--r--   0 nick       (501) staff       (20)     1930 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/pkgin.py
--rw-r--r--   0 nick       (501) staff       (20)     9162 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/postgresql.py
--rw-r--r--   0 nick       (501) staff       (20)      797 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/operations/puppet.py
--rw-r--r--   0 nick       (501) staff       (20)     1909 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/python.py
--rw-r--r--   0 nick       (501) staff       (20)     5347 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/selinux.py
--rw-r--r--   0 nick       (501) staff       (20)    35710 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/server.py
--rw-r--r--   0 nick       (501) staff       (20)     2987 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/snap.py
--rw-r--r--   0 nick       (501) staff       (20)     5493 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/ssh.py
--rw-r--r--   0 nick       (501) staff       (20)     3719 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/systemd.py
--rw-r--r--   0 nick       (501) staff       (20)     4003 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/sysvinit.py
--rw-r--r--   0 nick       (501) staff       (20)     1908 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/upstart.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.588904 pyinfra-3.0b0/pyinfra/operations/util/
--rw-r--r--   0 nick       (501) staff       (20)      366 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/util/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     3339 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/util/files.py
--rw-r--r--   0 nick       (501) staff       (20)     8300 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/util/packaging.py
--rw-r--r--   0 nick       (501) staff       (20)     1031 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/util/service.py
--rw-r--r--   0 nick       (501) staff       (20)     3010 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/vzctl.py
--rw-r--r--   0 nick       (501) staff       (20)     1446 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/xbps.py
--rw-r--r--   0 nick       (501) staff       (20)     5543 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/yum.py
--rw-r--r--   0 nick       (501) staff       (20)     5494 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra/operations/zypper.py
--rw-r--r--   0 nick       (501) staff       (20)     4193 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/progress.py
--rw-r--r--   0 nick       (501) staff       (20)        0 2024-01-23 20:10:51.000000 pyinfra-3.0b0/pyinfra/py.typed
--rw-r--r--   0 nick       (501) staff       (20)      153 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra/version.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.568474 pyinfra-3.0b0/pyinfra.egg-info/
--rw-r--r--   0 nick       (501) staff       (20)     5722 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/PKG-INFO
--rw-r--r--   0 nick       (501) staff       (20)     4722 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/SOURCES.txt
--rw-r--r--   0 nick       (501) staff       (20)        1 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/dependency_links.txt
--rw-r--r--   0 nick       (501) staff       (20)      471 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/entry_points.txt
--rw-r--r--   0 nick       (501) staff       (20)      884 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/requires.txt
--rw-r--r--   0 nick       (501) staff       (20)       26 2024-01-25 21:23:31.000000 pyinfra-3.0b0/pyinfra.egg-info/top_level.txt
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.590184 pyinfra-3.0b0/pyinfra_cli/
--rw-r--r--   0 nick       (501) staff       (20)      284 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra_cli/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)      881 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/__main__.py
--rw-r--r--   0 nick       (501) staff       (20)     1761 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/commands.py
--rw-r--r--   0 nick       (501) staff       (20)     4806 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)     9513 2024-01-25 20:16:09.000000 pyinfra-3.0b0/pyinfra_cli/inventory.py
--rw-r--r--   0 nick       (501) staff       (20)      461 2024-01-25 20:01:15.000000 pyinfra-3.0b0/pyinfra_cli/inventory_dsl.py
--rw-r--r--   0 nick       (501) staff       (20)     2201 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/log.py
--rw-r--r--   0 nick       (501) staff       (20)    19667 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/main.py
--rw-r--r--   0 nick       (501) staff       (20)    11769 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyinfra_cli/prints.py
--rw-r--r--   0 nick       (501) staff       (20)     6322 2024-01-25 20:15:55.000000 pyinfra-3.0b0/pyinfra_cli/util.py
--rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:43.000000 pyinfra-3.0b0/pyinfra_cli/virtualenv.py
--rw-r--r--   0 nick       (501) staff       (20)      381 2024-01-24 10:33:33.000000 pyinfra-3.0b0/pyproject.toml
--rw-r--r--   0 nick       (501) staff       (20)      663 2024-01-25 21:23:31.595227 pyinfra-3.0b0/setup.cfg
--rw-r--r--   0 nick       (501) staff       (20)     4683 2024-01-24 10:36:25.000000 pyinfra-3.0b0/setup.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.591073 pyinfra-3.0b0/tests/
--rw-r--r--   0 nick       (501) staff       (20)      343 2022-09-25 11:45:43.000000 pyinfra-3.0b0/tests/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2254 2022-11-03 15:24:51.000000 pyinfra-3.0b0/tests/paramiko_util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.592437 pyinfra-3.0b0/tests/test_api/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b0/tests/test_api/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     2413 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_api/test_api.py
--rw-r--r--   0 nick       (501) staff       (20)     1961 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_api/test_api_arguments.py
--rw-r--r--   0 nick       (501) staff       (20)     3204 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_api/test_api_command.py
--rw-r--r--   0 nick       (501) staff       (20)      708 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_api/test_api_config.py
--rw-r--r--   0 nick       (501) staff       (20)     4200 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_api/test_api_deploys.py
--rw-r--r--   0 nick       (501) staff       (20)    10687 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_api/test_api_facts.py
--rw-r--r--   0 nick       (501) staff       (20)     1119 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_api/test_api_host.py
--rw-r--r--   0 nick       (501) staff       (20)     2013 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_api/test_api_inventory.py
--rw-r--r--   0 nick       (501) staff       (20)    20162 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_api/test_api_operations.py
--rw-r--r--   0 nick       (501) staff       (20)     1716 2024-01-23 20:10:51.000000 pyinfra-3.0b0/tests/test_api/test_api_util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.593396 pyinfra-3.0b0/tests/test_cli/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b0/tests/test_cli/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     6045 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_cli/test_cli.py
--rw-r--r--   0 nick       (501) staff       (20)     4858 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_cli/test_cli_deploy.py
--rw-r--r--   0 nick       (501) staff       (20)     3088 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_cli/test_cli_exceptions.py
--rw-r--r--   0 nick       (501) staff       (20)     2562 2024-01-23 20:10:49.000000 pyinfra-3.0b0/tests/test_cli/test_cli_util.py
--rw-r--r--   0 nick       (501) staff       (20)     2130 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_cli/test_context_objects.py
--rw-r--r--   0 nick       (501) staff       (20)      338 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_cli/util.py
-drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-01-25 21:23:31.594635 pyinfra-3.0b0/tests/test_connectors/
--rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b0/tests/test_connectors/__init__.py
--rw-r--r--   0 nick       (501) staff       (20)     5907 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_chroot.py
--rw-r--r--   0 nick       (501) staff       (20)     6566 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_docker.py
--rw-r--r--   0 nick       (501) staff       (20)     9303 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_dockerssh.py
--rw-r--r--   0 nick       (501) staff       (20)     7442 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_local.py
--rw-r--r--   0 nick       (501) staff       (20)    36438 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_ssh.py
--rw-r--r--   0 nick       (501) staff       (20)     5734 2024-01-23 20:10:51.000000 pyinfra-3.0b0/tests/test_connectors/test_sshuserclient.py
--rw-r--r--   0 nick       (501) staff       (20)     3807 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_terraform.py
--rw-r--r--   0 nick       (501) staff       (20)     4647 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_util.py
--rw-r--r--   0 nick       (501) staff       (20)     3630 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_connectors/test_vagrant.py
--rw-r--r--   0 nick       (501) staff       (20)     3308 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_facts.py
--rw-r--r--   0 nick       (501) staff       (20)     1696 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_global_arguments.py
--rw-r--r--   0 nick       (501) staff       (20)     6074 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/test_operations.py
--rw-r--r--   0 nick       (501) staff       (20)      557 2022-09-25 11:45:44.000000 pyinfra-3.0b0/tests/test_operations_utils.py
--rw-r--r--   0 nick       (501) staff       (20)    11745 2024-01-24 10:33:34.000000 pyinfra-3.0b0/tests/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:48.002053 pyinfra-3.0b1/
+-rw-r--r--   0 nick       (501) staff       (20)     1527 2024-05-04 19:18:52.000000 pyinfra-3.0b1/CHANGELOG.md
+-rw-r--r--   0 nick       (501) staff       (20)     1076 2021-01-18 10:52:39.000000 pyinfra-3.0b1/LICENSE.md
+-rw-r--r--   0 nick       (501) staff       (20)       59 2024-01-23 20:10:51.000000 pyinfra-3.0b1/MANIFEST.in
+-rw-r--r--   0 nick       (501) staff       (20)     5773 2024-05-04 19:20:48.002138 pyinfra-3.0b1/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     4577 2024-05-04 18:38:15.000000 pyinfra-3.0b1/README.md
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.983260 pyinfra-3.0b1/pyinfra/
+-rw-r--r--   0 nick       (501) staff       (20)      535 2024-01-03 20:23:54.000000 pyinfra-3.0b1/pyinfra/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)       47 2020-01-22 18:18:30.000000 pyinfra-3.0b1/pyinfra/__main__.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.985839 pyinfra-3.0b1/pyinfra/api/
+-rw-r--r--   0 nick       (501) staff       (20)      942 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     9748 2024-03-09 11:54:16.000000 pyinfra-3.0b1/pyinfra/api/arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     2254 2024-03-09 11:53:41.000000 pyinfra-3.0b1/pyinfra/api/arguments_typed.py
+-rw-r--r--   0 nick       (501) staff       (20)     7176 2024-03-02 11:45:52.000000 pyinfra-3.0b1/pyinfra/api/command.py
+-rw-r--r--   0 nick       (501) staff       (20)     4221 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/config.py
+-rw-r--r--   0 nick       (501) staff       (20)     1416 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/connect.py
+-rw-r--r--   0 nick       (501) staff       (20)      544 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/connectors.py
+-rw-r--r--   0 nick       (501) staff       (20)     2756 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/deploy.py
+-rw-r--r--   0 nick       (501) staff       (20)     1861 2024-03-02 11:46:27.000000 pyinfra-3.0b1/pyinfra/api/exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)    10282 2024-03-02 11:46:19.000000 pyinfra-3.0b1/pyinfra/api/facts.py
+-rw-r--r--   0 nick       (501) staff       (20)    13475 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra/api/host.py
+-rw-r--r--   0 nick       (501) staff       (20)     7663 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)    14789 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra/api/operation.py
+-rw-r--r--   0 nick       (501) staff       (20)    10894 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra/api/operations.py
+-rw-r--r--   0 nick       (501) staff       (20)    12622 2024-03-09 11:50:20.000000 pyinfra-3.0b1/pyinfra/api/state.py
+-rw-r--r--   0 nick       (501) staff       (20)    11977 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/api/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.987244 pyinfra-3.0b1/pyinfra/connectors/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/connectors/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     3756 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/base.py
+-rw-r--r--   0 nick       (501) staff       (20)     5931 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/chroot.py
+-rw-r--r--   0 nick       (501) staff       (20)     8964 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/docker.py
+-rw-r--r--   0 nick       (501) staff       (20)     8919 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/dockerssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     6929 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/local.py
+-rw-r--r--   0 nick       (501) staff       (20)    21018 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/ssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     3683 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/connectors/ssh_util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.987630 pyinfra-3.0b1/pyinfra/connectors/sshuserclient/
+-rw-r--r--   0 nick       (501) staff       (20)       44 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/connectors/sshuserclient/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     9720 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/connectors/sshuserclient/client.py
+-rw-r--r--   0 nick       (501) staff       (20)     2721 2023-01-15 18:23:08.000000 pyinfra-3.0b1/pyinfra/connectors/sshuserclient/config.py
+-rw-r--r--   0 nick       (501) staff       (20)     3617 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/terraform.py
+-rw-r--r--   0 nick       (501) staff       (20)    11326 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra/connectors/util.py
+-rw-r--r--   0 nick       (501) staff       (20)     4722 2024-03-09 11:49:30.000000 pyinfra-3.0b1/pyinfra/connectors/vagrant.py
+-rw-r--r--   0 nick       (501) staff       (20)     3394 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/context.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.992298 pyinfra-3.0b1/pyinfra/facts/
+-rw-r--r--   0 nick       (501) staff       (20)      347 2024-03-02 20:02:31.000000 pyinfra-3.0b1/pyinfra/facts/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      482 2024-01-23 20:10:49.000000 pyinfra-3.0b1/pyinfra/facts/apk.py
+-rw-r--r--   0 nick       (501) staff       (20)     1999 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/apt.py
+-rw-r--r--   0 nick       (501) staff       (20)     2266 2022-11-03 15:24:51.000000 pyinfra-3.0b1/pyinfra/facts/brew.py
+-rw-r--r--   0 nick       (501) staff       (20)      490 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/bsdinit.py
+-rw-r--r--   0 nick       (501) staff       (20)      531 2024-01-23 20:10:49.000000 pyinfra-3.0b1/pyinfra/facts/cargo.py
+-rw-r--r--   0 nick       (501) staff       (20)      703 2024-03-02 11:46:15.000000 pyinfra-3.0b1/pyinfra/facts/choco.py
+-rw-r--r--   0 nick       (501) staff       (20)     1666 2024-03-02 11:24:26.000000 pyinfra-3.0b1/pyinfra/facts/deb.py
+-rw-r--r--   0 nick       (501) staff       (20)      862 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/dnf.py
+-rw-r--r--   0 nick       (501) staff       (20)     1678 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/docker.py
+-rw-r--r--   0 nick       (501) staff       (20)    11475 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/files.py
+-rw-r--r--   0 nick       (501) staff       (20)      473 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/gem.py
+-rw-r--r--   0 nick       (501) staff       (20)     1294 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/git.py
+-rw-r--r--   0 nick       (501) staff       (20)     3729 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/gpg.py
+-rw-r--r--   0 nick       (501) staff       (20)    11402 2024-03-09 11:49:18.000000 pyinfra-3.0b1/pyinfra/facts/hardware.py
+-rw-r--r--   0 nick       (501) staff       (20)     3374 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/iptables.py
+-rw-r--r--   0 nick       (501) staff       (20)      668 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/launchd.py
+-rw-r--r--   0 nick       (501) staff       (20)      337 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/lxd.py
+-rw-r--r--   0 nick       (501) staff       (20)     5896 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/mysql.py
+-rw-r--r--   0 nick       (501) staff       (20)      674 2022-11-03 15:24:51.000000 pyinfra-3.0b1/pyinfra/facts/npm.py
+-rw-r--r--   0 nick       (501) staff       (20)     1350 2024-01-23 20:10:49.000000 pyinfra-3.0b1/pyinfra/facts/openrc.py
+-rw-r--r--   0 nick       (501) staff       (20)     1001 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/pacman.py
+-rw-r--r--   0 nick       (501) staff       (20)      702 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/pip.py
+-rw-r--r--   0 nick       (501) staff       (20)      452 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/pkg.py
+-rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/pkgin.py
+-rw-r--r--   0 nick       (501) staff       (20)     4094 2024-03-09 11:50:02.000000 pyinfra-3.0b1/pyinfra/facts/postgres.py
+-rw-r--r--   0 nick       (501) staff       (20)      187 2024-03-09 11:50:02.000000 pyinfra-3.0b1/pyinfra/facts/postgresql.py
+-rw-r--r--   0 nick       (501) staff       (20)     1973 2022-10-24 10:12:32.000000 pyinfra-3.0b1/pyinfra/facts/rpm.py
+-rw-r--r--   0 nick       (501) staff       (20)     4272 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/selinux.py
+-rw-r--r--   0 nick       (501) staff       (20)    19794 2024-03-09 11:49:18.000000 pyinfra-3.0b1/pyinfra/facts/server.py
+-rw-r--r--   0 nick       (501) staff       (20)     1910 2022-10-24 10:12:32.000000 pyinfra-3.0b1/pyinfra/facts/snap.py
+-rw-r--r--   0 nick       (501) staff       (20)     3927 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/systemd.py
+-rw-r--r--   0 nick       (501) staff       (20)     1490 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/sysvinit.py
+-rw-r--r--   0 nick       (501) staff       (20)      543 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/upstart.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.992717 pyinfra-3.0b1/pyinfra/facts/util/
+-rw-r--r--   0 nick       (501) staff       (20)      521 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/util/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      730 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/util/databases.py
+-rw-r--r--   0 nick       (501) staff       (20)     1090 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/facts/util/packaging.py
+-rw-r--r--   0 nick       (501) staff       (20)     2561 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/util/win_files.py
+-rw-r--r--   0 nick       (501) staff       (20)      591 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/vzctl.py
+-rw-r--r--   0 nick       (501) staff       (20)      481 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/xbps.py
+-rw-r--r--   0 nick       (501) staff       (20)      827 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/yum.py
+-rw-r--r--   0 nick       (501) staff       (20)      766 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/facts/zypper.py
+-rw-r--r--   0 nick       (501) staff       (20)     2751 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/local.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.996657 pyinfra-3.0b1/pyinfra/operations/
+-rw-r--r--   0 nick       (501) staff       (20)      357 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/operations/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2049 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/apk.py
+-rw-r--r--   0 nick       (501) staff       (20)    13526 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/apt.py
+-rw-r--r--   0 nick       (501) staff       (20)     5040 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/brew.py
+-rw-r--r--   0 nick       (501) staff       (20)     1578 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/bsdinit.py
+-rw-r--r--   0 nick       (501) staff       (20)     1042 2024-03-09 11:07:57.000000 pyinfra-3.0b1/pyinfra/operations/cargo.py
+-rw-r--r--   0 nick       (501) staff       (20)     1453 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/choco.py
+-rw-r--r--   0 nick       (501) staff       (20)     5550 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/dnf.py
+-rw-r--r--   0 nick       (501) staff       (20)    52485 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra/operations/files.py
+-rw-r--r--   0 nick       (501) staff       (20)     1070 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/gem.py
+-rw-r--r--   0 nick       (501) staff       (20)    11543 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/git.py
+-rw-r--r--   0 nick       (501) staff       (20)     9009 2024-03-02 11:46:12.000000 pyinfra-3.0b1/pyinfra/operations/iptables.py
+-rw-r--r--   0 nick       (501) staff       (20)     1164 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/launchd.py
+-rw-r--r--   0 nick       (501) staff       (20)     1639 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/lxd.py
+-rw-r--r--   0 nick       (501) staff       (20)    19141 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/mysql.py
+-rw-r--r--   0 nick       (501) staff       (20)     1404 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/npm.py
+-rw-r--r--   0 nick       (501) staff       (20)     1510 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/openrc.py
+-rw-r--r--   0 nick       (501) staff       (20)     1672 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/pacman.py
+-rw-r--r--   0 nick       (501) staff       (20)     5699 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/pip.py
+-rw-r--r--   0 nick       (501) staff       (20)     2222 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/pkg.py
+-rw-r--r--   0 nick       (501) staff       (20)     1930 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/pkgin.py
+-rw-r--r--   0 nick       (501) staff       (20)     9152 2024-03-09 11:50:02.000000 pyinfra-3.0b1/pyinfra/operations/postgres.py
+-rw-r--r--   0 nick       (501) staff       (20)      797 2024-03-09 11:50:02.000000 pyinfra-3.0b1/pyinfra/operations/postgresql.py
+-rw-r--r--   0 nick       (501) staff       (20)      797 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/operations/puppet.py
+-rw-r--r--   0 nick       (501) staff       (20)     1909 2024-03-03 19:50:28.000000 pyinfra-3.0b1/pyinfra/operations/python.py
+-rw-r--r--   0 nick       (501) staff       (20)     5347 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/selinux.py
+-rw-r--r--   0 nick       (501) staff       (20)    35710 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/server.py
+-rw-r--r--   0 nick       (501) staff       (20)     2987 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/snap.py
+-rw-r--r--   0 nick       (501) staff       (20)     5493 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/ssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     3818 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/systemd.py
+-rw-r--r--   0 nick       (501) staff       (20)     4003 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/sysvinit.py
+-rw-r--r--   0 nick       (501) staff       (20)     1908 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/upstart.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.997132 pyinfra-3.0b1/pyinfra/operations/util/
+-rw-r--r--   0 nick       (501) staff       (20)      366 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/util/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     3339 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/util/files.py
+-rw-r--r--   0 nick       (501) staff       (20)     8300 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/util/packaging.py
+-rw-r--r--   0 nick       (501) staff       (20)     1031 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/util/service.py
+-rw-r--r--   0 nick       (501) staff       (20)     3010 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/vzctl.py
+-rw-r--r--   0 nick       (501) staff       (20)     1446 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/xbps.py
+-rw-r--r--   0 nick       (501) staff       (20)     5543 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/yum.py
+-rw-r--r--   0 nick       (501) staff       (20)     5494 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra/operations/zypper.py
+-rw-r--r--   0 nick       (501) staff       (20)     4193 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/progress.py
+-rw-r--r--   0 nick       (501) staff       (20)        0 2024-01-23 20:10:51.000000 pyinfra-3.0b1/pyinfra/py.typed
+-rw-r--r--   0 nick       (501) staff       (20)      153 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra/version.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.983964 pyinfra-3.0b1/pyinfra.egg-info/
+-rw-r--r--   0 nick       (501) staff       (20)     5773 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/PKG-INFO
+-rw-r--r--   0 nick       (501) staff       (20)     4750 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 nick       (501) staff       (20)        1 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 nick       (501) staff       (20)      471 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/entry_points.txt
+-rw-r--r--   0 nick       (501) staff       (20)      884 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/requires.txt
+-rw-r--r--   0 nick       (501) staff       (20)       26 2024-05-04 19:20:47.000000 pyinfra-3.0b1/pyinfra.egg-info/top_level.txt
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.998214 pyinfra-3.0b1/pyinfra_cli/
+-rw-r--r--   0 nick       (501) staff       (20)      284 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra_cli/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)      881 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra_cli/__main__.py
+-rw-r--r--   0 nick       (501) staff       (20)     1832 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra_cli/commands.py
+-rw-r--r--   0 nick       (501) staff       (20)     4953 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra_cli/exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)     9513 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra_cli/inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)     2201 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra_cli/log.py
+-rw-r--r--   0 nick       (501) staff       (20)    19715 2024-03-04 22:12:09.000000 pyinfra-3.0b1/pyinfra_cli/main.py
+-rw-r--r--   0 nick       (501) staff       (20)     9006 2024-05-04 18:34:00.000000 pyinfra-3.0b1/pyinfra_cli/prints.py
+-rw-r--r--   0 nick       (501) staff       (20)     6322 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyinfra_cli/util.py
+-rw-r--r--   0 nick       (501) staff       (20)     2466 2022-09-25 11:45:43.000000 pyinfra-3.0b1/pyinfra_cli/virtualenv.py
+-rw-r--r--   0 nick       (501) staff       (20)      381 2024-02-28 10:18:03.000000 pyinfra-3.0b1/pyproject.toml
+-rw-r--r--   0 nick       (501) staff       (20)      663 2024-05-04 19:20:48.002467 pyinfra-3.0b1/setup.cfg
+-rw-r--r--   0 nick       (501) staff       (20)     4683 2024-02-28 10:18:03.000000 pyinfra-3.0b1/setup.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:47.998904 pyinfra-3.0b1/tests/
+-rw-r--r--   0 nick       (501) staff       (20)      343 2022-09-25 11:45:43.000000 pyinfra-3.0b1/tests/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2254 2022-11-03 15:24:51.000000 pyinfra-3.0b1/tests/paramiko_util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:48.000165 pyinfra-3.0b1/tests/test_api/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b1/tests/test_api/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     2413 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_api/test_api.py
+-rw-r--r--   0 nick       (501) staff       (20)     1961 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_api/test_api_arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     3204 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_api/test_api_command.py
+-rw-r--r--   0 nick       (501) staff       (20)      708 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_api/test_api_config.py
+-rw-r--r--   0 nick       (501) staff       (20)     4200 2024-03-09 11:52:48.000000 pyinfra-3.0b1/tests/test_api/test_api_deploys.py
+-rw-r--r--   0 nick       (501) staff       (20)    10687 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_api/test_api_facts.py
+-rw-r--r--   0 nick       (501) staff       (20)     1119 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_api/test_api_host.py
+-rw-r--r--   0 nick       (501) staff       (20)     2013 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_api/test_api_inventory.py
+-rw-r--r--   0 nick       (501) staff       (20)    20144 2024-05-04 18:34:00.000000 pyinfra-3.0b1/tests/test_api/test_api_operations.py
+-rw-r--r--   0 nick       (501) staff       (20)     1716 2024-01-23 20:10:51.000000 pyinfra-3.0b1/tests/test_api/test_api_util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:48.000872 pyinfra-3.0b1/tests/test_cli/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b1/tests/test_cli/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     6045 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_cli/test_cli.py
+-rw-r--r--   0 nick       (501) staff       (20)     4858 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_cli/test_cli_deploy.py
+-rw-r--r--   0 nick       (501) staff       (20)     3088 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_cli/test_cli_exceptions.py
+-rw-r--r--   0 nick       (501) staff       (20)     2562 2024-01-23 20:10:49.000000 pyinfra-3.0b1/tests/test_cli/test_cli_util.py
+-rw-r--r--   0 nick       (501) staff       (20)     2130 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_cli/test_context_objects.py
+-rw-r--r--   0 nick       (501) staff       (20)      338 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_cli/util.py
+drwxr-xr-x   0 nick       (501) staff       (20)        0 2024-05-04 19:20:48.001959 pyinfra-3.0b1/tests/test_connectors/
+-rw-r--r--   0 nick       (501) staff       (20)        0 2020-01-15 13:37:52.000000 pyinfra-3.0b1/tests/test_connectors/__init__.py
+-rw-r--r--   0 nick       (501) staff       (20)     5907 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_connectors/test_chroot.py
+-rw-r--r--   0 nick       (501) staff       (20)     6566 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_connectors/test_docker.py
+-rw-r--r--   0 nick       (501) staff       (20)     9303 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_connectors/test_dockerssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     7442 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_connectors/test_local.py
+-rw-r--r--   0 nick       (501) staff       (20)    38399 2024-03-02 11:24:41.000000 pyinfra-3.0b1/tests/test_connectors/test_ssh.py
+-rw-r--r--   0 nick       (501) staff       (20)     5734 2024-01-23 20:10:51.000000 pyinfra-3.0b1/tests/test_connectors/test_sshuserclient.py
+-rw-r--r--   0 nick       (501) staff       (20)     3743 2024-03-09 11:52:48.000000 pyinfra-3.0b1/tests/test_connectors/test_terraform.py
+-rw-r--r--   0 nick       (501) staff       (20)     4647 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_connectors/test_util.py
+-rw-r--r--   0 nick       (501) staff       (20)     3646 2024-03-09 11:49:30.000000 pyinfra-3.0b1/tests/test_connectors/test_vagrant.py
+-rw-r--r--   0 nick       (501) staff       (20)     3308 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_facts.py
+-rw-r--r--   0 nick       (501) staff       (20)     1696 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_global_arguments.py
+-rw-r--r--   0 nick       (501) staff       (20)     6074 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/test_operations.py
+-rw-r--r--   0 nick       (501) staff       (20)      557 2022-09-25 11:45:44.000000 pyinfra-3.0b1/tests/test_operations_utils.py
+-rw-r--r--   0 nick       (501) staff       (20)    11745 2024-02-28 10:18:03.000000 pyinfra-3.0b1/tests/util.py
```

### Comparing `pyinfra-3.0b0/CHANGELOG.md` & `pyinfra-3.0b1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# v3.0.beta0
+# v3.0.beta1
 
 Welcome to pyinfra v3! This version is the biggest overhaul of pyinfra since it was created back in 2015. Most v2 deployment code should be automatically compatible, but as always be aware. Major changes:
 
 ## Runtime operation execution
 
 pyinfra now executes operations at runtime, rather than pre-generating commands. Although the change isn't noticeable this fixes an entire class of bugs and confusion. See the [limitations](https://docs.pyinfra.com/en/2.x/deploy-process.html#limitations) section in the v2 docs. All of those issues are now a thing of the past.
```

### Comparing `pyinfra-3.0b0/LICENSE.md` & `pyinfra-3.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/PKG-INFO` & `pyinfra-3.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra
-Version: 3.0b0
+Version: 3.0b1
 Summary: pyinfra automates/provisions/manages/deploys infrastructure.
 Home-page: https://pyinfra.com
 Author: Nick / Fizzadar
 Author-email: pointlessrambler@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/Fizzadar/pyinfra
@@ -31,33 +31,33 @@
 
 <p align="center">
     <a href="https://pyinfra.com">
         <img src="https://pyinfra.com/static/logo_readme.png" alt="pyinfra" />
     </a>
 </p>
 
-<p align="center">
+<p>
     <strong>Note: this is the v3 branch, which is currently in beta. <a href="https://docs.pyinfra.com/en/next">See the docs for v3</a>. If needed the <a href="https://github.com/pyinfra-dev/pyinfra/tree/2.x/">2.x branch is here</a>, but is in bugfix only mode.</strong>
 </p>
 
-<p align="center">
-    <em>pyinfra automates infrastructure using Python. It’s fast and scales from one server to thousands. Great for ad-hoc command execution, service deployment, configuration management and more.</em>
+<p>
+    pyinfra turns Python code into shell commands and runs them on your servers. Execute ad-hoc commands and write declarative operations. Target SSH servers, local machine and Docker containers. Fast and scales from one server to thousands. Think <code>ansible</code> but Python instead of YAML, and a lot faster.
 </p>
 
 ---
 
-<p align="center">
+<p>
     <a href="https://docs.pyinfra.com"><strong>Documentation</strong></a> &rArr;
     <a href="https://docs.pyinfra.com/page/getting-started.html"><strong>Getting Started</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/examples.html"><strong>Examples</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/support.html"><strong>Help & Support</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/contributing.html"><strong>Contributing</strong></a>
 </p>
 
-<p align="center">
+<p>
     Chat &rArr;
     <a href="https://matrix.to/#/#pyinfra:matrix.org"><strong><code>#pyinfra</code> on Matrix</strong></a>
 </p>
 
 ---
 
 Why pyinfra? Design features include:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra Version: 3.0b0 Summary: pyinfra automates/
+Metadata-Version: 2.1 Name: pyinfra Version: 3.0b1 Summary: pyinfra automates/
 provisions/manages/deploys infrastructure. Home-page: https://pyinfra.com
 Author: Nick / Fizzadar Author-email: pointlessrambler@gmail.com License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com Project-URL: GitHub,
 https://github.com/Fizzadar/pyinfra Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology Classifier: License ::
@@ -11,22 +11,23 @@
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: System :: Systems
 Administration Classifier: Topic :: System :: Installation/Setup Classifier:
 Topic :: Utilities Description-Content-Type: text/markdown Provides-Extra: test
 Provides-Extra: docs Provides-Extra: dev License-File: LICENSE.md
                                    _[_p_y_i_n_f_r_a_]
- NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
-         IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
-ppyyiinnffrraa aauuttoommaatteess iinnffrraassttrruuccttuurree uussiinngg PPyytthhoonn.. IItt?â??ss ffaasstt aanndd ssccaalleess ffrroomm oonnee
- sseerrvveerr ttoo tthhoouussaannddss.. GGrreeaatt ffoorr aadd--hhoocc ccoommmmaanndd eexxeeccuuttiioonn,, sseerrvviiccee ddeeppllooyymmeenntt,,
-                      ccoonnffiigguurraattiioonn mmaannaaggeemmeenntt aanndd mmoorree..
+NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
+IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
+pyinfra turns Python code into shell commands and runs them on your servers.
+Execute ad-hoc commands and write declarative operations. Target SSH servers,
+local machine and Docker containers. Fast and scales from one server to
+thousands. Think ansible but Python instead of YAML, and a lot faster.
 ---
-  _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
-                           Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
+_DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
+Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
 --- Why pyinfra? Design features include: + ð **Super fast** execution over
 thousands of hosts with predictable performance. + ð¨ **Instant debugging**
 with realtime stdin/stdout/stderr output (`-vvv`). + ð **Idempotent
 operations** that enable diffs and dry runs before making changes. + ð¦
 **Extendable** with the entire Python package ecosystem. + ð» **Agentless
 execution** against anything with shell access. + ð **Integrated** with
 connectors for Docker, Terraform, Vagrant and more. [https://pyinfra.com/
```

### Comparing `pyinfra-3.0b0/README.md` & `pyinfra-3.0b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 <p align="center">
     <a href="https://pyinfra.com">
         <img src="https://pyinfra.com/static/logo_readme.png" alt="pyinfra" />
     </a>
 </p>
 
-<p align="center">
+<p>
     <strong>Note: this is the v3 branch, which is currently in beta. <a href="https://docs.pyinfra.com/en/next">See the docs for v3</a>. If needed the <a href="https://github.com/pyinfra-dev/pyinfra/tree/2.x/">2.x branch is here</a>, but is in bugfix only mode.</strong>
 </p>
 
-<p align="center">
-    <em>pyinfra automates infrastructure using Python. It’s fast and scales from one server to thousands. Great for ad-hoc command execution, service deployment, configuration management and more.</em>
+<p>
+    pyinfra turns Python code into shell commands and runs them on your servers. Execute ad-hoc commands and write declarative operations. Target SSH servers, local machine and Docker containers. Fast and scales from one server to thousands. Think <code>ansible</code> but Python instead of YAML, and a lot faster.
 </p>
 
 ---
 
-<p align="center">
+<p>
     <a href="https://docs.pyinfra.com"><strong>Documentation</strong></a> &rArr;
     <a href="https://docs.pyinfra.com/page/getting-started.html"><strong>Getting Started</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/examples.html"><strong>Examples</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/support.html"><strong>Help & Support</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/contributing.html"><strong>Contributing</strong></a>
 </p>
 
-<p align="center">
+<p>
     Chat &rArr;
     <a href="https://matrix.to/#/#pyinfra:matrix.org"><strong><code>#pyinfra</code> on Matrix</strong></a>
 </p>
 
 ---
 
 Why pyinfra? Design features include:
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
                                    _[_p_y_i_n_f_r_a_]
- NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
-         IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
-ppyyiinnffrraa aauuttoommaatteess iinnffrraassttrruuccttuurree uussiinngg PPyytthhoonn.. IItt?â??ss ffaasstt aanndd ssccaalleess ffrroomm oonnee
- sseerrvveerr ttoo tthhoouussaannddss.. GGrreeaatt ffoorr aadd--hhoocc ccoommmmaanndd eexxeeccuuttiioonn,, sseerrvviiccee ddeeppllooyymmeenntt,,
-                      ccoonnffiigguurraattiioonn mmaannaaggeemmeenntt aanndd mmoorree..
+NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
+IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
+pyinfra turns Python code into shell commands and runs them on your servers.
+Execute ad-hoc commands and write declarative operations. Target SSH servers,
+local machine and Docker containers. Fast and scales from one server to
+thousands. Think ansible but Python instead of YAML, and a lot faster.
 ---
-  _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
-                           Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
+_DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
+Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
 --- Why pyinfra? Design features include: + ð **Super fast** execution over
 thousands of hosts with predictable performance. + ð¨ **Instant debugging**
 with realtime stdin/stdout/stderr output (`-vvv`). + ð **Idempotent
 operations** that enable diffs and dry runs before making changes. + ð¦
 **Extendable** with the entire Python package ecosystem. + ð» **Agentless
 execution** against anything with shell access. + ð **Integrated** with
 connectors for Docker, Terraform, Vagrant and more. [https://pyinfra.com/
```

### Comparing `pyinfra-3.0b0/pyinfra/__init__.py` & `pyinfra-3.0b1/pyinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/__init__.py` & `pyinfra-3.0b1/pyinfra/api/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     RsyncCommand,
     StringCommand,
 )
 from .config import Config  # noqa: F401 # pragma: no cover
 from .deploy import deploy  # noqa: F401 # pragma: no cover
 from .exceptions import DeployError  # noqa: F401 # pragma: no cover
 from .exceptions import (  # noqa: F401
+    FactError,
+    FactTypeError,
+    FactValueError,
     InventoryError,
     OperationError,
     OperationTypeError,
     OperationValueError,
 )
 from .facts import FactBase, ShortFactBase  # noqa: F401 # pragma: no cover
 from .host import Host  # noqa: F401 # pragma: no cover
```

### Comparing `pyinfra-3.0b0/pyinfra/api/arguments.py` & `pyinfra-3.0b1/pyinfra/api/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
+    List,
     Mapping,
     Optional,
     TypeVar,
     Union,
     cast,
     get_type_hints,
 )
@@ -165,15 +166,15 @@
 # These provide/extend additional operation metadata
 
 
 class MetaArguments(TypedDict):
     name: str
     _ignore_errors: bool
     _continue_on_error: bool
-    _if: Callable[[], bool]
+    _if: List[Callable[[], bool]]
 
 
 meta_argument_meta: dict[str, ArgumentMeta] = {
     # NOTE: name is the only non-_-prefixed argument
     "name": ArgumentMeta(
         "Name of the operation.",
         default=lambda _: None,
@@ -186,16 +187,16 @@
         (
             "Continue executing operation commands after error. "
             "Only applies when ``_ignore_errors`` is true."
         ),
         default=lambda _: False,
     ),
     "_if": ArgumentMeta(
-        "Only run this operation if this function returns True",
-        default=lambda _: None,
+        "Only run this operation if these functions returns True",
+        default=lambda _: [],
     ),
 }
 
 
 # Execution arguments
 # These alter how pyinfra is to execute an operation. Notably these must all have the same value
 # over every target host for the same operation.
@@ -295,15 +296,15 @@
     state = state or context.state
     host = host or context.host
 
     config = state.config
     if context.ctx_config.isset():
         config = context.config
 
-    meta_kwargs = host.current_deploy_kwargs or {}
+    meta_kwargs: dict[str, Any] = host.current_deploy_kwargs or {}  # type: ignore[assignment]
 
     arguments: dict[str, Any] = {}
     found_keys: list[str] = []
 
     for key, type_ in get_type_hints(AllArguments).items():
         if keys_to_check and key not in keys_to_check:
             continue
```

### Comparing `pyinfra-3.0b0/pyinfra/api/arguments_typed.py` & `pyinfra-3.0b1/pyinfra/api/arguments_typed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Generator, Generic, Iterable, Mapping, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Callable,
+    Generator,
+    Generic,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Union,
+)
 
 from typing_extensions import ParamSpec, Protocol
 
 if TYPE_CHECKING:
     from pyinfra.api.operation import OperationMeta
 
 P = ParamSpec("P")
@@ -47,15 +57,15 @@
         _stdin: Union[None, str, list[str], tuple[str, ...]] = None,
         #
         # MetaArguments
         #
         name: Optional[str] = None,
         _ignore_errors: bool = False,
         _continue_on_error: bool = False,
-        _if: Optional[Callable[[], bool]] = None,
+        _if: Optional[List[Callable[[], bool]]] = None,
         #
         # ExecutionArguments
         #
         _parallel: Optional[int] = None,
         _run_once: bool = False,
         _serial: bool = False,
         #
```

### Comparing `pyinfra-3.0b0/pyinfra/api/command.py` & `pyinfra-3.0b1/pyinfra/api/command.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/config.py` & `pyinfra-3.0b1/pyinfra/api/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/connect.py` & `pyinfra-3.0b1/pyinfra/api/connect.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/connectors.py` & `pyinfra-3.0b1/pyinfra/api/connectors.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/deploy.py` & `pyinfra-3.0b1/pyinfra/api/deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/exceptions.py` & `pyinfra-3.0b1/pyinfra/api/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,33 @@
 
 class ConnectError(PyinfraError):
     """
     Exception raised when connecting fails.
     """
 
 
+class FactError(PyinfraError):
+    """
+    Exception raised during fact gathering staging if a fact is unable to
+    generate output/change state.
+    """
+
+
+class FactTypeError(FactError, TypeError):
+    """
+    Exception raised when a fact is passed invalid argument types.
+    """
+
+
+class FactValueError(FactError, ValueError):
+    """
+    Exception raised when a fact is passed invalid argument values.
+    """
+
+
 class OperationError(PyinfraError):
     """
     Exception raised during fact gathering staging if an operation is unable to
     generate output/change state.
     """
```

### Comparing `pyinfra-3.0b0/pyinfra/api/facts.py` & `pyinfra-3.0b1/pyinfra/api/facts.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 from .arguments import CONNECTOR_ARGUMENT_KEYS
 
 if TYPE_CHECKING:
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
-SUDO_REGEX = r"^sudo: unknown user:"
+SUDO_REGEX = r"^sudo: unknown user"
 SU_REGEXES = (
     r"^su: user .+ does not exist",
     r"^su: unknown login",
 )
 
 
 T = TypeVar("T")
```

### Comparing `pyinfra-3.0b0/pyinfra/api/host.py` & `pyinfra-3.0b1/pyinfra/api/host.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Callable, Generator, Optional, Type, TypeVar, Union, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Generator,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
 from uuid import uuid4
 
 import click
+from typing_extensions import Unpack
 
 from pyinfra import logger
 from pyinfra.connectors.base import BaseConnector
 from pyinfra.connectors.util import CommandOutput, remove_any_sudo_askpass_file
 
 from .connectors import get_execution_connector
 from .exceptions import ConnectError
@@ -94,19 +106,24 @@
 
     # Current context inside an @operation function (op gen stage)
     in_op: bool = False
     in_callback_op: bool = False
     current_op_hash: Optional[str] = None
     current_op_global_arguments: Optional["AllArguments"] = None
 
-    # Current context inside a @deploy function (op gen stage)
+    # Current context inside a @deploy function which become part of the op data
     in_deploy: bool = False
     current_deploy_name: Optional[str] = None
     current_deploy_kwargs = None
-    current_deploy_data = None
+
+    # @deploy decorator data is a bit different - we need to handle the case
+    # where we're evaluating an operation at runtime (current_op_) but also
+    # when ordering operations (current_) outside of an operation context.
+    current_op_deploy_data: Optional[dict[str, Any]] = None
+    current_deploy_data: Optional[dict[str, Any]] = None
 
     # Current context during operation execution
     executing_op_hash: Optional[str] = None
     nested_executing_op_hash: Optional[str] = None
 
     loop_position: list[int]
 
@@ -200,28 +217,43 @@
         log_func(f"{self.print_prefix}{message}")
 
     def log_styled(self, message, log_func=logger.info, **kwargs):
         message_styled = click.style(message, **kwargs)
         self.log(message_styled, log_func=log_func)
 
     def get_deploy_data(self):
-        if self.current_deploy_data:
-            return self.current_deploy_data
-        return {}
+        return self.current_op_deploy_data or self.current_deploy_data or {}
 
     def noop(self, description):
         """
         Log a description for a noop operation.
         """
 
         handler = logger.info if self.state.print_noop_info else logger.debug
         handler("{0}noop: {1}".format(self.print_prefix, description))
 
+    def when(self, condition: Callable[[], bool]):
+        return self.deploy(
+            "",
+            cast("AllArguments", {"_if": [condition]}),
+            {},
+            in_deploy=False,
+        )
+
+    def arguments(self, **arguments: Unpack["AllArguments"]):
+        return self.deploy("", arguments, {}, in_deploy=False)
+
     @contextmanager
-    def deploy(self, name: str, kwargs, data, in_deploy: bool = True):
+    def deploy(
+        self,
+        name: str,
+        kwargs: Optional["AllArguments"],
+        data: Optional[dict],
+        in_deploy: bool = True,
+    ):
         """
         Wraps a group of operations as a deploy, this should not be used
         directly, instead use ``pyinfra.api.deploy.deploy``.
         """
 
         # Handle nested deploy names
         if self.current_deploy_name:
@@ -230,14 +262,21 @@
         # Store the previous values
         old_in_deploy = self.in_deploy
         old_deploy_name = self.current_deploy_name
         old_deploy_kwargs = self.current_deploy_kwargs
         old_deploy_data = self.current_deploy_data
         self.in_deploy = in_deploy
 
+        # Combine any old _ifs with the new ones
+        if old_deploy_kwargs and kwargs:
+            old_ifs = old_deploy_kwargs["_if"]
+            new_ifs = kwargs["_if"]
+            if old_ifs and new_ifs:
+                kwargs["_if"] = old_ifs + new_ifs
+
         # Set the new values
         self.current_deploy_name = name
         self.current_deploy_kwargs = kwargs
         self.current_deploy_data = data
         logger.debug(
             "Starting deploy %s (args=%r, data=%r)",
             name,
```

### Comparing `pyinfra-3.0b0/pyinfra/api/inventory.py` & `pyinfra-3.0b1/pyinfra/api/inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/api/operation.py` & `pyinfra-3.0b1/pyinfra/api/operation.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from __future__ import annotations
 
 from functools import wraps
 from inspect import signature
 from io import StringIO
 from types import FunctionType
-from typing import Any, Callable, Generator, Iterator, Optional, cast
+from typing import TYPE_CHECKING, Any, Callable, Generator, Iterator, Optional, cast
 
 from typing_extensions import ParamSpec
 
 import pyinfra
 from pyinfra import context, logger
 from pyinfra.context import ctx_host, ctx_state
 
@@ -32,104 +32,119 @@
     get_operation_order_from_stack,
     log_operation_start,
     make_hash,
 )
 
 op_meta_default = object()
 
+if TYPE_CHECKING:
+    from pyinfra.connectors.util import CommandOutput
+
 
 class OperationMeta:
     _hash: str
 
-    _combined_output_lines = None
+    _combined_output: Optional["CommandOutput"] = None
     _commands: Optional[list[Any]] = None
-    _maybe_is_change: bool = False
+    _maybe_is_change: Optional[bool] = False
     _success: Optional[bool] = None
 
-    def __init__(self, hash, is_change=False):
+    def __init__(self, hash, is_change: Optional[bool]):
         self._hash = hash
         self._maybe_is_change = is_change
 
     def __repr__(self) -> str:
         """
         Return Operation object as a string.
         """
 
         if self._commands is not None:
             return (
                 "OperationMeta(executed=True, "
-                f"changed={self.did_change()}, hash={self._hash}, commands={len(self._commands)})"
+                f"success={self.did_succeed}, hash={self._hash}, commands={len(self._commands)})"
             )
         return (
             "OperationMeta(executed=False, "
             f"maybeChange={self._maybe_is_change}, hash={self._hash})"
         )
 
     # Completion & status checks
     def set_complete(
         self,
         success: bool,
         commands: list[Any],
-        combined_output_lines,
+        combined_output: "CommandOutput",
     ) -> None:
         if self.is_complete():
             raise RuntimeError("Cannot complete an already complete operation")
         self._success = success
         self._commands = commands
-        self._combined_output_lines = combined_output_lines
+        self._combined_output = combined_output
 
     def is_complete(self) -> bool:
         return self._success is not None
 
     def _raise_if_not_complete(self) -> None:
         if not self.is_complete():
             raise RuntimeError("Cannot evaluate operation result before execution")
 
-    def did_change(self) -> bool:
-        self._raise_if_not_complete()
+    def _did_change(self) -> bool:
         return bool(self._success and len(self._commands or []) > 0)
 
+    @property
+    def did_change(self):
+        return context.host.when(self._did_change)
+
+    @property
+    def did_not_change(self):
+        return context.host.when(lambda: not self._did_change())
+
     def did_succeed(self) -> bool:
         self._raise_if_not_complete()
         return self._success is True
 
     def did_error(self) -> bool:
         self._raise_if_not_complete()
         return self._success is False
 
-    # Output lines
-    def _get_lines(self, types=("stdout", "stderr")):
-        self._raise_if_not_complete()
-        assert self._combined_output_lines is not None
-        return [line for type_, line in self._combined_output_lines if type_ in types]
+    # TODO: deprecated, remove in v4
+    @property
+    def changed(self) -> bool:
+        if self.is_complete():
+            return self._did_change()
+
+        if self._maybe_is_change is not None:
+            return self._maybe_is_change
+
+        op_data = context.state.get_op_data_for_host(context.host, self._hash)
+        cmd_gen = op_data.command_generator
+        for _ in cmd_gen():
+            return True
+        return False
 
     @property
-    def stdout_lines(self):
-        return self._get_lines(types=("stdout",))
+    def stdout_lines(self) -> list[str]:
+        self._raise_if_not_complete()
+        assert self._combined_output is not None
+        return self._combined_output.stdout_lines
 
     @property
-    def stderr_lines(self):
-        return self._get_lines(types=("stderr",))
+    def stderr_lines(self) -> list[str]:
+        self._raise_if_not_complete()
+        assert self._combined_output is not None
+        return self._combined_output.stderr_lines
 
     @property
     def stdout(self) -> str:
         return "\n".join(self.stdout_lines)
 
     @property
     def stderr(self) -> str:
         return "\n".join(self.stderr_lines)
 
-    # TODO: deprecated, remove in v4
-    @property
-    def changed(self) -> int:
-        if not self.is_complete():
-            logger.warning("Checking changed before execution can give unexpected results")
-            return self._maybe_is_change
-        return self.did_change()
-
 
 def add_op(state: State, op_func, *args, **kwargs):
     """
     Prepare & add an operation to ``pyinfra.state`` by executing it on all hosts.
 
     Args:
         state (``pyinfra.api.State`` obj): the deploy state to add the operation
@@ -160,25 +175,29 @@
 
 P = ParamSpec("P")
 
 
 def operation(
     is_idempotent: bool = True,
     idempotent_notice: Optional[str] = None,
+    is_deprecated: bool = False,
+    deprecated_for: Optional[str] = None,
     _set_in_op: bool = True,
 ) -> Callable[[Callable[P, Generator]], PyinfraOperation[P]]:
     """
     Decorator that takes a simple module function and turn it into the internal
     operation representation that consists of a list of commands + options
     (sudo, (sudo|su)_user, env).
     """
 
     def decorator(f: Callable[P, Generator]) -> PyinfraOperation[P]:
         f.is_idempotent = is_idempotent  # type: ignore[attr-defined]
         f.idempotent_notice = idempotent_notice  # type: ignore[attr-defined]
+        f.is_deprecated = is_deprecated  # type: ignore[attr-defined]
+        f.deprecated_for = deprecated_for  # type: ignore[attr-defined]
         return _wrap_operation(f, _set_in_op=_set_in_op)
 
     return decorator
 
 
 def _wrap_operation(func: Callable[P, Generator], _set_in_op: bool = True) -> PyinfraOperation[P]:
     @wraps(func)
@@ -188,14 +207,23 @@
 
         if host.in_op:
             raise Exception(
                 "Operation called within another operation, this is not allowed! Use the `_inner` "
                 + "function to call the underlying operation."
             )
 
+        if func.is_deprecated:  # type: ignore[attr-defined]
+            if func.deprecated_for:  # type: ignore[attr-defined]
+                logger.warning(
+                    f"The {get_operation_name_from_func(func)} operation is "
+                    + f"deprecated, please use: {func.deprecated_for}",  # type: ignore[attr-defined] # noqa
+                )
+            else:
+                logger.warning(f"The {get_operation_name_from_func(func)} operation is deprecated")
+
         # Configure operation
         #
         # Get the meta kwargs (globals that apply to all hosts)
         global_arguments, global_argument_keys = pop_global_arguments(kwargs)
 
         names, add_args = generate_operation_name(func, host, kwargs, global_arguments)
         op_order, op_hash = solve_operation_consistency(names, state, host)
@@ -213,44 +241,52 @@
             has_run = False
             for ops in state.ops.values():
                 if op_hash in ops:
                     has_run = True
                     break
 
             if has_run:
-                return OperationMeta(op_hash)
+                return OperationMeta(op_hash, is_change=False)
+
+        # Grab a reference to any *current* deploy data as this may change when
+        # we later evaluate the operation at runtime.This means we put back the
+        # expected deploy data.
+        current_deploy_data = host.current_deploy_data
 
         # "Run" operation - here we make a generator that will yield out actual commands to execute
         # and, if we're diff-ing, we then iterate the generator now to determine if any changes
         # *would* be made based on the *current* remote state.
 
         def command_generator() -> Iterator[PyinfraCommand]:
             # Check global _if_ argument function and do nothing if returns False
             if state.is_executing:
-                _if = global_arguments.get("_if")
-                if _if and _if() is False:
+                _ifs = global_arguments.get("_if")
+                if _ifs and not all(_if() for _if in _ifs):
                     return
 
             host.in_op = _set_in_op
             host.current_op_hash = op_hash
             host.current_op_global_arguments = global_arguments
+            host.current_op_deploy_data = current_deploy_data
 
             try:
                 for command in func(*args, **kwargs):
                     if isinstance(command, str):
                         command = StringCommand(command.strip())
                     yield command
             finally:
                 host.in_op = False
                 host.current_op_hash = None
                 host.current_op_global_arguments = None
+                host.current_op_deploy_data = None
 
-        op_is_change = False
+        op_is_change = None
         if state.should_check_for_changes():
-            for command in command_generator():
+            op_is_change = False
+            for _ in command_generator():
                 op_is_change = True
                 break
         else:
             # If not calling the op function to check for change we still want to ensure the args
             # are valid, so use Signature.bind to trigger any TypeError.
             signature(func).bind(*args, **kwargs)
 
@@ -275,30 +311,32 @@
         # Return result meta for use in deploy scripts
         return operation_meta
 
     decorated_func._inner = func  # type: ignore[attr-defined]
     return cast(PyinfraOperation[P], decorated_func)
 
 
+def get_operation_name_from_func(func):
+    if func.__module__:
+        module_bits = func.__module__.split(".")
+        module_name = module_bits[-1]
+        return "{0}.{1}".format(module_name, func.__name__)
+    else:
+        return func.__name__
+
+
 def generate_operation_name(func, host, kwargs, global_arguments):
     # Generate an operation name if needed (Module/Operation format)
     name = global_arguments.get("name")
     add_args = False
     if name:
         names = {name}
     else:
         add_args = True
-
-        if func.__module__:
-            module_bits = func.__module__.split(".")
-            module_name = module_bits[-1]
-            name = "{0}/{1}".format(module_name.title(), func.__name__.title())
-        else:
-            name = func.__name__
-
+        name = get_operation_name_from_func(func)
         names = {name}
 
     if host.current_deploy_name:
         names = {"{0} | {1}".format(host.current_deploy_name, name) for name in names}
 
     return names, add_args
```

### Comparing `pyinfra-3.0b0/pyinfra/api/operations.py` & `pyinfra-3.0b1/pyinfra/api/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,25 +63,24 @@
     global_arguments = op_data.global_arguments
 
     ignore_errors = global_arguments["_ignore_errors"]
     continue_on_error = global_arguments["_continue_on_error"]
     timeout = global_arguments.get("_timeout", 0)
 
     executor_kwarg_keys = CONNECTOR_ARGUMENT_KEYS
-    base_connector_arguments: ConnectorArguments = (
-        cast(  # https://github.com/python/mypy/issues/10371
-            ConnectorArguments,
-            {key: global_arguments[key] for key in executor_kwarg_keys if key in global_arguments},
-        )
+    # See: https://github.com/python/mypy/issues/10371
+    base_connector_arguments: ConnectorArguments = cast(
+        ConnectorArguments,
+        {key: global_arguments[key] for key in executor_kwarg_keys if key in global_arguments},  # type: ignore[literal-required] # noqa
     )
 
     did_error = False
     executed_commands = 0
     commands = []
-    all_combined_output_lines: list[OutputLine] = []
+    all_output_lines: list[OutputLine] = []
 
     for command in op_data.command_generator():
         commands.append(command)
 
         status = False
 
         connector_arguments = base_connector_arguments.copy()
@@ -99,27 +98,27 @@
                 host.log_styled(
                     f"Unexpected error in Python callback: {format_exception(e)}",
                     fg="red",
                     log_func=logger.warning,
                 )
 
         elif isinstance(command, StringCommand):
-            combined_output_lines = CommandOutput([])
+            output_lines = CommandOutput([])
             try:
-                status, combined_output_lines = command.execute(
+                status, output_lines = command.execute(
                     state,
                     host,
                     connector_arguments,
                 )
             except (timeout_error, socket_error, SSHException) as e:
                 log_host_command_error(host, e, timeout=timeout)
-            all_combined_output_lines.extend(combined_output_lines)
+            all_output_lines.extend(output_lines)
             # If we failed and have not already printed the stderr, print it
             if status is False and not state.print_output:
-                print_host_combined_output(host, combined_output_lines)
+                print_host_combined_output(host, output_lines)
 
         else:
             try:
                 status = command.execute(state, host, connector_arguments)
             except (timeout_error, socket_error, SSHException, IOError) as e:
                 log_host_command_error(host, e, timeout=timeout)
 
@@ -166,15 +165,15 @@
 
         # Unignored error -> False
         state.trigger_callbacks("operation_host_error", host, op_hash)
 
     op_data.operation_meta.set_complete(
         op_success,
         commands,
-        all_combined_output_lines,
+        CommandOutput(all_output_lines),
     )
 
     return return_status
 
 
 # Run all operations strategies
 #
```

### Comparing `pyinfra-3.0b0/pyinfra/api/state.py` & `pyinfra-3.0b1/pyinfra/api/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,18 +340,27 @@
 
     def get_meta_for_host(self, host: "Host") -> StateHostMeta:
         return self.meta[host]
 
     def get_results_for_host(self, host: "Host") -> StateHostResults:
         return self.results[host]
 
-    def get_op_data_for_host(self, host: "Host", op_hash: str):
+    def get_op_data_for_host(
+        self,
+        host: "Host",
+        op_hash: str,
+    ) -> StateOperationHostData:
         return self.ops[host][op_hash]
 
-    def set_op_data_for_host(self, host: "Host", op_hash: str, op_data: StateOperationHostData):
+    def set_op_data_for_host(
+        self,
+        host: "Host",
+        op_hash: str,
+        op_data: StateOperationHostData,
+    ):
         self.ops[host][op_hash] = op_data
 
     def activate_host(self, host: "Host"):
         """
         Flag a host as active.
         """
```

### Comparing `pyinfra-3.0b0/pyinfra/api/util.py` & `pyinfra-3.0b1/pyinfra/api/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/connectors/base.py` & `pyinfra-3.0b1/pyinfra/connectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     def __init__(self, state: "State", host: "Host"):
         self.state = state
         self.host = host
         self.data = host_to_connector_data(self.data_cls, self.data_meta, host.data)
 
     @staticmethod
     @abc.abstractmethod
-    def make_names_data(id: str) -> Iterator[tuple[str, dict, list[str]]]:
+    def make_names_data(name: str) -> Iterator[tuple[str, dict, list[str]]]:
         """
         Generates hosts/data/groups information for inventory. This allows a
         single connector reference to generate multiple target hosts.
         """
         ...
 
     def connect(self) -> None:
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/chroot.py` & `pyinfra-3.0b1/pyinfra/connectors/chroot.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,40 +36,39 @@
     local: LocalConnector
 
     def __init__(self, state: "State", host: "Host"):
         super().__init__(state, host)
         self.local = LocalConnector(state, host)
 
     @staticmethod
-    def make_names_data(directory: Optional[str] = None):
-        if not directory:
+    def make_names_data(name: Optional[str] = None):
+        if not name:
             raise InventoryError("No directory provided!")
 
         show_warning()
 
-        yield "@chroot/{0}".format(directory), {
-            "chroot_directory": "/{0}".format(directory.lstrip("/")),
+        yield "@chroot/{0}".format(name), {
+            "chroot_directory": "/{0}".format(name.lstrip("/")),
         }, ["@chroot"]
 
-    def connect(self):
+    def connect(self) -> None:
         self.local.connect()
 
         chroot_directory = self.host.data.chroot_directory
 
         try:
             with progress_spinner({"chroot run"}):
                 local.shell(
                     "chroot {0} ls".format(chroot_directory),
                     splitlines=True,
                 )
         except PyinfraError as e:
             raise ConnectError(e.args[0])
 
         self.host.connector_data["chroot_directory"] = chroot_directory
-        return True
 
     def run_shell_command(
         self,
         command,
         print_output: bool = False,
         print_input: bool = False,
         **command_arguments: Unpack["ConnectorArguments"],
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/docker.py` & `pyinfra-3.0b1/pyinfra/connectors/docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 
 if TYPE_CHECKING:
     from pyinfra.api.arguments import ConnectorArguments
     from pyinfra.api.host import Host
     from pyinfra.api.state import State
 
 
-class ConnectorData(TypedDict, total=False):
+class ConnectorData(TypedDict):
     docker_identifier: str
 
 
 connector_data_meta: dict[str, DataMeta] = {
     "docker_identifier": DataMeta("ID of container or image to start from"),
 }
 
 
 def _find_start_docker_container(container_id) -> tuple[str, bool]:
     docker_info = local.shell("docker container inspect {0}".format(container_id))
+    assert isinstance(docker_info, str)
     docker_info = json.loads(docker_info)[0]
     if docker_info["State"]["Running"] is False:
         logger.info("Starting stopped container: {0}".format(container_id))
         local.shell("docker container start {0}".format(container_id))
         return container_id, False
     return container_id, True
 
@@ -56,16 +57,18 @@
 
 
 class DockerConnector(BaseConnector):
     """
     The docker connector allows you to build Docker images or modify running
     Docker containers. You can pass either an image name or existing container ID:
 
-    + Image - will create a new container from the image, execute operations against it, save into a new Docker image and remove the container
-    + Existing container ID - will execute operations against the running container, leaving it running
+    + Image - will create a new container from the image, execute operations \
+        against it, save into a new Docker image and remove the container
+    + Existing container ID - will execute operations against the running \
+        container, leaving it running
 
     .. code:: shell
 
         # A Docker base image must be provided
         pyinfra @docker/alpine:3.8 ...
 
         # pyinfra can run on multiple Docker images in parallel
@@ -87,38 +90,36 @@
     no_stop: bool = False
 
     def __init__(self, state: "State", host: "Host"):
         super().__init__(state, host)
         self.local = LocalConnector(state, host)
 
     @staticmethod
-    def make_names_data(identifier=None):
-        if not identifier:
+    def make_names_data(name=None):
+        if not name:
             raise InventoryError("No docker base ID provided!")
 
         yield (
-            "@docker/{0}".format(identifier),
-            {"docker_identifier": identifier},
+            "@docker/{0}".format(name),
+            {"docker_identifier": name},
             ["@docker"],
         )
 
-    def connect(self):
+    def connect(self) -> None:
         self.local.connect()
 
         docker_identifier = self.data["docker_identifier"]
         with progress_spinner({"prepare docker container"}):
             try:
                 self.container_id, was_running = _find_start_docker_container(docker_identifier)
                 if was_running:
                     self.no_stop = True
             except PyinfraError:
                 self.container_id = _start_docker_image(docker_identifier)
 
-        return True
-
     def disconnect(self):
         container_id = self.container_id
 
         if self.no_stop:
             logger.info(
                 "{0}docker build complete, container left running: {1}".format(
                     self.host.print_prefix,
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/dockerssh.py` & `pyinfra-3.0b1/pyinfra/connectors/dockerssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
     logger.warning("The @dockerssh connector is in beta!")
 
 
 class DockerSSHConnector(BaseConnector):
     """
     **Note**: this connector is in beta!
 
-    The ``@dockerssh`` connector allows you to run commands on Docker containers on a remote machine.
+    The ``@dockerssh`` connector allows you to run commands on Docker containers \
+    on a remote machine.
 
     .. code:: shell
 
         # A Docker base image must be provided
         pyinfra @dockerssh/remotehost:alpine:3.8 ...
 
         # pyinfra can run on multiple Docker images in parallel
@@ -46,18 +47,18 @@
     ssh: SSHConnector
 
     def __init__(self, state: "State", host: "Host"):
         super().__init__(state, host)
         self.ssh = SSHConnector(state, host)
 
     @staticmethod
-    def make_names_data(host_image_str):
+    def make_names_data(name):
         try:
-            hostname, image = host_image_str.split(":", 1)
-        except (AttributeError, ValueError):  # failure to parse the host_image_str
+            hostname, image = name.split(":", 1)
+        except (AttributeError, ValueError):  # failure to parse the name
             raise InventoryError("No ssh host or docker base image provided!")
 
         if not image:
             raise InventoryError("No docker base image provided!")
 
         show_warning()
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/local.py` & `pyinfra-3.0b1/pyinfra/connectors/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 
 if TYPE_CHECKING:
     from pyinfra.api.arguments import ConnectorArguments
 
 
 class LocalConnector(BaseConnector):
     """
-    The ``@local`` connector executes changes on the local machine using subprocesses. **This connector is only compatible with MacOS & Linux hosts**.
+    The ``@local`` connector executes changes on the local machine using
+    subprocesses. **This connector is only compatible with MacOS & Linux hosts**.
 
     Examples:
 
     .. code::
 
         # Install nginx
         pyinfra inventory.py apt.packages nginx update=true _sudo=true
     """
 
     handles_execution = True
 
     @staticmethod
-    def make_names_data(_=None):
-        if _ is not None:
+    def make_names_data(name=None):
+        if name is not None:
             raise InventoryError("Cannot have more than one @local")
 
         yield "@local", {}, ["@local"]
 
     def run_shell_command(
         self,
         command: StringCommand,
@@ -201,16 +202,15 @@
             click.echo(
                 "{0}file copied: {1}".format(self.host.print_prefix, remote_filename),
                 err=True,
             )
 
         return True
 
-    @staticmethod
-    def check_can_rsync(host):
+    def check_can_rsync(self):
         if not find_executable("rsync"):
             raise NotImplementedError("The `rsync` binary is not available on this system.")
 
     def rsync(
         self,
         src,
         dest,
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/ssh.py` & `pyinfra-3.0b1/pyinfra/connectors/ssh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
 
 import shlex
 from distutils.spawn import find_executable
+from random import uniform
 from socket import error as socket_error, gaierror
+from time import sleep
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Tuple
 
 import click
 from paramiko import AuthenticationException, BadHostKeyException, SFTPClient, SSHException
 from typing_extensions import TypedDict, Unpack
 
 from pyinfra import logger
@@ -44,14 +46,18 @@
 
     ssh_config_file: str
     ssh_known_hosts_file: str
     ssh_strict_host_key_checking: str
 
     ssh_paramiko_connect_kwargs: dict
 
+    ssh_connect_retries: int
+    ssh_connect_retry_min_delay: float
+    ssh_connect_retry_max_delay: float
+
 
 connector_data_meta: dict[str, DataMeta] = {
     "ssh_hostname": DataMeta("SSH hostname"),
     "ssh_port": DataMeta("SSH port"),
     "ssh_user": DataMeta("SSH user"),
     "ssh_password": DataMeta("SSH password"),
     "ssh_key": DataMeta("SSH key filename"),
@@ -73,14 +79,23 @@
     "ssh_strict_host_key_checking": DataMeta(
         "SSH strict host key checking",
         "accept-new",
     ),
     "ssh_paramiko_connect_kwargs": DataMeta(
         "Override keyword arguments passed into Paramiko's ``SSHClient.connect``"
     ),
+    "ssh_connect_retries": DataMeta("Number of tries to connect via ssh", 0),
+    "ssh_connect_retry_min_delay": DataMeta(
+        "Lower bound for random delay between retries",
+        0.1,
+    ),
+    "ssh_connect_retry_max_delay": DataMeta(
+        "Upper bound for random delay between retries",
+        0.5,
+    ),
 }
 
 
 class SSHConnector(BaseConnector):
     """
     Connect to hosts over SSH. This is the default connector and all targets default
     to this meaning you do not need to specify it - ie the following two commands
@@ -121,16 +136,17 @@
 
     data_cls = ConnectorData
     data_meta = connector_data_meta
     data: ConnectorData
 
     client: Optional[SSHClient] = None
 
-    def make_names_data(hostname):
-        yield "@ssh/{0}".format(hostname), {"ssh_hostname": hostname}, []
+    @staticmethod
+    def make_names_data(name):
+        yield "@ssh/{0}".format(name), {"ssh_hostname": name}, []
 
     def make_paramiko_kwargs(self) -> dict[str, Any]:
         kwargs = {
             "allow_agent": False,
             "look_for_keys": False,
             "hostname": self.data["ssh_hostname"] or self.host.name,
             # Overrides of SSH config via pyinfra host data
@@ -168,14 +184,37 @@
         else:
             kwargs["allow_agent"] = self.data["ssh_allow_agent"]
             kwargs["look_for_keys"] = self.data["ssh_look_for_keys"]
 
         return kwargs
 
     def connect(self) -> None:
+        retries = self.data["ssh_connect_retries"]
+
+        try:
+            while True:
+                try:
+                    return self._connect()
+                except (SSHException, gaierror, socket_error, EOFError):
+                    if retries == 0:
+                        raise
+                    retries -= 1
+                    min_delay = self.data["ssh_connect_retry_min_delay"]
+                    max_delay = self.data["ssh_connect_retry_max_delay"]
+                    sleep(uniform(min_delay, max_delay))
+        except SSHException as e:
+            raise_connect_error(self.host, "SSH error", e)
+        except gaierror as e:
+            raise_connect_error(self.host, "Could not resolve hostname", e)
+        except socket_error as e:
+            raise_connect_error(self.host, "Could not connect", e)
+        except EOFError as e:
+            raise_connect_error(self.host, "EOF error", e)
+
+    def _connect(self) -> None:
         """
         Connect to a single host. Returns the SSH client if successful. Stateless by
         design so can be run in parallel.
         """
 
         kwargs = self.make_paramiko_kwargs()
         hostname = kwargs.pop("hostname")
@@ -217,26 +256,14 @@
 
             raise_connect_error(
                 self.host,
                 "SSH host key error",
                 f"Host key for {e.hostname} does not match.",
             )
 
-        except SSHException as e:
-            raise_connect_error(self.host, "SSH error", e)
-
-        except gaierror:
-            raise_connect_error(self.host, "Could not resolve hostname", hostname)
-
-        except socket_error as e:
-            raise_connect_error(self.host, "Could not connect", e)
-
-        except EOFError as e:
-            raise_connect_error(self.host, "EOF error", e)
-
     def run_shell_command(
         self,
         command: StringCommand,
         print_output: bool = False,
         print_input: bool = False,
         **arguments: Unpack["ConnectorArguments"],
     ) -> Tuple[bool, CommandOutput]:
@@ -446,24 +473,18 @@
         # user connected, so upload to tmp and copy/chown w/sudo and/or su_user
         if _sudo or _doas or _su_user:
             # Get temp file location
             temp_file = remote_temp_filename or self.host.get_temp_filename(remote_filename)
             self._put_file(filename_or_io, temp_file)
 
             # Make sure our sudo/su user can access the file
-            if _su_user:
-                command = StringCommand("setfacl", "-m", "u:{0}:r".format(_su_user), temp_file)
-            elif _sudo_user:
-                command = StringCommand("setfacl", "-m", "u:{0}:r".format(_sudo_user), temp_file)
-            elif _doas_user:
-                command = StringCommand("setfacl", "-m", "u:{0}:r".format(_doas_user), temp_file)
-
-            if _su_user or _sudo_user or _doas_user:
+            other_user = _su_user or _sudo_user or _doas_user
+            if other_user:
                 status, output = self.run_shell_command(
-                    command,
+                    StringCommand("setfacl", "-m", f"u:{other_user}:r", temp_file),
                     print_output=print_output,
                     print_input=print_input,
                     **arguments,
                 )
 
                 if status is False:
                     logger.error("Error on handover to sudo/su user: {0}".format(output.stderr))
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/ssh_util.py` & `pyinfra-3.0b1/pyinfra/connectors/ssh_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/connectors/sshuserclient/client.py` & `pyinfra-3.0b1/pyinfra/connectors/sshuserclient/client.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/connectors/sshuserclient/config.py` & `pyinfra-3.0b1/pyinfra/connectors/sshuserclient/config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/connectors/terraform.py` & `pyinfra-3.0b1/pyinfra/connectors/terraform.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 def _flatten_dict(d: dict, parent_key: str = "", sep: str = "."):
     return dict(_flatten_dict_gen(d, parent_key, sep))
 
 
 class TerraformInventoryConnector(BaseConnector):
     """
-    Generate one or more SSH hosts from a Terraform output variable. The variable must be a list of hostnames or dictionaries.
+    Generate one or more SSH hosts from a Terraform output variable. The variable
+    must be a list of hostnames or dictionaries.
 
     Output is fetched from a flattened JSON dictionary output from ``terraform output
     -json``. For example the following object:
 
     .. code:: json
 
         {
@@ -73,29 +74,31 @@
             }
           }
         }
 
     """
 
     @staticmethod
-    def make_names_data(output_key=None):
+    def make_names_data(name=None):
         show_warning()
 
-        if not output_key:
-            raise InventoryError("No Terraform output key!")
+        if not name:
+            name = ""
 
         with progress_spinner({"fetch terraform output"}):
             tf_output_raw = local.shell("terraform output -json")
 
+        assert isinstance(tf_output_raw, str)
         tf_output = json.loads(tf_output_raw)
         tf_output = _flatten_dict(tf_output)
 
-        tf_output_value = tf_output.get(output_key)
+        tf_output_value = tf_output.get(name)
         if tf_output_value is None:
-            raise InventoryError(f"No Terraform output with key: `{output_key}`")
+            keys = "\n".join(f"   - {k}" for k in tf_output.keys())
+            raise InventoryError(f"No Terraform output with key: `{name}`, valid keys:\n{keys}")
 
         if not isinstance(tf_output_value, list):
             raise InventoryError(
                 "Invalid Terraform output type, should be `list`, got "
                 f"`{type(tf_output_value).__name__}`",
             )
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/util.py` & `pyinfra-3.0b1/pyinfra/connectors/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 def run_local_process(
     command: str,
     stdin=None,
     timeout: Optional[int] = None,
     print_output: bool = False,
-    print_prefix=None,
+    print_prefix: str = "",
 ) -> tuple[int, "CommandOutput"]:
     process = Popen(command, shell=True, stdout=PIPE, stderr=PIPE, stdin=PIPE)
 
     if stdin:
         write_stdin(stdin, process.stdin)
 
     assert process.stdout is not None
```

### Comparing `pyinfra-3.0b0/pyinfra/connectors/vagrant.py` & `pyinfra-3.0b1/pyinfra/connectors/vagrant.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,16 +128,16 @@
         pyinfra @vagrant/my-vm-name ...
 
         # Run on multiple named VMs
         pyinfra @vagrant/my-vm-name,@vagrant/another-vm-name ...
     """
 
     @staticmethod
-    def make_names_data(limit=None):
-        vagrant_ssh_info = get_vagrant_config(limit)
+    def make_names_data(name=None):
+        vagrant_ssh_info = get_vagrant_config(name)
 
         logger.debug("Got Vagrant SSH info: \n%s", vagrant_ssh_info)
 
         hosts = []
         current_host = None
 
         for line in vagrant_ssh_info:
@@ -166,14 +166,15 @@
             else:
                 logger.debug("Extra Vagrant SSH key/value (%s=%s)", key, value)
 
         if current_host:
             hosts.append(_make_name_data(current_host))
 
         if not hosts:
-            if limit:
+            if name:
                 raise InventoryError(
-                    "No running Vagrant instances matching `{0}` found!".format(limit)
+                    "No running Vagrant instances matching `{0}` found!".format(name)
                 )
             raise InventoryError("No running Vagrant instances found!")
 
-        return hosts
+        for host in hosts:
+            yield host
```

### Comparing `pyinfra-3.0b0/pyinfra/context.py` & `pyinfra-3.0b1/pyinfra/context.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/apt.py` & `pyinfra-3.0b1/pyinfra/facts/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/brew.py` & `pyinfra-3.0b1/pyinfra/facts/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/cargo.py` & `pyinfra-3.0b1/pyinfra/facts/cargo.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/choco.py` & `pyinfra-3.0b1/pyinfra/facts/choco.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     .. code:: python
 
         {
             "package_name": ["version"],
         }
     """
 
-    command = "choco list --local-only"
+    command = "choco list"
     shell_executable = "ps"
 
     default = dict
 
     def process(self, output):
         return parse_packages(CHOCO_REGEX, output)
```

### Comparing `pyinfra-3.0b0/pyinfra/facts/deb.py` & `pyinfra-3.0b1/pyinfra/facts/deb.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
 class DebPackage(FactBase):
     """
     Returns information on a .deb archive or installed package.
     """
 
     _regexes = {
-        "name": r"^Package: ({0})$".format(DEB_PACKAGE_NAME_REGEX),
-        "version": r"^Version: ({0})$".format(DEB_PACKAGE_VERSION_REGEX),
+        "name": r"^Package:\s+({0})$".format(DEB_PACKAGE_NAME_REGEX),
+        "version": r"^Version:\s+({0})$".format(DEB_PACKAGE_VERSION_REGEX),
     }
 
     requires_command = "dpkg"
 
     def command(self, name):
         return "! test -e {0} && (dpkg -s {0} 2>/dev/null || true) || dpkg -I {0}".format(name)
```

### Comparing `pyinfra-3.0b0/pyinfra/facts/dnf.py` & `pyinfra-3.0b1/pyinfra/facts/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/docker.py` & `pyinfra-3.0b1/pyinfra/facts/docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/files.py` & `pyinfra-3.0b1/pyinfra/facts/files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/git.py` & `pyinfra-3.0b1/pyinfra/facts/git.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/gpg.py` & `pyinfra-3.0b1/pyinfra/facts/gpg.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/hardware.py` & `pyinfra-3.0b1/pyinfra/facts/hardware.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/iptables.py` & `pyinfra-3.0b1/pyinfra/facts/iptables.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/launchd.py` & `pyinfra-3.0b1/pyinfra/facts/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/mysql.py` & `pyinfra-3.0b1/pyinfra/facts/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/npm.py` & `pyinfra-3.0b1/pyinfra/facts/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/openrc.py` & `pyinfra-3.0b1/pyinfra/facts/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/pacman.py` & `pyinfra-3.0b1/pyinfra/facts/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/pip.py` & `pyinfra-3.0b1/pyinfra/facts/pip.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/postgresql.py` & `pyinfra-3.0b1/pyinfra/facts/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return StringCommand(
         make_psql_command(**psql_kwargs),
         "-Ac",
         QuoteString(command),  # quote this whole item as a single shell argument
     )
 
 
-class PostgresqlFactBase(FactBase):
+class PostgresFactBase(FactBase):
     abstract = True
 
     psql_command: str
     requires_command = "psql"
 
     def command(
         self,
@@ -62,15 +62,15 @@
             user=psql_user,
             password=psql_password,
             host=psql_host,
             port=psql_port,
         )
 
 
-class PostgresqlRoles(PostgresqlFactBase):
+class PostgresRoles(PostgresFactBase):
     """
     Returns a dict of PostgreSQL roles and data:
 
     .. code:: python
 
         {
             "pyinfra": {
@@ -114,15 +114,15 @@
                     details[key] = value == "t"
 
             users[details.pop("name")] = details
 
         return users
 
 
-class PostgresqlDatabases(PostgresqlFactBase):
+class PostgresDatabases(PostgresFactBase):
     """
     Returns a dict of PostgreSQL databases and metadata:
 
     .. code:: python
 
         {
             "pyinfra_stuff": {
```

### Comparing `pyinfra-3.0b0/pyinfra/facts/rpm.py` & `pyinfra-3.0b1/pyinfra/facts/rpm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/selinux.py` & `pyinfra-3.0b1/pyinfra/facts/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/server.py` & `pyinfra-3.0b1/pyinfra/facts/server.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/snap.py` & `pyinfra-3.0b1/pyinfra/facts/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/systemd.py` & `pyinfra-3.0b1/pyinfra/facts/systemd.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
-from typing import Dict
+from typing import Dict, Iterable
 
-from pyinfra.api import FactBase
+from pyinfra.api import FactBase, FactTypeError, QuoteString, StringCommand
 
 # Valid unit names consist of a "name prefix" and a dot and a suffix specifying the unit type.
 # The "unit prefix" must consist of one or more valid characters
 # (ASCII letters, digits, ":", "-", "_", ".", and "\").
 # The total length of the unit name including the suffix must not exceed 256 characters.
 # The type suffix must be one of
 # ".service", ".socket", ".device", ".mount", ".automount",
@@ -18,26 +18,24 @@
     r"[a-zA-Z0-9\:\-\_\.\\\@]+\."
     r"(?:service|socket|device|mount|automount|swap|target|path|timer|slice|scope)"
 )
 
 
 def _make_systemctl_cmd(user_mode=False, machine=None, user_name=None):
     # base command for normal and user mode
-    systemctl_cmd = "systemctl --user" if user_mode else "systemctl"
+    systemctl_cmd = ["systemctl --user"] if user_mode else ["systemctl"]
 
     # add user and machine flag if given in args
     if machine is not None:
         if user_name is not None:
-            machine_opt = "--machine={1}@{0}".format(machine, user_name)
+            systemctl_cmd.append("--machine={1}@{0}".format(machine, user_name))
         else:
-            machine_opt = "--machine={0}".format(machine)
+            systemctl_cmd.append("--machine={0}".format(machine))
 
-        systemctl_cmd = "{0} {1}".format(systemctl_cmd, machine_opt)
-
-    return systemctl_cmd
+    return StringCommand(*systemctl_cmd)
 
 
 class SystemdStatus(FactBase[Dict[str, bool]]):
     """
     Returns a dictionary map of systemd units to booleans indicating whether they are active.
 
     + user_mode: whether to use user mode
@@ -55,22 +53,40 @@
     requires_command = "systemctl"
 
     default = dict
 
     state_key = "SubState"
     state_values = ["running", "waiting", "exited"]
 
-    def command(self, user_mode=False, machine=None, user_name=None):
+    def command(self, user_mode=False, machine=None, user_name=None, services=None):
         fact_cmd = _make_systemctl_cmd(
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
         )
 
-        return f"{fact_cmd} show --all --property Id --property {self.state_key} '*'"
+        if services is None:
+            service_strs = [QuoteString("*")]
+        elif isinstance(services, str):
+            service_strs = [QuoteString(services)]
+        elif isinstance(services, Iterable):
+            service_strs = [QuoteString(s) for s in services]
+        else:
+            raise FactTypeError(f"Invalid type passed for services argument: {type(services)}")
+
+        return StringCommand(
+            fact_cmd,
+            "show",
+            "--all",
+            "--property",
+            "Id",
+            "--property",
+            self.state_key,
+            *service_strs,
+        )
 
     def process(self, output) -> Dict[str, bool]:
         services: Dict[str, bool] = {}
 
         current_unit = None
         for line in output:
             line = line.strip()
```

### Comparing `pyinfra-3.0b0/pyinfra/facts/sysvinit.py` & `pyinfra-3.0b1/pyinfra/facts/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/upstart.py` & `pyinfra-3.0b1/pyinfra/facts/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/util/__init__.py` & `pyinfra-3.0b1/pyinfra/facts/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/util/databases.py` & `pyinfra-3.0b1/pyinfra/facts/util/databases.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/util/packaging.py` & `pyinfra-3.0b1/pyinfra/facts/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/util/win_files.py` & `pyinfra-3.0b1/pyinfra/facts/util/win_files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/vzctl.py` & `pyinfra-3.0b1/pyinfra/facts/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/yum.py` & `pyinfra-3.0b1/pyinfra/facts/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/facts/zypper.py` & `pyinfra-3.0b1/pyinfra/facts/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/local.py` & `pyinfra-3.0b1/pyinfra/local.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/apk.py` & `pyinfra-3.0b1/pyinfra/operations/apk.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/apt.py` & `pyinfra-3.0b1/pyinfra/operations/apt.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/brew.py` & `pyinfra-3.0b1/pyinfra/operations/brew.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/bsdinit.py` & `pyinfra-3.0b1/pyinfra/operations/bsdinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/cargo.py` & `pyinfra-3.0b1/pyinfra/operations/cargo.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/choco.py` & `pyinfra-3.0b1/pyinfra/operations/choco.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/dnf.py` & `pyinfra-3.0b1/pyinfra/operations/dnf.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/files.py` & `pyinfra-3.0b1/pyinfra/operations/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import os
 import posixpath
 import sys
 import traceback
 from datetime import timedelta
 from fnmatch import fnmatch
 from io import StringIO
+from pathlib import Path
 from typing import Union
 
 from jinja2 import TemplateRuntimeError, TemplateSyntaxError, UndefinedError
 
 from pyinfra import host, logger, state
 from pyinfra.api import (
     FileDownloadCommand,
@@ -26,14 +27,15 @@
     RsyncCommand,
     StringCommand,
     operation,
 )
 from pyinfra.api.command import make_formatted_string_command
 from pyinfra.api.util import (
     get_call_location,
+    get_file_io,
     get_file_sha1,
     get_path_permissions_mode,
     get_template,
     memoize,
 )
 from pyinfra.facts.files import (
     MARKER_BEGIN_DEFAULT,
@@ -565,15 +567,15 @@
     if exclude_dir is not None:
         if not isinstance(exclude_dir, (list, tuple)):
             exclude_dir = [exclude_dir]
 
     put_files = []
     ensure_dirnames = []
     for dirpath, dirnames, filenames in os.walk(src, topdown=True):
-        remote_dirpath = os.path.normpath(os.path.relpath(dirpath, src))
+        remote_dirpath = Path(os.path.normpath(os.path.relpath(dirpath, src))).as_posix()
 
         # Filter excluded dirs
         for child_dir in dirnames[:]:
             child_path = os.path.normpath(os.path.join(remote_dirpath, child_dir))
             if exclude_dir and any(fnmatch(child_path, match) for match in exclude_dir):
                 dirnames.remove(child_dir)
 
@@ -995,28 +997,28 @@
             for frame in traceback.extract_tb(sys.exc_info()[2])
             if frame[2] in ("template", "<module>", "top-level template code")
         ]  # thank you https://github.com/saltstack/salt/blob/master/salt/utils/templates.py
 
         line_number = trace_frames[-1][1]
 
         # Quickly read the line in question and one above/below for nicer debugging
-        with open(src, "r") as f:
+        with get_file_io(src, "r") as f:
             template_lines = f.readlines()
 
         template_lines = [line.strip() for line in template_lines]
         relevant_lines = template_lines[max(line_number - 2, 0) : line_number + 1]
 
         raise OperationError(
             "Error in template: {0} (L{1}): {2}\n...\n{3}\n...".format(
                 src,
                 line_number,
                 e,
                 "\n".join(relevant_lines),
             ),
-        )
+        ) from None
 
     output_file = StringIO(output)
     # Set the template attribute for nicer debugging
     output_file.template = src  # type: ignore[attr-defined]
 
     # Pass to the put function
     yield from put._inner(
```

### Comparing `pyinfra-3.0b0/pyinfra/operations/gem.py` & `pyinfra-3.0b1/pyinfra/operations/gem.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/git.py` & `pyinfra-3.0b1/pyinfra/operations/git.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/iptables.py` & `pyinfra-3.0b1/pyinfra/operations/iptables.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,26 +259,32 @@
 
         if protocol:
             args.extend(("-p", protocol))
 
         if source:
             args.extend(("-s", source))
 
+        if destination:
+            args.extend(("-d", destination))
+
         if in_interface:
             args.extend(("-i", in_interface))
 
         if out_interface:
             args.extend(("-o", out_interface))
 
         if not_protocol:
             args.extend(("!", "-p", not_protocol.lower()))
 
         if not_source:
             args.extend(("!", "-s", not_source))
 
+        if not_destination:
+            args.extend(("!", "-d", not_destination))
+
         if not_in_interface:
             args.extend(("!", "-i", not_in_interface))
 
         if not_out_interface:
             args.extend(("!", "-o", not_out_interface))
 
         if extras:
```

### Comparing `pyinfra-3.0b0/pyinfra/operations/launchd.py` & `pyinfra-3.0b1/pyinfra/operations/launchd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/lxd.py` & `pyinfra-3.0b1/pyinfra/operations/lxd.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/mysql.py` & `pyinfra-3.0b1/pyinfra/operations/mysql.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/npm.py` & `pyinfra-3.0b1/pyinfra/operations/npm.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/openrc.py` & `pyinfra-3.0b1/pyinfra/operations/openrc.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/pacman.py` & `pyinfra-3.0b1/pyinfra/operations/pacman.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/pip.py` & `pyinfra-3.0b1/pyinfra/operations/pip.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,14 +181,19 @@
         else:
             yield "{0} -r {1}".format(uninstall_command, requirements)
 
     # Handle passed in packages
     if packages:
         current_packages = host.get_fact(PipPackages, pip=pip)
 
+        # PEP-0426 states that Python packages should be compared using lowercase, so lowercase both
+        # the input packages and the fact packages before comparison.
+        packages = [pkg.lower() for pkg in packages]
+        current_packages = {pkg.lower(): versions for pkg, versions in current_packages.items()}
+
         yield from ensure_packages(
             host,
             packages,
             current_packages,
             present,
             install_command=install_command,
             uninstall_command=uninstall_command,
```

### Comparing `pyinfra-3.0b0/pyinfra/operations/pkg.py` & `pyinfra-3.0b1/pyinfra/operations/pkg.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/pkgin.py` & `pyinfra-3.0b1/pyinfra/operations/pkgin.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/postgresql.py` & `pyinfra-3.0b1/pyinfra/operations/postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 See example/postgresql.py for detailed example
 
 """
 
 from pyinfra import host
 from pyinfra.api import MaskString, StringCommand, operation
-from pyinfra.facts.postgresql import (
-    PostgresqlDatabases,
-    PostgresqlRoles,
+from pyinfra.facts.postgres import (
+    PostgresDatabases,
+    PostgresRoles,
     make_execute_psql_command,
     make_psql_command,
 )
 
 
 @operation(is_idempotent=False)
 def sql(
@@ -101,15 +101,15 @@
             login=True,
             sudo_user="postgres",
         )
 
     """
 
     roles = host.get_fact(
-        PostgresqlRoles,
+        PostgresRoles,
         psql_user=psql_user,
         psql_password=psql_password,
         psql_host=psql_host,
         psql_port=psql_port,
     )
 
     is_present = role in roles
@@ -207,15 +207,15 @@
             encoding="UTF8",
             sudo_user="postgres",
         )
 
     """
 
     current_databases = host.get_fact(
-        PostgresqlDatabases,
+        PostgresDatabases,
         psql_user=psql_user,
         psql_password=psql_password,
         psql_host=psql_host,
         psql_port=psql_port,
     )
 
     is_present = database in current_databases
```

### Comparing `pyinfra-3.0b0/pyinfra/operations/puppet.py` & `pyinfra-3.0b1/pyinfra/operations/puppet.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/python.py` & `pyinfra-3.0b1/pyinfra/operations/python.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/selinux.py` & `pyinfra-3.0b1/pyinfra/operations/selinux.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/server.py` & `pyinfra-3.0b1/pyinfra/operations/server.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/snap.py` & `pyinfra-3.0b1/pyinfra/operations/snap.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/ssh.py` & `pyinfra-3.0b1/pyinfra/operations/ssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/systemd.py` & `pyinfra-3.0b1/pyinfra/operations/systemd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Manage systemd services.
 """
 
 from pyinfra import host
-from pyinfra.api import operation
+from pyinfra.api import StringCommand, operation
 from pyinfra.facts.systemd import SystemdEnabled, SystemdStatus, _make_systemctl_cmd
 
 from .util.service import handle_service_control
 
 
 @operation(is_idempotent=False)
 def daemon_reload(user_mode=False, machine=None, user_name=None):
@@ -21,15 +21,15 @@
 
     systemctl_cmd = _make_systemctl_cmd(
         user_mode=user_mode,
         machine=machine,
         user_name=user_name,
     )
 
-    yield "{0} daemon-reload".format(systemctl_cmd)
+    yield StringCommand(systemctl_cmd, "daemon-reload")
 
 
 _daemon_reload = daemon_reload._inner  # noqa: E305
 
 
 @operation()
 def service(
@@ -113,28 +113,30 @@
         host,
         service,
         host.get_fact(
             SystemdStatus,
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
+            services=[service],
         ),
-        " ".join([systemctl_cmd, "{1}", "{0}"]),
+        " ".join([systemctl_cmd.get_raw_value(), "{1}", "{0}"]),
         running,
         restarted,
         reloaded,
         command,
     )
 
     if isinstance(enabled, bool):
         systemd_enabled = host.get_fact(
             SystemdEnabled,
             user_mode=user_mode,
             machine=machine,
             user_name=user_name,
+            services=[service],
         )
         is_enabled = systemd_enabled.get(service, False)
 
         # Isn't enabled and want enabled?
         if not is_enabled and enabled is True:
             yield "{0} enable {1}".format(systemctl_cmd, service)
```

### Comparing `pyinfra-3.0b0/pyinfra/operations/sysvinit.py` & `pyinfra-3.0b1/pyinfra/operations/sysvinit.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/upstart.py` & `pyinfra-3.0b1/pyinfra/operations/upstart.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/util/files.py` & `pyinfra-3.0b1/pyinfra/operations/util/files.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/util/packaging.py` & `pyinfra-3.0b1/pyinfra/operations/util/packaging.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/util/service.py` & `pyinfra-3.0b1/pyinfra/operations/util/service.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/vzctl.py` & `pyinfra-3.0b1/pyinfra/operations/vzctl.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/xbps.py` & `pyinfra-3.0b1/pyinfra/operations/xbps.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/yum.py` & `pyinfra-3.0b1/pyinfra/operations/yum.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/operations/zypper.py` & `pyinfra-3.0b1/pyinfra/operations/zypper.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra/progress.py` & `pyinfra-3.0b1/pyinfra/progress.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra.egg-info/PKG-INFO` & `pyinfra-3.0b1/pyinfra.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinfra
-Version: 3.0b0
+Version: 3.0b1
 Summary: pyinfra automates/provisions/manages/deploys infrastructure.
 Home-page: https://pyinfra.com
 Author: Nick / Fizzadar
 Author-email: pointlessrambler@gmail.com
 License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com
 Project-URL: GitHub, https://github.com/Fizzadar/pyinfra
@@ -31,33 +31,33 @@
 
 <p align="center">
     <a href="https://pyinfra.com">
         <img src="https://pyinfra.com/static/logo_readme.png" alt="pyinfra" />
     </a>
 </p>
 
-<p align="center">
+<p>
     <strong>Note: this is the v3 branch, which is currently in beta. <a href="https://docs.pyinfra.com/en/next">See the docs for v3</a>. If needed the <a href="https://github.com/pyinfra-dev/pyinfra/tree/2.x/">2.x branch is here</a>, but is in bugfix only mode.</strong>
 </p>
 
-<p align="center">
-    <em>pyinfra automates infrastructure using Python. It’s fast and scales from one server to thousands. Great for ad-hoc command execution, service deployment, configuration management and more.</em>
+<p>
+    pyinfra turns Python code into shell commands and runs them on your servers. Execute ad-hoc commands and write declarative operations. Target SSH servers, local machine and Docker containers. Fast and scales from one server to thousands. Think <code>ansible</code> but Python instead of YAML, and a lot faster.
 </p>
 
 ---
 
-<p align="center">
+<p>
     <a href="https://docs.pyinfra.com"><strong>Documentation</strong></a> &rArr;
     <a href="https://docs.pyinfra.com/page/getting-started.html"><strong>Getting Started</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/examples.html"><strong>Examples</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/support.html"><strong>Help & Support</strong></a> &bull;
     <a href="https://docs.pyinfra.com/page/contributing.html"><strong>Contributing</strong></a>
 </p>
 
-<p align="center">
+<p>
     Chat &rArr;
     <a href="https://matrix.to/#/#pyinfra:matrix.org"><strong><code>#pyinfra</code> on Matrix</strong></a>
 </p>
 
 ---
 
 Why pyinfra? Design features include:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyinfra Version: 3.0b0 Summary: pyinfra automates/
+Metadata-Version: 2.1 Name: pyinfra Version: 3.0b1 Summary: pyinfra automates/
 provisions/manages/deploys infrastructure. Home-page: https://pyinfra.com
 Author: Nick / Fizzadar Author-email: pointlessrambler@gmail.com License: MIT
 Project-URL: Documentation, https://docs.pyinfra.com Project-URL: GitHub,
 https://github.com/Fizzadar/pyinfra Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology Classifier: License ::
@@ -11,22 +11,23 @@
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Topic :: System :: Systems
 Administration Classifier: Topic :: System :: Installation/Setup Classifier:
 Topic :: Utilities Description-Content-Type: text/markdown Provides-Extra: test
 Provides-Extra: docs Provides-Extra: dev License-File: LICENSE.md
                                    _[_p_y_i_n_f_r_a_]
- NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
-         IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
-ppyyiinnffrraa aauuttoommaatteess iinnffrraassttrruuccttuurree uussiinngg PPyytthhoonn.. IItt?â??ss ffaasstt aanndd ssccaalleess ffrroomm oonnee
- sseerrvveerr ttoo tthhoouussaannddss.. GGrreeaatt ffoorr aadd--hhoocc ccoommmmaanndd eexxeeccuuttiioonn,, sseerrvviiccee ddeeppllooyymmeenntt,,
-                      ccoonnffiigguurraattiioonn mmaannaaggeemmeenntt aanndd mmoorree..
+NNoottee:: tthhiiss iiss tthhee vv33 bbrraanncchh,, wwhhiicchh iiss ccuurrrreennttllyy iinn bbeettaa.. _SS_ee_ee_ _tt_hh_ee_ _dd_oo_cc_ss_ _ff_oo_rr_ _vv_33..
+IIff nneeeeddeedd tthhee _22_.._xx_ _bb_rr_aa_nn_cc_hh_ _ii_ss_ _hh_ee_rr_ee,, bbuutt iiss iinn bbuuggffiixx oonnllyy mmooddee..
+pyinfra turns Python code into shell commands and runs them on your servers.
+Execute ad-hoc commands and write declarative operations. Target SSH servers,
+local machine and Docker containers. Fast and scales from one server to
+thousands. Think ansible but Python instead of YAML, and a lot faster.
 ---
-  _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
-                           Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
+_DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ⇒ _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd • _EE_xx_aa_mm_pp_ll_ee_ss • _HH_ee_ll_pp_ _&&_ _SS_uu_pp_pp_oo_rr_tt • _CC_oo_nn_tt_rr_ii_bb_uu_tt_ii_nn_gg
+Chat ⇒ _##_pp_yy_ii_nn_ff_rr_aa_ _oo_nn_ _MM_aa_tt_rr_ii_xx
 --- Why pyinfra? Design features include: + ð **Super fast** execution over
 thousands of hosts with predictable performance. + ð¨ **Instant debugging**
 with realtime stdin/stdout/stderr output (`-vvv`). + ð **Idempotent
 operations** that enable diffs and dry runs before making changes. + ð¦
 **Extendable** with the entire Python package ecosystem. + ð» **Agentless
 execution** against anything with shell access. + ð **Integrated** with
 connectors for Docker, Terraform, Vagrant and more. [https://pyinfra.com/
```

### Comparing `pyinfra-3.0b0/pyinfra.egg-info/SOURCES.txt` & `pyinfra-3.0b1/pyinfra.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 pyinfra/facts/mysql.py
 pyinfra/facts/npm.py
 pyinfra/facts/openrc.py
 pyinfra/facts/pacman.py
 pyinfra/facts/pip.py
 pyinfra/facts/pkg.py
 pyinfra/facts/pkgin.py
+pyinfra/facts/postgres.py
 pyinfra/facts/postgresql.py
 pyinfra/facts/rpm.py
 pyinfra/facts/selinux.py
 pyinfra/facts/server.py
 pyinfra/facts/snap.py
 pyinfra/facts/systemd.py
 pyinfra/facts/sysvinit.py
@@ -106,14 +107,15 @@
 pyinfra/operations/mysql.py
 pyinfra/operations/npm.py
 pyinfra/operations/openrc.py
 pyinfra/operations/pacman.py
 pyinfra/operations/pip.py
 pyinfra/operations/pkg.py
 pyinfra/operations/pkgin.py
+pyinfra/operations/postgres.py
 pyinfra/operations/postgresql.py
 pyinfra/operations/puppet.py
 pyinfra/operations/python.py
 pyinfra/operations/selinux.py
 pyinfra/operations/server.py
 pyinfra/operations/snap.py
 pyinfra/operations/ssh.py
@@ -129,15 +131,14 @@
 pyinfra/operations/util/packaging.py
 pyinfra/operations/util/service.py
 pyinfra_cli/__init__.py
 pyinfra_cli/__main__.py
 pyinfra_cli/commands.py
 pyinfra_cli/exceptions.py
 pyinfra_cli/inventory.py
-pyinfra_cli/inventory_dsl.py
 pyinfra_cli/log.py
 pyinfra_cli/main.py
 pyinfra_cli/prints.py
 pyinfra_cli/util.py
 pyinfra_cli/virtualenv.py
 tests/__init__.py
 tests/paramiko_util.py
```

### Comparing `pyinfra-3.0b0/pyinfra.egg-info/requires.txt` & `pyinfra-3.0b1/pyinfra.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra_cli/__main__.py` & `pyinfra-3.0b1/pyinfra_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra_cli/commands.py` & `pyinfra-3.0b1/pyinfra_cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,34 +32,35 @@
         for key, value in [arg.split("=", 1) for arg in operation_args if "=" in arg]
     }
 
     return op, (args, kwargs)
 
 
 def get_facts_and_args(commands):
-    facts: list[FactBase] = []
+    facts: list[tuple[FactBase, tuple, dict]] = []
 
     current_fact = None
 
     for command in commands:
         if "=" in command:
             if not current_fact:
                 raise CliError("Invalid fact commands: `{0}`".format(commands))
 
             key, value = command.split("=", 1)
-            current_fact[2][key] = value
+            current_fact[2][key] = parse_cli_arg(value)
             continue
 
         if current_fact:
             facts.append(current_fact)
             current_fact = None
 
         if "." not in command:
             raise CliError(f"Invalid fact: `{command}`, should be in the format `module.cls`")
 
         fact_cls = try_import_module_attribute(command, prefix="pyinfra.facts")
+        assert fact_cls is not None
         current_fact = (fact_cls, (), {})
 
     if current_fact:
         facts.append(current_fact)
 
     return facts
```

### Comparing `pyinfra-3.0b0/pyinfra_cli/exceptions.py` & `pyinfra-3.0b1/pyinfra_cli/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import abc
 import sys
 from inspect import getframeinfo
+from os import path
 from traceback import format_exception, format_tb, walk_tb
 from types import TracebackType
 
 import click
 
 from pyinfra import logger
 from pyinfra.api.exceptions import (
@@ -19,14 +20,18 @@
 def get_frame_line_from_tb(tb: TracebackType):
     frame_lines = list(walk_tb(tb))
     frame_lines.reverse()
     for frame, line in frame_lines:
         info = getframeinfo(frame)
         if info.filename.startswith(PYINFRA_INSTALL_DIR):
             continue
+        if info.filename.startswith("/"):
+            continue
+        if not path.exists(info.filename):
+            continue
         return info
 
 
 class WrappedError(click.ClickException):
     def __init__(self, e: Exception):
         self.traceback = e.__traceback__
         self.exception = e
```

### Comparing `pyinfra-3.0b0/pyinfra_cli/inventory.py` & `pyinfra-3.0b1/pyinfra_cli/inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra_cli/log.py` & `pyinfra-3.0b1/pyinfra_cli/log.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra_cli/main.py` & `pyinfra-3.0b1/pyinfra_cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 )
 @click.option(
     "-y",
     "--yes",
     is_flag=True,
     default=False,
     help="Execute operations immediately on hosts without prompt or checking for changes.",
+    envvar="PYINFRA_YES",
+    show_envvar=True,
 )
 @click.option(
     "--limit",
     help="Restrict the target hosts by name and group name.",
     multiple=True,
 )
 @click.option("--fail-percent", type=int, help="% of hosts that need to fail before exiting early.")
```

### Comparing `pyinfra-3.0b0/pyinfra_cli/prints.py` & `pyinfra-3.0b1/pyinfra_cli/prints.py`

 * *Files 22% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         name = "{0} ({1})".format(name, ", ".join(str(arg) for arg in op_meta.args))
 
     return name
 
 
 def print_meta(state: "State"):
     rows: List[Tuple[Callable, Union[List[str], str]]] = [
-        (logger.info, ["Operation", "Hosts"]),
+        (logger.info, ["Operation", "Change", "Conditional Change"]),
     ]
 
     for op_hash in state.get_op_order():
         hosts_in_op = []
         hosts_maybe_in_op = []
         for host in state.inventory.iter_activated_hosts():
             if op_hash in state.ops[host]:
@@ -233,22 +233,26 @@
                         hosts_in_op.append(host.name)
 
         rows.append(
             (
                 logger.info,
                 [
                     pretty_op_name(state.op_meta[op_hash]),
-                    "{0}{1}/{2} ({3})".format(
+                    "-"
+                    if len(hosts_in_op) == 0
+                    else "{0} ({1})".format(
                         len(hosts_in_op),
-                        f"-{len(hosts_maybe_in_op)}" if hosts_maybe_in_op else "",
-                        len(state.inventory),
-                        truncate(", ".join(sorted(hosts_in_op + hosts_maybe_in_op)), 48),
-                    )
-                    if hosts_in_op or hosts_maybe_in_op
-                    else "No hosts with changes at this time",
+                        truncate(", ".join(sorted(hosts_in_op)), 48),
+                    ),
+                    "-"
+                    if len(hosts_maybe_in_op) == 0
+                    else "{0} ({1})".format(
+                        len(hosts_maybe_in_op),
+                        truncate(", ".join(sorted(hosts_maybe_in_op)), 48),
+                    ),
                 ],
             )
         )
 
     print_rows(rows)
 
 
@@ -257,130 +261,44 @@
         (logger.info, ["Operation", "Hosts", "Success", "Error", "No Change"]),
     ]
 
     for op_hash in state.get_op_order():
         hosts_in_op = 0
         hosts_in_op_success: list[str] = []
         hosts_in_op_error: list[str] = []
-        hosts_in_op_no_attempt: list[str] = []
+        hosts_in_op_no_change: list[str] = []
         for host in state.inventory.iter_activated_hosts():
             if op_hash not in state.ops[host]:
                 continue
 
             hosts_in_op += 1
 
-            result = state.ops[host][op_hash].operation_meta.did_succeed()
-            if result is True:
-                hosts_in_op_success.append(host.name)
-            elif result is False:
-                hosts_in_op_error.append(host.name)
+            op_meta = state.ops[host][op_hash].operation_meta
+            if op_meta.did_succeed():
+                if op_meta._did_change():
+                    hosts_in_op_success.append(host.name)
+                else:
+                    hosts_in_op_no_change.append(host.name)
             else:
-                hosts_in_op_no_attempt.append(host.name)
-
-        # if not hosts_in_op:
-        #     continue
+                hosts_in_op_error.append(host.name)
 
         row = [
             pretty_op_name(state.op_meta[op_hash]),
             str(hosts_in_op),
         ]
 
         if hosts_in_op_success:
             row.append(f"{len(hosts_in_op_success)}")
         else:
             row.append("-")
         if hosts_in_op_error:
             row.append(f"{len(hosts_in_op_error)}")
         else:
             row.append("-")
-        if hosts_in_op_no_attempt:
-            row.append(f"{len(hosts_in_op_no_attempt)}")
+        if hosts_in_op_no_change:
+            row.append(f"{len(hosts_in_op_no_change)}")
         else:
             row.append("-")
 
         rows.append((logger.info, row))
 
     print_rows(rows)
-
-
-def get_fucked(state: "State"):
-    group_combinations = _get_group_combinations(state.inventory.iter_activated_hosts())
-    rows: List[Tuple[Callable, Union[List[str], str]]] = []
-
-    for i, (groups, hosts) in enumerate(group_combinations.items(), 1):
-        if not hosts:
-            continue
-
-        if groups:
-            rows.append(
-                (
-                    logger.info,
-                    "Groups: {0}".format(
-                        click.style(" / ".join(groups), bold=True),
-                    ),
-                ),
-            )
-        else:
-            rows.append((logger.info, "Ungrouped:"))
-
-        for host in hosts:
-            # Didn't connect to this host?
-            if host not in state.activated_hosts:
-                rows.append(
-                    (
-                        logger.info,
-                        [
-                            host.style_print_prefix("red", bold=True),
-                            click.style("No connection", "red"),
-                        ],
-                    ),
-                )
-                continue
-
-            results = state.results[host]
-
-            meta = state.meta[host]
-            success_ops = results.success_ops
-            partial_ops = results.partial_ops
-            # TODO: type meta object
-            changed_ops = success_ops - meta.ops_no_change  # type: ignore
-            error_ops = results.error_ops
-            ignored_error_ops = results.ignored_error_ops
-
-            host_args = ("green",)
-            host_kwargs = {}
-
-            # If all ops got complete
-            if results.ops == meta.ops:
-                # We had some errors - but we ignored them - so "warning" color
-                if error_ops != 0:
-                    host_args = ("yellow",)
-
-            # Ops did not complete!
-            else:
-                host_args = ("red",)
-                host_kwargs["bold"] = True
-
-            changed_str = "Changed: {0}".format(click.style(f"{changed_ops}", bold=True))
-            if partial_ops:
-                changed_str = f"{changed_str} ({partial_ops} partial)"
-
-            error_str = "Errors: {0}".format(click.style(f"{error_ops}", bold=True))
-            if ignored_error_ops:
-                error_str = f"{error_str} ({ignored_error_ops} ignored)"
-
-            rows.append(
-                (
-                    logger.info,
-                    [
-                        host.style_print_prefix(*host_args, **host_kwargs),
-                        changed_str,
-                        "No change: {0}".format(click.style(f"{meta.ops_no_change}", bold=True)),
-                        error_str,
-                    ],
-                ),
-            )
-
-        if i != len(group_combinations):
-            rows.append((lambda m: click.echo(m, err=True), []))
-
-    print_rows(rows)
```

### Comparing `pyinfra-3.0b0/pyinfra_cli/util.py` & `pyinfra-3.0b1/pyinfra_cli/util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/pyinfra_cli/virtualenv.py` & `pyinfra-3.0b1/pyinfra_cli/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/setup.cfg` & `pyinfra-3.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/setup.py` & `pyinfra-3.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/paramiko_util.py` & `pyinfra-3.0b1/tests/paramiko_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api.py` & `pyinfra-3.0b1/tests/test_api/test_api.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_arguments.py` & `pyinfra-3.0b1/tests/test_api/test_api_arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_command.py` & `pyinfra-3.0b1/tests/test_api/test_api_command.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_config.py` & `pyinfra-3.0b1/tests/test_api/test_api_config.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_deploys.py` & `pyinfra-3.0b1/tests/test_api/test_api_deploys.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,24 +36,24 @@
         # Ensure we have an op
         assert len(op_order) == 2
 
         # Ensure run ops works
         run_ops(state)
 
         first_op_hash = op_order[0]
-        assert state.op_meta[first_op_hash].names == {"test_deploy | Server/Shell"}
+        assert state.op_meta[first_op_hash].names == {"test_deploy | server.shell"}
         assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
         assert state.ops[anotherhost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
 
         second_op_hash = op_order[1]
-        assert state.op_meta[second_op_hash].names == {"test_deploy | Server/Shell"}
+        assert state.op_meta[second_op_hash].names == {"test_deploy | server.shell"}
         assert state.ops[somehost][second_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
         assert state.ops[anotherhost][second_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
 
@@ -100,25 +100,25 @@
         # Ensure we have an op
         assert len(op_order) == 3
 
         # Ensure run ops works
         run_ops(state)
 
         first_op_hash = op_order[0]
-        assert state.op_meta[first_op_hash].names == {"test_deploy | Server/Shell"}
+        assert state.op_meta[first_op_hash].names == {"test_deploy | server.shell"}
         assert state.ops[somehost][first_op_hash].operation_meta._commands == [
             StringCommand("echo first command"),
         ]
 
         second_op_hash = op_order[1]
         assert state.op_meta[second_op_hash].names == {
-            "test_deploy | test_nested_deploy | Server/Shell",
+            "test_deploy | test_nested_deploy | server.shell",
         }
         assert state.ops[somehost][second_op_hash].operation_meta._commands == [
             StringCommand("echo nested command"),
         ]
 
         third_op_hash = op_order[2]
-        assert state.op_meta[third_op_hash].names == {"test_deploy | Server/Shell"}
+        assert state.op_meta[third_op_hash].names == {"test_deploy | server.shell"}
         assert state.ops[somehost][third_op_hash].operation_meta._commands == [
             StringCommand("echo second command"),
         ]
```

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_facts.py` & `pyinfra-3.0b1/tests/test_api/test_api_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_host.py` & `pyinfra-3.0b1/tests/test_api/test_api_host.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_inventory.py` & `pyinfra-3.0b1/tests/test_api/test_api_inventory.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_operations.py` & `pyinfra-3.0b1/tests/test_api/test_api_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         # Ensure we have an op
         assert len(op_order) == 1
 
         first_op_hash = op_order[0]
 
         # Ensure the op name
-        assert state.op_meta[first_op_hash].names == {"Files/File"}
+        assert state.op_meta[first_op_hash].names == {"files.file"}
 
         # Ensure the global kwargs (same for both hosts)
         somehost_global_arguments = state.ops[somehost][first_op_hash].global_arguments
         assert somehost_global_arguments["_sudo"] is True
         assert somehost_global_arguments["_sudo_user"] == "test_sudo"
         assert somehost_global_arguments["_su_user"] == "test_su"
         assert somehost_global_arguments["_ignore_errors"] is True
@@ -429,29 +429,29 @@
         ctx_state.set(state)
         ctx_host.set(somehost)
 
         pyinfra.is_cli = True
 
         try:
             outer_result = server.shell(commands="echo outer")
-            assert outer_result._combined_output_lines is None
+            assert outer_result._combined_output is None
 
             def callback():
                 inner_result = server.shell(commands="echo inner")
-                assert inner_result._combined_output_lines is not None
+                assert inner_result._combined_output is not None
 
             python.call(function=callback)
 
             assert len(state.get_op_order()) == 2
 
             run_ops(state)
 
             assert len(state.get_op_order()) == 3
             assert state.results[somehost].success_ops == 3
-            assert outer_result._combined_output_lines is not None
+            assert outer_result._combined_output is not None
 
             disconnect_all(state)
         finally:
             pyinfra.is_cli = False
 
 
 class TestOperationFailures(PatchSSHTestCase):
```

### Comparing `pyinfra-3.0b0/tests/test_api/test_api_util.py` & `pyinfra-3.0b1/tests/test_api/test_api_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_cli/test_cli.py` & `pyinfra-3.0b1/tests/test_cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_cli/test_cli_deploy.py` & `pyinfra-3.0b1/tests/test_cli/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_cli/test_cli_exceptions.py` & `pyinfra-3.0b1/tests/test_cli/test_cli_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_cli/test_cli_util.py` & `pyinfra-3.0b1/tests/test_cli/test_cli_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_cli/test_context_objects.py` & `pyinfra-3.0b1/tests/test_cli/test_context_objects.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_chroot.py` & `pyinfra-3.0b1/tests/test_connectors/test_chroot.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_docker.py` & `pyinfra-3.0b1/tests/test_connectors/test_docker.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_dockerssh.py` & `pyinfra-3.0b1/tests/test_connectors/test_dockerssh.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_local.py` & `pyinfra-3.0b1/tests/test_connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_ssh.py` & `pyinfra-3.0b1/tests/test_connectors/test_ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -997,7 +997,59 @@
         with patch("pyinfra.api.util.open", fake_open, create=True):
             with self.assertRaises(ConnectError):
                 host.put_file(
                     "not-a-file",
                     "not-another-file",
                     print_output=True,
                 )
+
+    @patch("pyinfra.connectors.ssh.SSHClient")
+    @patch("time.sleep")
+    def test_ssh_connect_fail_retry(self, fake_sleep, fake_ssh_client):
+        for exception_class in (
+            SSHException,
+            gaierror,
+            socket_error,
+            EOFError,
+        ):
+            inventory = make_inventory(
+                hosts=("unresposivehost",), override_data={"ssh_connect_retries": 1}
+            )
+            State(inventory, Config())
+
+            unresposivehost = inventory.get_host("unresposivehost")
+            assert unresposivehost.data.ssh_connect_retries == 1
+
+            fake_ssh = MagicMock()
+            fake_ssh.connect.side_effect = exception_class()
+            fake_ssh_client.return_value = fake_ssh
+
+            with self.assertRaises(ConnectError):
+                unresposivehost.connect(show_errors=False, raise_exceptions=True)
+            assert fake_sleep.called_once()
+            assert fake_ssh_client.connect.called_twice()
+
+    @patch("pyinfra.connectors.ssh.SSHClient")
+    @patch("time.sleep")
+    def test_ssh_connect_fail_success(self, fake_sleep, fake_ssh_client):
+        for exception_class in (
+            SSHException,
+            gaierror,
+            socket_error,
+            EOFError,
+        ):
+            inventory = make_inventory(
+                hosts=("unresposivehost",), override_data={"ssh_connect_retries": 1}
+            )
+            State(inventory, Config())
+
+            unresposivehost = inventory.get_host("unresposivehost")
+            assert unresposivehost.data.ssh_connect_retries == 1
+
+            connection = MagicMock()
+            fake_ssh = MagicMock()
+            fake_ssh.connect.side_effect = [exception_class(), connection]
+            fake_ssh_client.return_value = fake_ssh
+
+            unresposivehost.connect(show_errors=False, raise_exceptions=True)
+            assert fake_sleep.called_once()
+            assert fake_ssh_client.connect.called_twice()
```

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_sshuserclient.py` & `pyinfra-3.0b1/tests/test_connectors/test_sshuserclient.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_terraform.py` & `pyinfra-3.0b1/tests/test_connectors/test_terraform.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 from unittest.mock import patch
 
 from pyinfra.api.exceptions import InventoryError
 from pyinfra.connectors.terraform import TerraformInventoryConnector
 
 
 class TestTerraformConnector(TestCase):
-    def test_make_names_data_no_output_key(self):
-        with self.assertRaises(InventoryError) as context:
-            list(TerraformInventoryConnector.make_names_data())
-
-        assert context.exception.args[0] == "No Terraform output key!"
-
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_no_output(self, fake_shell):
-        fake_shell.return_value = json.dumps({})
+        fake_shell.return_value = json.dumps(
+            {
+                "hello": {
+                    "world": [],
+                },
+            },
+        )
 
         with self.assertRaises(InventoryError) as context:
             list(TerraformInventoryConnector.make_names_data("output_key"))
 
-        assert context.exception.args[0] == "No Terraform output with key: `output_key`"
+        assert (
+            context.exception.args[0]
+            == "No Terraform output with key: `output_key`, valid keys:\n   - hello.world"
+        )
 
     @patch("pyinfra.connectors.terraform.local.shell")
     def test_make_names_data_invalid_output(self, fake_shell):
         fake_shell.return_value = json.dumps({"output_key": "wrongvalue"})
 
         with self.assertRaises(InventoryError) as context:
             list(TerraformInventoryConnector.make_names_data("output_key"))
```

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_util.py` & `pyinfra-3.0b1/tests/test_connectors/test_util.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_connectors/test_vagrant.py` & `pyinfra-3.0b1/tests/test_connectors/test_vagrant.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @patch(
         "pyinfra.connectors.vagrant.open",
         mock_open(read_data=FAKE_VAGRANT_OPTIONS_DATA),
         create=True,
     )
     @patch("pyinfra.connectors.vagrant.path.exists", lambda path: True)
     def test_make_names_data_with_options(self):
-        data = VagrantInventoryConnector.make_names_data()
+        data = list(VagrantInventoryConnector.make_names_data())
 
         assert data == [
             (
                 "@vagrant/ubuntu16",
                 {
                     "ssh_port": "2222",
                     "ssh_user": "vagrant",
@@ -99,15 +99,15 @@
                     "ssh_hostname": "127.0.0.1",
                 },
                 ["@vagrant"],
             ),
         ]
 
     def test_make_names_data_with_limit(self):
-        data = VagrantInventoryConnector.make_names_data(limit=("ubuntu16",))
+        data = list(VagrantInventoryConnector.make_names_data(name=("ubuntu16",)))
 
         assert data == [
             (
                 "@vagrant/ubuntu16",
                 {
                     "ssh_port": "2222",
                     "ssh_user": "vagrant",
@@ -116,8 +116,8 @@
                 },
                 ["@vagrant"],
             ),
         ]
 
     def test_make_names_data_no_matches(self):
         with self.assertRaises(InventoryError):
-            VagrantInventoryConnector.make_names_data(limit="nope")
+            list(VagrantInventoryConnector.make_names_data(name="nope"))
```

### Comparing `pyinfra-3.0b0/tests/test_facts.py` & `pyinfra-3.0b1/tests/test_facts.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_global_arguments.py` & `pyinfra-3.0b1/tests/test_global_arguments.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_operations.py` & `pyinfra-3.0b1/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/test_operations_utils.py` & `pyinfra-3.0b1/tests/test_operations_utils.py`

 * *Files identical despite different names*

### Comparing `pyinfra-3.0b0/tests/util.py` & `pyinfra-3.0b1/tests/util.py`

 * *Files identical despite different names*

