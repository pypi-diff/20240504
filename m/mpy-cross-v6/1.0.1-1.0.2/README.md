# Comparing `tmp/mpy-cross-v6-1.0.1.tar.gz` & `tmp/mpy_cross_v6-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpy-cross-v6-1.0.1.tar", last modified: Thu Feb 16 20:50:42 2023, max compression
+gzip compressed data, was "mpy_cross_v6-1.0.2.tar", last modified: Sat May  4 21:00:48 2024, max compression
```

## Comparing `mpy-cross-v6-1.0.1.tar` & `mpy_cross_v6-1.0.2.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.559968 mpy-cross-v6-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-16 20:50:42.559968 mpy-cross-v6-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.523968 mpy-cross-v6-1.0.1/micropython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.523968 mpy-cross-v6-1.0.1/micropython/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10008 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.527968 mpy-cross-v6-1.0.1/micropython/mpy-cross/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/gccollect.c
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/mpconfigport.h
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/mphalport.h
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/mpy-cross.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/mpy-cross/qstrdefsport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.547968 mpy-cross-v6-1.0.1/micropython/py/
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/argcheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmarm.c
--rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmarm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmbase.c
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmbase.h
--rw-r--r--   0 runner    (1001) docker     (123)    22763 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmthumb.c
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmthumb.h
--rw-r--r--   0 runner    (1001) docker     (123)    23504 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmx64.c
--rw-r--r--   0 runner    (1001) docker     (123)    10697 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmx64.h
--rw-r--r--   0 runner    (1001) docker     (123)    19404 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmx86.c
--rw-r--r--   0 runner    (1001) docker     (123)    10558 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmx86.h
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmxtensa.c
--rw-r--r--   0 runner    (1001) docker     (123)    18289 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/asmxtensa.h
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/bc.c
--rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/bc.h
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/bc0.h
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/binary.c
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/binary.h
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/builtin.h
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/builtinevex.c
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/builtinhelp.c
--rw-r--r--   0 runner    (1001) docker     (123)    24973 2023-02-16 20:50:32.000000 mpy-cross-v6-1.0.1/micropython/py/builtinimport.c
--rw-r--r--   0 runner    (1001) docker     (123)   147838 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/compile.c
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/compile.h
--rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/dynruntime.h
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/dynruntime.mk
--rw-r--r--   0 runner    (1001) docker     (123)    14701 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emit.h
--rw-r--r--   0 runner    (1001) docker     (123)    33763 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitbc.c
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitcommon.c
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitglue.c
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitglue.h
--rw-r--r--   0 runner    (1001) docker     (123)    34694 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitinlinethumb.c
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitinlinextensa.c
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnarm.c
--rw-r--r--   0 runner    (1001) docker     (123)   126889 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnative.c
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnthumb.c
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnx64.c
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnx86.c
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnxtensa.c
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/emitnxtensawin.c
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/formatfloat.c
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/formatfloat.h
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/frozenmod.c
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/frozenmod.h
--rw-r--r--   0 runner    (1001) docker     (123)    35400 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/gc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/gc.h
--rw-r--r--   0 runner    (1001) docker     (123)    23548 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/grammar.h
--rw-r--r--   0 runner    (1001) docker     (123)    32877 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/lexer.c
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/lexer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/makecompresseddata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/makemoduledefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/makeqstrdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/makeqstrdefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/makeversionhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/malloc.c
--rw-r--r--   0 runner    (1001) docker     (123)    17435 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/map.c
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/misc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mkenv.mk
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mkrules.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mkrules.mk
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modarray.c
--rw-r--r--   0 runner    (1001) docker     (123)    31505 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modbuiltins.c
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modcmath.c
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modcollections.c
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modgc.c
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modio.c
--rw-r--r--   0 runner    (1001) docker     (123)    16502 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modmath.c
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modmicropython.c
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modstruct.c
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modsys.c
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/modthread.c
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/moduerrno.c
--rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpconfig.h
--rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mperrno.h
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mphal.h
--rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpprint.c
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpprint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpstate.c
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpstate.h
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpthread.h
--rw-r--r--   0 runner    (1001) docker     (123)    47792 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpz.c
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/mpz.h
--rw-r--r--   0 runner    (1001) docker     (123)    10298 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nativeglue.c
--rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nativeglue.h
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlr.h
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlraarch64.c
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrpowerpc.c
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrsetjmp.c
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrthumb.c
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrx64.c
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrx86.c
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/nlrxtensa.c
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/obj.c
--rw-r--r--   0 runner    (1001) docker     (123)    46112 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/obj.h
--rw-r--r--   0 runner    (1001) docker     (123)    27262 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objarray.c
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objarray.h
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objattrtuple.c
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objbool.c
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objboundmeth.c
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objcell.c
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objclosure.c
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objcomplex.c
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objdeque.c
--rw-r--r--   0 runner    (1001) docker     (123)    23483 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objdict.c
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objenumerate.c
--rw-r--r--   0 runner    (1001) docker     (123)    26024 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objexcept.c
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objexcept.h
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objfilter.c
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objfloat.c
--rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objfun.c
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objfun.h
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objgenerator.c
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objgenerator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objgetitemiter.c
--rw-r--r--   0 runner    (1001) docker     (123)    16201 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objint.c
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objint.h
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objint_longlong.c
--rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objint_mpz.c
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objlist.c
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objmap.c
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objmodule.c
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objmodule.h
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objnamedtuple.c
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objnamedtuple.h
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objnone.c
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objobject.c
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objpolyiter.c
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objproperty.c
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objrange.c
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objreversed.c
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objset.c
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objsingleton.c
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objslice.c
--rw-r--r--   0 runner    (1001) docker     (123)    78600 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objstr.c
--rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objstr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objstringio.c
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objstringio.h
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objstrunicode.c
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objtuple.c
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objtuple.h
--rw-r--r--   0 runner    (1001) docker     (123)    56792 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objtype.c
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objtype.h
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/objzip.c
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/opmethods.c
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/pairheap.c
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/pairheap.h
--rw-r--r--   0 runner    (1001) docker     (123)    54922 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parse.c
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parse.h
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parsenum.c
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parsenum.h
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parsenumbase.c
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/parsenumbase.h
--rw-r--r--   0 runner    (1001) docker     (123)    21721 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/persistentcode.c
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/persistentcode.h
--rw-r--r--   0 runner    (1001) docker     (123)    31632 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/profile.c
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/profile.h
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/py.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/py.mk
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/pystack.c
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/pystack.h
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/qstr.c
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/qstr.h
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/qstrdefs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/reader.c
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/reader.h
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/repl.c
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/repl.h
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/ringbuf.c
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/ringbuf.h
--rw-r--r--   0 runner    (1001) docker     (123)    65163 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/runtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/runtime0.h
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/runtime_utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/scheduler.c
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/scope.c
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/scope.h
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/sequence.c
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/showbc.c
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/smallint.c
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/smallint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/stackctrl.c
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/stackctrl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/stream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/stream.h
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/unicode.c
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/unicode.h
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/usermod.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    63459 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/vm.c
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/vmentrytable.h
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/vstr.c
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/py/warning.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.547968 mpy-cross-v6-1.0.1/micropython/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.547968 mpy-cross-v6-1.0.1/micropython/shared/libc/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/libc/__errno.c
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/libc/abort_.c
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/libc/printf.c
--rw-r--r--   0 runner    (1001) docker     (123)     7030 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/libc/string0.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.547968 mpy-cross-v6-1.0.1/micropython/shared/memzip/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/import.c
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/lexermemzip.c
--rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/make-memzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/memzip.c
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/memzip/memzip.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.551968 mpy-cross-v6-1.0.1/micropython/shared/netutils/
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/netutils/dhcpserver.c
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/netutils/dhcpserver.h
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/netutils/netutils.c
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/netutils/netutils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/netutils/trace.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.551968 mpy-cross-v6-1.0.1/micropython/shared/readline/
--rw-r--r--   0 runner    (1001) docker     (123)    20735 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/readline/readline.c
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/readline/readline.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.551968 mpy-cross-v6-1.0.1/micropython/shared/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_generic.c
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_m0.s
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_m3.s
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_native.c
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/interrupt_char.c
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/interrupt_char.h
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/mpirq.c
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/mpirq.h
--rw-r--r--   0 runner    (1001) docker     (123)    24538 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/pyexec.c
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/pyexec.h
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/semihosting.c
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/semihosting.h
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/stdout_helpers.c
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/runtime/sys_stdio_mphal.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.551968 mpy-cross-v6-1.0.1/micropython/shared/timeutils/
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/timeutils/timeutils.c
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/timeutils/timeutils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.551968 mpy-cross-v6-1.0.1/micropython/shared/upytesthelper/
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/upytesthelper/upytesthelper.c
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/shared/upytesthelper/upytesthelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/micropython/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/.gitattributes
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/micropython/tools/autobuild/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3182 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/autobuild.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-boards.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-cc3200-latest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-downloads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-esp8266-latest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-stm32-extra.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2047 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/autobuild/remove_old_firmware.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8667 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/cc1
--rwxr-xr-x   0 runner    (1001) docker     (123)    23081 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/ci.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6871 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/codeformat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5304 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/codestats.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     5505 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/dfu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/file2h.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      243 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/gen-changelog.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/gen-cpydiff.py
--rw-r--r--   0 runner    (1001) docker     (123)    17076 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/gendoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/insert-usb-ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/makemanifest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7146 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/micropython/tools/mpremote/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/pyboardextended.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpremote/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    65953 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpy-tool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpy_bin2res.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1234 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpy_cross_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36382 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/mpy_ld.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26773 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/pyboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20108 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/pydfu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4224 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/tinytest-codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/uf2conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/uf2families.json
--rw-r--r--   0 runner    (1001) docker     (123)   122555 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/uncrustify.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/upip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/upip_utarfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3847 2023-02-16 20:50:33.000000 mpy-cross-v6-1.0.1/micropython/tools/verifygitlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-16 20:50:42.559968 mpy-cross-v6-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.523968 mpy-cross-v6-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/src/mpy_cross_v6/
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/src/mpy_cross_v6/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/src/mpy_cross_v6/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/src/mpy_cross_v6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-02-16 20:50:42.000000 mpy-cross-v6-1.0.1/src/mpy_cross_v6.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 20:50:42.555968 mpy-cross-v6-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-16 20:50:29.000000 mpy-cross-v6-1.0.1/tests/test_mpy_cross.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.325649 mpy_cross_v6-1.0.2/micropython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.325649 mpy_cross_v6-1.0.2/micropython/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10008 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.325649 mpy_cross_v6-1.0.2/micropython/mpy-cross/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/gccollect.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13362 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/main.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/mpconfigport.h
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/mphalport.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/mpy-cross.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/mpy-cross/qstrdefsport.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.365649 mpy_cross_v6-1.0.2/micropython/py/
+-rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/argcheck.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmarm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmarm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmbase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmbase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmthumb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    19423 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmthumb.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23504 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmx64.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmx64.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmx86.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10558 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmx86.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmxtensa.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18289 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/asmxtensa.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14278 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/bc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15227 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/bc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/bc0.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13816 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/binary.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/binary.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/builtin.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/builtinevex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/builtinhelp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24973 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/builtinimport.c
+-rw-r--r--   0 runner    (1001) docker     (127)   147838 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/compile.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/compile.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13838 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/dynruntime.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/dynruntime.mk
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emit.h
+-rw-r--r--   0 runner    (1001) docker     (127)    33763 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitbc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitcommon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitglue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitglue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34694 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitinlinethumb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12865 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitinlinextensa.c
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnarm.c
+-rw-r--r--   0 runner    (1001) docker     (127)   126889 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnative.c
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnthumb.c
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnx64.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnx86.c
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnxtensa.c
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/emitnxtensawin.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/formatfloat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/formatfloat.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/frozenmod.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/frozenmod.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35400 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/gc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/gc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23548 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/grammar.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32877 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/lexer.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/makecompresseddata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/makemoduledefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/makeqstrdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/makeqstrdefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/makeversionhdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/malloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17435 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/map.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12113 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mkenv.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mkrules.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8489 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mkrules.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modarray.c
+-rw-r--r--   0 runner    (1001) docker     (127)    31505 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modbuiltins.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modcmath.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modcollections.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modgc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16502 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modmath.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modmicropython.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modstruct.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9950 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modsys.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/modthread.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/moduerrno.c
+-rw-r--r--   0 runner    (1001) docker     (127)    67024 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpconfig.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mperrno.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mphal.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpprint.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpprint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpstate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpstate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpthread.h
+-rw-r--r--   0 runner    (1001) docker     (127)    47792 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/mpz.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nativeglue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nativeglue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlraarch64.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrpowerpc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrsetjmp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrthumb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrx64.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrx86.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/nlrxtensa.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21232 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/obj.c
+-rw-r--r--   0 runner    (1001) docker     (127)    46112 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/obj.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27262 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objarray.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objarray.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objattrtuple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objbool.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objboundmeth.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objcell.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objclosure.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9467 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objcomplex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objdeque.c
+-rw-r--r--   0 runner    (1001) docker     (127)    23483 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objdict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objenumerate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26024 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objexcept.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objexcept.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objfilter.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objfloat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20029 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objfun.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objfun.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14565 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objgenerator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objgenerator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objgetitemiter.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16201 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objint.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objint_longlong.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objint_mpz.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20381 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objlist.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objlist.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objmap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objmodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objmodule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objnamedtuple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objnamedtuple.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objnone.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objobject.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objpolyiter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objproperty.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7541 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objrange.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objreversed.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21330 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objsingleton.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objslice.c
+-rw-r--r--   0 runner    (1001) docker     (127)    78600 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objstr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objstr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objstringio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objstringio.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objstrunicode.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objtuple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objtuple.h
+-rw-r--r--   0 runner    (1001) docker     (127)    56792 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objtype.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objtype.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/objzip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/opmethods.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/pairheap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/pairheap.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parse.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parsenum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parsenum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parsenumbase.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/parsenumbase.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/persistentcode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/persistentcode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/profile.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/profile.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/py.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/py.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/pystack.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/pystack.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14220 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/qstr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/qstr.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/qstrdefs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/reader.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/reader.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10771 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/repl.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/repl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/ringbuf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/ringbuf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    65163 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/runtime.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/runtime.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/runtime0.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/runtime_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/scheduler.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/scope.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/scope.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/sequence.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17987 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/showbc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/smallint.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/smallint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/stackctrl.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/stackctrl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/stream.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/stream.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/unicode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/unicode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/usermod.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)    63459 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/vm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/vmentrytable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/vstr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/py/warning.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.365649 mpy_cross_v6-1.0.2/micropython/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.365649 mpy_cross_v6-1.0.2/micropython/shared/libc/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/libc/__errno.c
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/libc/abort_.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/libc/printf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/libc/string0.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.365649 mpy_cross_v6-1.0.2/micropython/shared/memzip/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/import.c
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/lexermemzip.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2521 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/make-memzip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/memzip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/memzip/memzip.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.369650 mpy_cross_v6-1.0.2/micropython/shared/netutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/netutils/dhcpserver.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/netutils/dhcpserver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/netutils/netutils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/netutils/netutils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/netutils/trace.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.369650 mpy_cross_v6-1.0.2/micropython/shared/readline/
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/readline/readline.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/readline/readline.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.369650 mpy_cross_v6-1.0.2/micropython/shared/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_m0.s
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_m3.s
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_native.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/interrupt_char.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/interrupt_char.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/mpirq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/mpirq.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24538 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/pyexec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/pyexec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/semihosting.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/semihosting.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/stdout_helpers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/runtime/sys_stdio_mphal.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.369650 mpy_cross_v6-1.0.2/micropython/shared/timeutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/timeutils/timeutils.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/timeutils/timeutils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.373649 mpy_cross_v6-1.0.2/micropython/shared/upytesthelper/
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/upytesthelper/upytesthelper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/shared/upytesthelper/upytesthelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.377649 mpy_cross_v6-1.0.2/micropython/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/.gitattributes
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.377649 mpy_cross_v6-1.0.2/micropython/tools/autobuild/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3182 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/autobuild.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3433 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-boards.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      651 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-cc3200-latest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2152 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-downloads.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1591 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-esp8266-latest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1778 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-stm32-extra.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2047 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/autobuild/remove_old_firmware.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8667 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/cc1
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23081 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/ci.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6871 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/codeformat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5304 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/codestats.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5505 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/dfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/file2h.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      243 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/gen-changelog.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9314 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/gen-cpydiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17076 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/gendoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/insert-usb-ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/makemanifest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7146 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.377649 mpy_cross_v6-1.0.2/micropython/tools/mpremote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19695 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20113 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/pyboardextended.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       84 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpremote/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65953 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpy-tool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      497 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpy_bin2res.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1234 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpy_cross_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36382 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/mpy_ld.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26773 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/pyboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20108 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/pydfu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4224 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/tinytest-codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/uf2conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/uf2families.json
+-rw-r--r--   0 runner    (1001) docker     (127)   122555 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/uncrustify.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/upip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/upip_utarfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3847 2024-05-04 21:00:41.000000 mpy_cross_v6-1.0.2/micropython/tools/verifygitlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.325649 mpy_cross_v6-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/src/mpy_cross_v6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/src/mpy_cross_v6/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/src/mpy_cross_v6/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/src/mpy_cross_v6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-04 21:00:48.000000 mpy_cross_v6-1.0.2/src/mpy_cross_v6.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 21:00:48.381649 mpy_cross_v6-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-04 21:00:38.000000 mpy_cross_v6-1.0.2/tests/test_mpy_cross.py
```

### Comparing `mpy-cross-v6-1.0.1/PKG-INFO` & `mpy_cross_v6-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpy-cross-v6
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper for the mpy-cross tool from MicroPython.
 Description-Content-Type: text/markdown
 
 # Python packaging for mpy-cross
 
 This repository contains Python packaging to distribute the `mpy-cross` tool
 from [MicroPython](https://github.com/micropython/micropython) via PyPI.
```

### Comparing `mpy-cross-v6-1.0.1/micropython/docs/conf.py` & `mpy_cross_v6-1.0.2/micropython/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/Makefile` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/Makefile`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/README.md` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/README.md`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/gccollect.c` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/gccollect.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/main.c` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/main.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/mpconfigport.h` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/mpconfigport.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/mpy-cross/mpy-cross.vcxproj` & `mpy_cross_v6-1.0.2/micropython/mpy-cross/mpy-cross.vcxproj`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/argcheck.c` & `mpy_cross_v6-1.0.2/micropython/py/argcheck.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmarm.c` & `mpy_cross_v6-1.0.2/micropython/py/asmarm.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmarm.h` & `mpy_cross_v6-1.0.2/micropython/py/asmarm.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmbase.c` & `mpy_cross_v6-1.0.2/micropython/py/asmbase.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmbase.h` & `mpy_cross_v6-1.0.2/micropython/py/asmbase.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmthumb.c` & `mpy_cross_v6-1.0.2/micropython/py/asmthumb.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmthumb.h` & `mpy_cross_v6-1.0.2/micropython/py/asmthumb.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmx64.c` & `mpy_cross_v6-1.0.2/micropython/py/asmx64.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmx64.h` & `mpy_cross_v6-1.0.2/micropython/py/asmx64.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmx86.c` & `mpy_cross_v6-1.0.2/micropython/py/asmx86.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmx86.h` & `mpy_cross_v6-1.0.2/micropython/py/asmx86.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmxtensa.c` & `mpy_cross_v6-1.0.2/micropython/py/asmxtensa.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/asmxtensa.h` & `mpy_cross_v6-1.0.2/micropython/py/asmxtensa.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/bc.c` & `mpy_cross_v6-1.0.2/micropython/py/bc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/bc.h` & `mpy_cross_v6-1.0.2/micropython/py/bc.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/bc0.h` & `mpy_cross_v6-1.0.2/micropython/py/bc0.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/binary.c` & `mpy_cross_v6-1.0.2/micropython/py/binary.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/binary.h` & `mpy_cross_v6-1.0.2/micropython/py/binary.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/builtin.h` & `mpy_cross_v6-1.0.2/micropython/py/builtin.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/builtinevex.c` & `mpy_cross_v6-1.0.2/micropython/py/builtinevex.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/builtinhelp.c` & `mpy_cross_v6-1.0.2/micropython/py/builtinhelp.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/builtinimport.c` & `mpy_cross_v6-1.0.2/micropython/py/builtinimport.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/compile.c` & `mpy_cross_v6-1.0.2/micropython/py/compile.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/compile.h` & `mpy_cross_v6-1.0.2/micropython/py/compile.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/dynruntime.h` & `mpy_cross_v6-1.0.2/micropython/py/dynruntime.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/dynruntime.mk` & `mpy_cross_v6-1.0.2/micropython/py/dynruntime.mk`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emit.h` & `mpy_cross_v6-1.0.2/micropython/py/emit.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitbc.c` & `mpy_cross_v6-1.0.2/micropython/py/emitbc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitcommon.c` & `mpy_cross_v6-1.0.2/micropython/py/emitcommon.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitglue.c` & `mpy_cross_v6-1.0.2/micropython/py/emitglue.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitglue.h` & `mpy_cross_v6-1.0.2/micropython/py/emitglue.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitinlinethumb.c` & `mpy_cross_v6-1.0.2/micropython/py/emitinlinethumb.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitinlinextensa.c` & `mpy_cross_v6-1.0.2/micropython/py/emitinlinextensa.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitnative.c` & `mpy_cross_v6-1.0.2/micropython/py/emitnative.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/emitnx86.c` & `mpy_cross_v6-1.0.2/micropython/py/emitnx86.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/formatfloat.c` & `mpy_cross_v6-1.0.2/micropython/py/formatfloat.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/formatfloat.h` & `mpy_cross_v6-1.0.2/micropython/py/formatfloat.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/frozenmod.c` & `mpy_cross_v6-1.0.2/micropython/py/frozenmod.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/frozenmod.h` & `mpy_cross_v6-1.0.2/micropython/py/frozenmod.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/gc.c` & `mpy_cross_v6-1.0.2/micropython/py/gc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/gc.h` & `mpy_cross_v6-1.0.2/micropython/py/gc.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/grammar.h` & `mpy_cross_v6-1.0.2/micropython/py/grammar.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/lexer.c` & `mpy_cross_v6-1.0.2/micropython/py/lexer.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/lexer.h` & `mpy_cross_v6-1.0.2/micropython/py/lexer.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/makecompresseddata.py` & `mpy_cross_v6-1.0.2/micropython/py/makecompresseddata.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/makemoduledefs.py` & `mpy_cross_v6-1.0.2/micropython/py/makemoduledefs.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/makeqstrdata.py` & `mpy_cross_v6-1.0.2/micropython/py/makeqstrdata.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/makeqstrdefs.py` & `mpy_cross_v6-1.0.2/micropython/py/makeqstrdefs.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/makeversionhdr.py` & `mpy_cross_v6-1.0.2/micropython/py/makeversionhdr.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/malloc.c` & `mpy_cross_v6-1.0.2/micropython/py/malloc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/map.c` & `mpy_cross_v6-1.0.2/micropython/py/map.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/misc.h` & `mpy_cross_v6-1.0.2/micropython/py/misc.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mkenv.mk` & `mpy_cross_v6-1.0.2/micropython/py/mkenv.mk`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mkrules.cmake` & `mpy_cross_v6-1.0.2/micropython/py/mkrules.cmake`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mkrules.mk` & `mpy_cross_v6-1.0.2/micropython/py/mkrules.mk`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modarray.c` & `mpy_cross_v6-1.0.2/micropython/py/modarray.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modbuiltins.c` & `mpy_cross_v6-1.0.2/micropython/py/modbuiltins.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modcmath.c` & `mpy_cross_v6-1.0.2/micropython/py/modcmath.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modcollections.c` & `mpy_cross_v6-1.0.2/micropython/py/modcollections.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modgc.c` & `mpy_cross_v6-1.0.2/micropython/py/modgc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modio.c` & `mpy_cross_v6-1.0.2/micropython/py/modio.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modmath.c` & `mpy_cross_v6-1.0.2/micropython/py/modmath.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modmicropython.c` & `mpy_cross_v6-1.0.2/micropython/py/modmicropython.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modstruct.c` & `mpy_cross_v6-1.0.2/micropython/py/modstruct.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modsys.c` & `mpy_cross_v6-1.0.2/micropython/py/modsys.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/modthread.c` & `mpy_cross_v6-1.0.2/micropython/py/modthread.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/moduerrno.c` & `mpy_cross_v6-1.0.2/micropython/py/moduerrno.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpconfig.h` & `mpy_cross_v6-1.0.2/micropython/py/mpconfig.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mperrno.h` & `mpy_cross_v6-1.0.2/micropython/py/mperrno.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mphal.h` & `mpy_cross_v6-1.0.2/micropython/py/mphal.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpprint.c` & `mpy_cross_v6-1.0.2/micropython/py/mpprint.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpprint.h` & `mpy_cross_v6-1.0.2/micropython/py/mpprint.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpstate.c` & `mpy_cross_v6-1.0.2/micropython/py/mpstate.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpstate.h` & `mpy_cross_v6-1.0.2/micropython/py/mpstate.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpthread.h` & `mpy_cross_v6-1.0.2/micropython/py/mpthread.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpz.c` & `mpy_cross_v6-1.0.2/micropython/py/mpz.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/mpz.h` & `mpy_cross_v6-1.0.2/micropython/py/mpz.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nativeglue.c` & `mpy_cross_v6-1.0.2/micropython/py/nativeglue.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nativeglue.h` & `mpy_cross_v6-1.0.2/micropython/py/nativeglue.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlr.c` & `mpy_cross_v6-1.0.2/micropython/py/nlr.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlr.h` & `mpy_cross_v6-1.0.2/micropython/py/nlr.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlraarch64.c` & `mpy_cross_v6-1.0.2/micropython/py/nlraarch64.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrpowerpc.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrpowerpc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrsetjmp.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrsetjmp.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrthumb.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrthumb.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrx64.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrx64.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrx86.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrx86.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/nlrxtensa.c` & `mpy_cross_v6-1.0.2/micropython/py/nlrxtensa.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/obj.c` & `mpy_cross_v6-1.0.2/micropython/py/obj.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/obj.h` & `mpy_cross_v6-1.0.2/micropython/py/obj.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objarray.c` & `mpy_cross_v6-1.0.2/micropython/py/objarray.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objarray.h` & `mpy_cross_v6-1.0.2/micropython/py/objarray.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objattrtuple.c` & `mpy_cross_v6-1.0.2/micropython/py/objattrtuple.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objbool.c` & `mpy_cross_v6-1.0.2/micropython/py/objbool.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objboundmeth.c` & `mpy_cross_v6-1.0.2/micropython/py/objboundmeth.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objcell.c` & `mpy_cross_v6-1.0.2/micropython/py/objcell.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objclosure.c` & `mpy_cross_v6-1.0.2/micropython/py/objclosure.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objcomplex.c` & `mpy_cross_v6-1.0.2/micropython/py/objcomplex.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objdeque.c` & `mpy_cross_v6-1.0.2/micropython/py/objdeque.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objdict.c` & `mpy_cross_v6-1.0.2/micropython/py/objdict.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objenumerate.c` & `mpy_cross_v6-1.0.2/micropython/py/objenumerate.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objexcept.c` & `mpy_cross_v6-1.0.2/micropython/py/objexcept.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objexcept.h` & `mpy_cross_v6-1.0.2/micropython/py/objexcept.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objfilter.c` & `mpy_cross_v6-1.0.2/micropython/py/objfilter.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objfloat.c` & `mpy_cross_v6-1.0.2/micropython/py/objfloat.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objfun.c` & `mpy_cross_v6-1.0.2/micropython/py/objfun.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objfun.h` & `mpy_cross_v6-1.0.2/micropython/py/objfun.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objgenerator.c` & `mpy_cross_v6-1.0.2/micropython/py/objgenerator.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objgenerator.h` & `mpy_cross_v6-1.0.2/micropython/py/objgenerator.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objgetitemiter.c` & `mpy_cross_v6-1.0.2/micropython/py/objgetitemiter.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objint.c` & `mpy_cross_v6-1.0.2/micropython/py/objint.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objint.h` & `mpy_cross_v6-1.0.2/micropython/py/objint.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objint_longlong.c` & `mpy_cross_v6-1.0.2/micropython/py/objint_longlong.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objint_mpz.c` & `mpy_cross_v6-1.0.2/micropython/py/objint_mpz.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objlist.c` & `mpy_cross_v6-1.0.2/micropython/py/objlist.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objlist.h` & `mpy_cross_v6-1.0.2/micropython/py/objlist.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objmap.c` & `mpy_cross_v6-1.0.2/micropython/py/objmap.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objmodule.c` & `mpy_cross_v6-1.0.2/micropython/py/objmodule.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objmodule.h` & `mpy_cross_v6-1.0.2/micropython/py/objmodule.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objnamedtuple.c` & `mpy_cross_v6-1.0.2/micropython/py/objnamedtuple.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objnamedtuple.h` & `mpy_cross_v6-1.0.2/micropython/py/objnamedtuple.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objnone.c` & `mpy_cross_v6-1.0.2/micropython/py/objnone.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objobject.c` & `mpy_cross_v6-1.0.2/micropython/py/objobject.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objpolyiter.c` & `mpy_cross_v6-1.0.2/micropython/py/objpolyiter.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objproperty.c` & `mpy_cross_v6-1.0.2/micropython/py/objproperty.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objrange.c` & `mpy_cross_v6-1.0.2/micropython/py/objrange.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objreversed.c` & `mpy_cross_v6-1.0.2/micropython/py/objreversed.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objset.c` & `mpy_cross_v6-1.0.2/micropython/py/objset.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objsingleton.c` & `mpy_cross_v6-1.0.2/micropython/py/objsingleton.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objslice.c` & `mpy_cross_v6-1.0.2/micropython/py/objslice.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objstr.c` & `mpy_cross_v6-1.0.2/micropython/py/objstr.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objstr.h` & `mpy_cross_v6-1.0.2/micropython/py/objstr.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objstringio.c` & `mpy_cross_v6-1.0.2/micropython/py/objstringio.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objstringio.h` & `mpy_cross_v6-1.0.2/micropython/py/objstringio.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objstrunicode.c` & `mpy_cross_v6-1.0.2/micropython/py/objstrunicode.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objtuple.c` & `mpy_cross_v6-1.0.2/micropython/py/objtuple.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objtuple.h` & `mpy_cross_v6-1.0.2/micropython/py/objtuple.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objtype.c` & `mpy_cross_v6-1.0.2/micropython/py/objtype.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objtype.h` & `mpy_cross_v6-1.0.2/micropython/py/objtype.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/objzip.c` & `mpy_cross_v6-1.0.2/micropython/py/objzip.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/opmethods.c` & `mpy_cross_v6-1.0.2/micropython/py/opmethods.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/pairheap.c` & `mpy_cross_v6-1.0.2/micropython/py/pairheap.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/pairheap.h` & `mpy_cross_v6-1.0.2/micropython/py/pairheap.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parse.c` & `mpy_cross_v6-1.0.2/micropython/py/parse.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parse.h` & `mpy_cross_v6-1.0.2/micropython/py/parse.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parsenum.c` & `mpy_cross_v6-1.0.2/micropython/py/parsenum.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parsenum.h` & `mpy_cross_v6-1.0.2/micropython/py/parsenum.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parsenumbase.c` & `mpy_cross_v6-1.0.2/micropython/py/parsenumbase.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/parsenumbase.h` & `mpy_cross_v6-1.0.2/micropython/py/parsenumbase.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/persistentcode.c` & `mpy_cross_v6-1.0.2/micropython/py/persistentcode.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/persistentcode.h` & `mpy_cross_v6-1.0.2/micropython/py/persistentcode.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/profile.c` & `mpy_cross_v6-1.0.2/micropython/py/profile.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/profile.h` & `mpy_cross_v6-1.0.2/micropython/py/profile.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/py.cmake` & `mpy_cross_v6-1.0.2/micropython/py/py.cmake`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/py.mk` & `mpy_cross_v6-1.0.2/micropython/py/py.mk`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/pystack.c` & `mpy_cross_v6-1.0.2/micropython/py/pystack.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/pystack.h` & `mpy_cross_v6-1.0.2/micropython/py/pystack.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/qstr.c` & `mpy_cross_v6-1.0.2/micropython/py/qstr.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/qstr.h` & `mpy_cross_v6-1.0.2/micropython/py/qstr.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/qstrdefs.h` & `mpy_cross_v6-1.0.2/micropython/py/qstrdefs.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/reader.c` & `mpy_cross_v6-1.0.2/micropython/py/reader.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/reader.h` & `mpy_cross_v6-1.0.2/micropython/py/reader.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/repl.c` & `mpy_cross_v6-1.0.2/micropython/py/repl.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/repl.h` & `mpy_cross_v6-1.0.2/micropython/py/repl.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/ringbuf.c` & `mpy_cross_v6-1.0.2/micropython/py/ringbuf.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/ringbuf.h` & `mpy_cross_v6-1.0.2/micropython/py/ringbuf.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/runtime.c` & `mpy_cross_v6-1.0.2/micropython/py/runtime.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/runtime.h` & `mpy_cross_v6-1.0.2/micropython/py/runtime.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/runtime0.h` & `mpy_cross_v6-1.0.2/micropython/py/runtime0.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/runtime_utils.c` & `mpy_cross_v6-1.0.2/micropython/py/runtime_utils.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/scheduler.c` & `mpy_cross_v6-1.0.2/micropython/py/scheduler.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/scope.c` & `mpy_cross_v6-1.0.2/micropython/py/scope.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/scope.h` & `mpy_cross_v6-1.0.2/micropython/py/scope.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/sequence.c` & `mpy_cross_v6-1.0.2/micropython/py/sequence.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/showbc.c` & `mpy_cross_v6-1.0.2/micropython/py/showbc.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/smallint.c` & `mpy_cross_v6-1.0.2/micropython/py/smallint.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/smallint.h` & `mpy_cross_v6-1.0.2/micropython/py/smallint.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/stackctrl.c` & `mpy_cross_v6-1.0.2/micropython/py/stackctrl.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/stackctrl.h` & `mpy_cross_v6-1.0.2/micropython/py/stackctrl.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/stream.c` & `mpy_cross_v6-1.0.2/micropython/py/stream.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/stream.h` & `mpy_cross_v6-1.0.2/micropython/py/stream.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/unicode.c` & `mpy_cross_v6-1.0.2/micropython/py/unicode.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/unicode.h` & `mpy_cross_v6-1.0.2/micropython/py/unicode.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/usermod.cmake` & `mpy_cross_v6-1.0.2/micropython/py/usermod.cmake`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/vm.c` & `mpy_cross_v6-1.0.2/micropython/py/vm.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/vmentrytable.h` & `mpy_cross_v6-1.0.2/micropython/py/vmentrytable.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/vstr.c` & `mpy_cross_v6-1.0.2/micropython/py/vstr.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/py/warning.c` & `mpy_cross_v6-1.0.2/micropython/py/warning.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/libc/printf.c` & `mpy_cross_v6-1.0.2/micropython/shared/libc/printf.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/libc/string0.c` & `mpy_cross_v6-1.0.2/micropython/shared/libc/string0.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/memzip/README.md` & `mpy_cross_v6-1.0.2/micropython/shared/memzip/README.md`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/memzip/make-memzip.py` & `mpy_cross_v6-1.0.2/micropython/shared/memzip/make-memzip.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/memzip/memzip.c` & `mpy_cross_v6-1.0.2/micropython/shared/memzip/memzip.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/memzip/memzip.h` & `mpy_cross_v6-1.0.2/micropython/shared/memzip/memzip.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/netutils/dhcpserver.c` & `mpy_cross_v6-1.0.2/micropython/shared/netutils/dhcpserver.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/netutils/dhcpserver.h` & `mpy_cross_v6-1.0.2/micropython/shared/netutils/dhcpserver.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/netutils/netutils.c` & `mpy_cross_v6-1.0.2/micropython/shared/netutils/netutils.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/netutils/netutils.h` & `mpy_cross_v6-1.0.2/micropython/shared/netutils/netutils.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/netutils/trace.c` & `mpy_cross_v6-1.0.2/micropython/shared/netutils/trace.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/readline/readline.c` & `mpy_cross_v6-1.0.2/micropython/shared/readline/readline.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/readline/readline.h` & `mpy_cross_v6-1.0.2/micropython/shared/readline/readline.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper.h` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_generic.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_generic.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_m0.s` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_m0.s`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_m3.s` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_m3.s`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/gchelper_native.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/gchelper_native.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/interrupt_char.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/interrupt_char.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/interrupt_char.h` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/interrupt_char.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/mpirq.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/mpirq.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/mpirq.h` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/mpirq.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/pyexec.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/pyexec.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/pyexec.h` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/pyexec.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/semihosting.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/semihosting.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/semihosting.h` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/semihosting.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/stdout_helpers.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/stdout_helpers.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/runtime/sys_stdio_mphal.c` & `mpy_cross_v6-1.0.2/micropython/shared/runtime/sys_stdio_mphal.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/timeutils/timeutils.c` & `mpy_cross_v6-1.0.2/micropython/shared/timeutils/timeutils.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/timeutils/timeutils.h` & `mpy_cross_v6-1.0.2/micropython/shared/timeutils/timeutils.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/upytesthelper/upytesthelper.c` & `mpy_cross_v6-1.0.2/micropython/shared/upytesthelper/upytesthelper.c`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/shared/upytesthelper/upytesthelper.h` & `mpy_cross_v6-1.0.2/micropython/shared/upytesthelper/upytesthelper.h`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/autobuild.sh` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/autobuild.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-boards.sh` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-boards.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-cc3200-latest.sh` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-cc3200-latest.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-downloads.py` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-downloads.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-esp8266-latest.sh` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-esp8266-latest.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/build-stm32-extra.sh` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/build-stm32-extra.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/autobuild/remove_old_firmware.py` & `mpy_cross_v6-1.0.2/micropython/tools/autobuild/remove_old_firmware.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/cc1` & `mpy_cross_v6-1.0.2/micropython/tools/cc1`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/ci.sh` & `mpy_cross_v6-1.0.2/micropython/tools/ci.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/codeformat.py` & `mpy_cross_v6-1.0.2/micropython/tools/codeformat.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/codestats.sh` & `mpy_cross_v6-1.0.2/micropython/tools/codestats.sh`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/dfu.py` & `mpy_cross_v6-1.0.2/micropython/tools/dfu.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/file2h.py` & `mpy_cross_v6-1.0.2/micropython/tools/file2h.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/gen-cpydiff.py` & `mpy_cross_v6-1.0.2/micropython/tools/gen-cpydiff.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/gendoc.py` & `mpy_cross_v6-1.0.2/micropython/tools/gendoc.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/insert-usb-ids.py` & `mpy_cross_v6-1.0.2/micropython/tools/insert-usb-ids.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/makemanifest.py` & `mpy_cross_v6-1.0.2/micropython/tools/makemanifest.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/metrics.py` & `mpy_cross_v6-1.0.2/micropython/tools/metrics.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/LICENSE` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/LICENSE`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/README.md` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/README.md`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/console.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/console.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/main.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/main.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/mpremote/pyboardextended.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/mpremote/pyboardextended.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpremote/setup.cfg` & `mpy_cross_v6-1.0.2/micropython/tools/mpremote/setup.cfg`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpy-tool.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpy-tool.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpy_cross_all.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpy_cross_all.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/mpy_ld.py` & `mpy_cross_v6-1.0.2/micropython/tools/mpy_ld.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/pyboard.py` & `mpy_cross_v6-1.0.2/micropython/tools/pyboard.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/pydfu.py` & `mpy_cross_v6-1.0.2/micropython/tools/pydfu.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/tinytest-codegen.py` & `mpy_cross_v6-1.0.2/micropython/tools/tinytest-codegen.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/uf2conv.py` & `mpy_cross_v6-1.0.2/micropython/tools/uf2conv.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/uf2families.json` & `mpy_cross_v6-1.0.2/micropython/tools/uf2families.json`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/uncrustify.cfg` & `mpy_cross_v6-1.0.2/micropython/tools/uncrustify.cfg`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/upip.py` & `mpy_cross_v6-1.0.2/micropython/tools/upip.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/upip_utarfile.py` & `mpy_cross_v6-1.0.2/micropython/tools/upip_utarfile.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/micropython/tools/verifygitlog.py` & `mpy_cross_v6-1.0.2/micropython/tools/verifygitlog.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/pyproject.toml` & `mpy_cross_v6-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpy-cross-v6"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python wrapper for the mpy-cross tool from MicroPython."
 readme = "README.md"
 
 [project.scripts]
 mpy-cross-v6 = "mpy_cross_v6:_run"
 
 [tool.setuptools.packages.find]
```

### Comparing `mpy-cross-v6-1.0.1/setup.py` & `mpy_cross_v6-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/src/mpy_cross_v6/__init__.py` & `mpy_cross_v6-1.0.2/src/mpy_cross_v6/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
             args.append(f"-O{optimization_level}")
 
         if small_number_bits is not None:
             args.append(f"-msmall-int-bits={small_number_bits}")
 
         if arch is not None:
-            args.append(f"-arch={arch.value}")
+            args.append(f"-march={arch.value}")
 
         if emit is not None:
             args += ["-X", f"emit={emit.value}"]
 
         if heap_size is not None:
             args += ["-X", f"heapsize={heap_size}"]
```

### Comparing `mpy-cross-v6-1.0.1/src/mpy_cross_v6.egg-info/SOURCES.txt` & `mpy_cross_v6-1.0.2/src/mpy_cross_v6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpy-cross-v6-1.0.1/tests/test_mpy_cross.py` & `mpy_cross_v6-1.0.2/tests/test_mpy_cross.py`

 * *Files identical despite different names*

