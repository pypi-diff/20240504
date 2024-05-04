# Comparing `tmp/pyadic-0.2.0.tar.gz` & `tmp/pyadic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyadic-0.2.0.tar", last modified: Tue Jan  2 16:43:11 2024, max compression
+gzip compressed data, was "pyadic-0.2.1.tar", last modified: Sat May  4 20:11:15 2024, max compression
```

## Comparing `pyadic-0.2.0.tar` & `pyadic-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,26 @@
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/.github/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/.github/workflows/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1175 2023-09-08 13:20:44.000000 pyadic-0.2.0/.github/workflows/continuous_integration.yml
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       79 2023-09-08 13:20:00.000000 pyadic-0.2.0/.gitignore
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       15 2022-07-25 22:46:02.000000 pyadic-0.2.0/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    35149 2022-03-24 18:46:40.000000 pyadic-0.2.0/LICENSE.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4174 2024-01-02 16:43:11.800854 pyadic-0.2.0/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     3421 2023-12-22 19:32:14.000000 pyadic-0.2.0/README.md
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/pyadic/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.2.0/pyadic/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      171 2023-12-22 12:00:09.000000 pyadic-0.2.0/pyadic/__init__.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4006 2023-09-06 15:57:31.000000 pyadic-0.2.0/pyadic/field_extension.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    13675 2023-12-22 18:41:11.000000 pyadic-0.2.0/pyadic/finite_field.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     3819 2023-12-22 11:53:24.000000 pyadic-0.2.0/pyadic/gaussian_rationals.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     3635 2023-09-05 10:32:48.000000 pyadic-0.2.0/pyadic/interpolation.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    13274 2023-09-06 15:57:35.000000 pyadic-0.2.0/pyadic/padic.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1380 2023-04-03 14:45:28.000000 pyadic-0.2.0/pyadic/primes.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/pyadic.egg-info/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4174 2024-01-02 16:43:11.000000 pyadic-0.2.0/pyadic.egg-info/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      542 2024-01-02 16:43:11.000000 pyadic-0.2.0/pyadic.egg-info/SOURCES.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        1 2024-01-02 16:43:11.000000 pyadic-0.2.0/pyadic.egg-info/dependency_links.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       12 2024-01-02 16:43:11.000000 pyadic-0.2.0/pyadic.egg-info/requires.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        7 2024-01-02 16:43:11.000000 pyadic-0.2.0/pyadic.egg-info/top_level.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       14 2022-10-21 11:06:30.000000 pyadic-0.2.0/runtime.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      201 2024-01-02 16:43:11.800854 pyadic-0.2.0/setup.cfg
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1160 2024-01-02 16:14:08.000000 pyadic-0.2.0/setup.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2024-01-02 16:43:11.800854 pyadic-0.2.0/tests/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       11 2022-07-25 22:51:57.000000 pyadic-0.2.0/tests/.hidden
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1897 2023-09-06 14:08:59.000000 pyadic-0.2.0/tests/test_field_extension.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     6036 2023-12-22 11:56:32.000000 pyadic-0.2.0/tests/test_finite_field.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4802 2023-12-22 11:54:42.000000 pyadic-0.2.0/tests/test_padic.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1253 2022-07-25 22:36:25.000000 pyadic-0.2.0/update-badges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:11:15.423061 pyadic-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 20:11:03.000000 pyadic-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-04 20:11:15.423061 pyadic-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-04 20:11:03.000000 pyadic-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:11:15.419061 pyadic-0.2.1/pyadic/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/field_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/finite_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/gaussian_rationals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/padic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-04 20:11:03.000000 pyadic-0.2.1/pyadic/primes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:11:15.423061 pyadic-0.2.1/pyadic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-04 20:11:15.000000 pyadic-0.2.1/pyadic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-04 20:11:15.000000 pyadic-0.2.1/pyadic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 20:11:15.000000 pyadic-0.2.1/pyadic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-04 20:11:15.000000 pyadic-0.2.1/pyadic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 20:11:15.000000 pyadic-0.2.1/pyadic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-04 20:11:15.423061 pyadic-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-04 20:11:03.000000 pyadic-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 20:11:15.423061 pyadic-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-04 20:11:03.000000 pyadic-0.2.1/tests/test_field_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-04 20:11:03.000000 pyadic-0.2.1/tests/test_finite_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-04 20:11:03.000000 pyadic-0.2.1/tests/test_gaussian_rationals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-04 20:11:03.000000 pyadic-0.2.1/tests/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-04 20:11:03.000000 pyadic-0.2.1/tests/test_padic.py
```

### Comparing `pyadic-0.2.0/LICENSE.txt` & `pyadic-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyadic-0.2.0/PKG-INFO` & `pyadic-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pyadic
-Version: 0.2.0
+Version: 0.2.1
 Summary: p-Adic numbers and finite fields in Python
 Home-page: https://github.com/GDeLaurentis/pyadic
+Download-URL: https://github.com/GDeLaurentis/pyadic/archive/v0.2.0.tar.gz
 Author: Giuseppe De Laurentis
 Author-email: g.dl@hotmail.it
 License: GNU General Public License v3.0
-Download-URL: https://github.com/GDeLaurentis/pyadic/archive/v0.2.0.tar.gz
 Keywords: p-adic numbers,finite-fields,rational reconstruction
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: sympy
 
 # pyAdic
 
-[![Continuous Integration Status](https://github.com/GDeLaurentis/pyadic/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions)
+[![CI Lint](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml)
+[![CI Test](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml)
 [![Coverage](https://img.shields.io/badge/Coverage-91%25-green?labelColor=2a2f35)](https://github.com/GDeLaurentis/pyadic/actions)
-[![pypi](https://img.shields.io/pypi/v/pyadic)](https://pypi.org/project/pyadic/)
+[![PyPI](https://img.shields.io/pypi/v/pyadic?label=PyPI)](https://pypi.org/project/pyadic/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyadic.svg?label=PyPI%20downloads)](https://pypistats.org/packages/pyadic)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GDeLaurentis/pyadic/HEAD)
 
 
-The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
+The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is to mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
 
 In addition to arithmetic operations, the pyadic library also provides the following functions:
 
 - `rationalise` to perform rationalization ($\mathbb{F}_p\rightarrow \mathbb{Q}$ and $\mathbb{Q}_p \rightarrow \mathbb{Q}$);
 - `finite_field_sqrt` and `padic_sqrt` to compute square roots (which may involve `FieldExtension`);
 - `padic_log` to compute the $p$-adic logarithm.
 
@@ -96,8 +98,7 @@
     archivePrefix = "arXiv",
     primaryClass = "hep-th",
     reportNumber = "PSI-PR-23-14",
     month = "5",
     year = "2023"
 }
 ```
-
```

### Comparing `pyadic-0.2.0/README.md` & `pyadic-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # pyAdic
 
-[![Continuous Integration Status](https://github.com/GDeLaurentis/pyadic/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions)
+[![CI Lint](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml)
+[![CI Test](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml)
 [![Coverage](https://img.shields.io/badge/Coverage-91%25-green?labelColor=2a2f35)](https://github.com/GDeLaurentis/pyadic/actions)
-[![pypi](https://img.shields.io/pypi/v/pyadic)](https://pypi.org/project/pyadic/)
+[![PyPI](https://img.shields.io/pypi/v/pyadic?label=PyPI)](https://pypi.org/project/pyadic/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyadic.svg?label=PyPI%20downloads)](https://pypistats.org/packages/pyadic)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GDeLaurentis/pyadic/HEAD)
 
 
-The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
+The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is to mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
 
 In addition to arithmetic operations, the pyadic library also provides the following functions:
 
 - `rationalise` to perform rationalization ($\mathbb{F}_p\rightarrow \mathbb{Q}$ and $\mathbb{Q}_p \rightarrow \mathbb{Q}$);
 - `finite_field_sqrt` and `padic_sqrt` to compute square roots (which may involve `FieldExtension`);
 - `padic_log` to compute the $p$-adic logarithm.
```

### Comparing `pyadic-0.2.0/pyadic/field_extension.py` & `pyadic-0.2.1/pyadic/field_extension.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.2.0/pyadic/finite_field.py` & `pyadic-0.2.1/pyadic/finite_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,21 +56,25 @@
                 b = ModP(n.imag, p)
                 i = finite_field_sqrt(ModP(-1, p))  # this fails if p is a prime power
                 res += i * b
             if isinstance(res, FieldExtension):
                 raise ValueError("Complex to ModP conversion requires √-1 in field or zero imaginary part.")
             self.n = res.n
             self.p = res.p
-        elif p is None and isinstance(n, ModP):
+        elif isinstance(n, ModP):
+            if p is not None:
+                assert p == n.p
             self.n = n.n
             self.p = n.p
         elif p is None and isinstance(n, padic.PAdic):
             self.n = int(n)
-            self.p = n.p ** n.k
-        elif p is None and isinstance(n, str):
+            self.p = n.p ** n._k
+        elif isinstance(n, str) and (n.isnumeric() or n.lstrip("+-").isnumeric()) and p is not None:
+            self.n, self.p = int(n) % int(p), p
+        elif isinstance(n, str):
             self.n, self.p = self.__rstr__(n)
         else:
             raise TypeError('Bad finite field constructor, (n, p) of  value:({}, {}) and type:({}, {}).'.format(n, p, type(n), type(p)))
 
     def __getstate__(self):
         return (int(self), self.p)
 
@@ -156,15 +160,15 @@
             return root_2_res * root_2_res
         else:
             return self * (self ** (n - 1))
 
     def _inv(self):
         """Find multiplicative inverse of self in Z_p (Z mod p) using the extended Euclidean algorithm."""
 
-        s, t, gcd = extended_euclideal_algorithm(int(self), self.p)
+        s, t, gcd = extended_euclidean_algorithm(int(self), self.p)
 
         if gcd != 1:
             raise ZeroDivisionError("Inverse of {} mod {} does not exist. Are you sure {} is prime?".format(self, self.p, self.p))
 
         return ModP(s, self.p)
 
     def __hash__(self):
@@ -189,19 +193,25 @@
             return ModPtensor
         return _vec_ModP_optimized_
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
 
-def extended_euclideal_algorithm(a, b):
+def extended_euclidean_algorithm(a, b):
     """Returns Bezout coefficients (s,t) and gcd(a,b) such that: as+bt=gcd(a,b). - Pseudocode from https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm"""
+
+    # This ensures that the output is of the same type as the input,
+    # e.g. for working with a, b in sympy.polys.rings.PolyElement
+    zero = a * 0
+    one = zero + 1
+
     (old_r, r) = (a, b)
-    (old_s, s) = (1, 0)
-    (old_t, t) = (0, 1)
+    (old_s, s) = (one, zero)
+    (old_t, t) = (zero, one)
 
     while r != 0:
         quotient = old_r // r
         (old_r, r) = (r, old_r - quotient * r)
         (old_s, s) = (s, old_s - quotient * s)
         (old_t, t) = (t, old_t - quotient * t)
 
@@ -209,15 +219,15 @@
     # output "greatest common divisor:", old_r
     # output "quotients by the gcd:", (t, s)
 
     return (old_s, old_t, old_r)
 
 
 def gcd(a, b):
-    _, _, gcd = extended_euclideal_algorithm(a, b)
+    _, _, gcd = extended_euclidean_algorithm(a, b)
     return gcd
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
 
 def MQRR(u, m, T=None):
@@ -273,26 +283,26 @@
     """Given (a, n) returns a fraction r / s such that r/s % n = a, by lattice reduction. r = sa + mn  <-> r/s % n = a"""
     if n is None:  # for FF argument
         if isinstance(a, int):
             return fractions.Fraction(a, 1)
         elif isinstance(a, ModP):
             return rationalise(int(a), a.p, algorithm)
         elif isinstance(a, padic.PAdic):
-            return rationalise(int(a), a.p ** a.k, algorithm)
+            return rationalise(int(a), a.p ** a.k, algorithm) * fractions.Fraction(a.p) ** a.n
     return algorithm(a, n)
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
 
 def chinese_remainder(a1, a2):
     """Given a1 = a % n1 and a2 = a % n2 and assuming gcd(n1,n2)=1 (i.e. n1, n2 co-prime), returns a12 = a % (n1*n2)"""
     a1, n1 = int(a1), a1.p
     a2, n2 = int(a2), a2.p
-    q1, q2, gcd = extended_euclideal_algorithm(n1, n2)
+    q1, q2, gcd = extended_euclidean_algorithm(n1, n2)
     assert gcd == 1
     return ModP(a1 * (q2 * n2) + a2 * (q1 * n1), n1 * n2)
 
 
 def chained_chinese_remainder(*vals, primes=None):
     """Vectorized (concatenated) version of chinese remainder function."""
     if not (all([isinstance(val, ModP) for val in vals]) or len(vals) == len(primes)):
```

### Comparing `pyadic-0.2.0/pyadic/gaussian_rationals.py` & `pyadic-0.2.1/pyadic/gaussian_rationals.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.2.0/pyadic/padic.py` & `pyadic-0.2.1/pyadic/padic.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,28 +115,34 @@
                 self.num = self.num + p ** self.k * full_range_random_padic_filling(self.p, factors_of_p)
                 self.k = self.k + factors_of_p
             if all_precision_loss_warning and self.k == 0:
                 print("Lost all precision @", self)
         elif isinstance(num, fractions.Fraction):
             res = PAdic(num.numerator, p, k, n, from_addition) / PAdic(num.denominator, p, k, n, from_addition)
             self.num, self.p, self.k, self.n = res.num, res.p, res.k, res.n
+        elif isinstance(num, PAdic):
+            self.num, self.p, self.k, self.n = num.num, num.p, num.k, num.n
         elif hasattr(num, "imag"):
             res = PAdic(num.real, p, k, n, from_addition)
             if num.imag != 0:
                 b = PAdic(num.imag, p, k, n, from_addition)
                 i = padic_sqrt(PAdic(-1, p, k, n, from_addition))
                 res += + i * b
             if isinstance(res, FieldExtension):
                 raise ValueError(f"Can't create {p}-adic from {num}. A field extension is required.")
             self.p = res.p
             self.k = res.k
             self.n = res.n
             self.num = res.num
-        elif isinstance(num, str):
+        elif p is None and k is None and isinstance(num, str):
             self.num, self.p, self.k, self.n = self.__rstr__(num)
+        elif isinstance(num, str):
+            num = fractions.Fraction(num)
+            res = PAdic(num.numerator, p, k, n, from_addition) / PAdic(num.denominator, p, k, n, from_addition)
+            self.num, self.p, self.k, self.n = res.num, res.p, res.k, res.n
         else:
             raise Exception(f"Invalid p-adic initialisation: {num}, {p}, {k}, {n}, {from_addition}.")
 
     # GETTERS and SETTERS
 
     @property
     def num(self):
@@ -169,16 +175,24 @@
         """k: number of significant digits."""
         if value < 0:
             value = 0
         self._k = value
 
     @property
     def as_tuple(self):
+        """Tuple reprensentation of the mantissa."""
         return (to_base(int(self), self.p) + tuple([0 for i in range(self.k)]))[:self.k]
 
+    @property
+    def as_tuple_from_zero(self):
+        """Tuple representation of the mantissa, shifted to start from p^0 term."""
+        if self.n < 0:
+            raise ValueError("PAdic tuple from zero representation is only defined for PAdic integers (non-negative valuation).")
+        return (0, ) * self.n + self.as_tuple
+
     def __getstate__(self):
         return (int(self), self.p, self.k, self.n)
 
     def __setstate__(self, state):
         self.__init__(*state)
 
     def __str__(self):
```

### Comparing `pyadic-0.2.0/pyadic/primes.py` & `pyadic-0.2.1/pyadic/primes.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.2.0/pyadic.egg-info/PKG-INFO` & `pyadic-0.2.1/pyadic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: pyadic
-Version: 0.2.0
+Version: 0.2.1
 Summary: p-Adic numbers and finite fields in Python
 Home-page: https://github.com/GDeLaurentis/pyadic
+Download-URL: https://github.com/GDeLaurentis/pyadic/archive/v0.2.0.tar.gz
 Author: Giuseppe De Laurentis
 Author-email: g.dl@hotmail.it
 License: GNU General Public License v3.0
-Download-URL: https://github.com/GDeLaurentis/pyadic/archive/v0.2.0.tar.gz
 Keywords: p-adic numbers,finite-fields,rational reconstruction
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: sympy
 
 # pyAdic
 
-[![Continuous Integration Status](https://github.com/GDeLaurentis/pyadic/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions)
+[![CI Lint](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_lint.yml)
+[![CI Test](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml/badge.svg)](https://github.com/GDeLaurentis/pyadic/actions/workflows/ci_test.yml)
 [![Coverage](https://img.shields.io/badge/Coverage-91%25-green?labelColor=2a2f35)](https://github.com/GDeLaurentis/pyadic/actions)
-[![pypi](https://img.shields.io/pypi/v/pyadic)](https://pypi.org/project/pyadic/)
+[![PyPI](https://img.shields.io/pypi/v/pyadic?label=PyPI)](https://pypi.org/project/pyadic/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/pyadic.svg?label=PyPI%20downloads)](https://pypistats.org/packages/pyadic)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/GDeLaurentis/pyadic/HEAD)
 
 
-The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
+The `pyadic` library is Python 3 package that provides number types for finite fields $\mathbb{F}_p$ (`ModP`) and $p$-adic numbers $\mathbb{Q}_p$ (`PAdic`). The goal is to mimic the flexible behavior of built-in types, such as `int`, `float` and `complex`. Thus, one can mix-and-match the different number types, as long as the operations are consistent. In particular, `ModP` and `PAdic` are compatible with `fractions.Fraction`.
 
 In addition to arithmetic operations, the pyadic library also provides the following functions:
 
 - `rationalise` to perform rationalization ($\mathbb{F}_p\rightarrow \mathbb{Q}$ and $\mathbb{Q}_p \rightarrow \mathbb{Q}$);
 - `finite_field_sqrt` and `padic_sqrt` to compute square roots (which may involve `FieldExtension`);
 - `padic_log` to compute the $p$-adic logarithm.
 
@@ -96,8 +98,7 @@
     archivePrefix = "arXiv",
     primaryClass = "hep-th",
     reportNumber = "PSI-PR-23-14",
     month = "5",
     year = "2023"
 }
 ```
-
```

### Comparing `pyadic-0.2.0/setup.py` & `pyadic-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pyadic',
-    version='0.2.0',
+    version='0.2.1',
     license='GNU General Public License v3.0',
     description='p-Adic numbers and finite fields in Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Giuseppe De Laurentis',
     author_email='g.dl@hotmail.it',
     url='https://github.com/GDeLaurentis/pyadic',
```

### Comparing `pyadic-0.2.0/tests/test_field_extension.py` & `pyadic-0.2.1/tests/test_field_extension.py`

 * *Files identical despite different names*

### Comparing `pyadic-0.2.0/tests/test_finite_field.py` & `pyadic-0.2.1/tests/test_finite_field.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pytest
 import sympy
 import numpy
 
 from fractions import Fraction as Q
 
 from pyadic import ModP, PAdic
-from pyadic.finite_field import vec_ModP, extended_euclideal_algorithm, rationalise, MQRR, LGRR, \
+from pyadic.finite_field import vec_ModP, extended_euclidean_algorithm, rationalise, MQRR, LGRR, \
     finite_field_sqrt, chained_chinese_remainder, vec_chained_FF_rationalize
 from pyadic.field_extension import FieldExtension
 from pyadic.primes import primes
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
@@ -27,14 +27,18 @@
     assert ModP(ModP(123, 2 ** 31 - 19)) == + ModP(123, 2 ** 31 - 19)
 
 
 def test_instantiation_from_padic():
     assert ModP(PAdic(123, 2 ** 31 - 19, 3)) == ModP(123, (2 ** 31 - 19) ** 3)
 
 
+def test_instantiation_from_string():
+    assert ModP('+123', 2 ** 31 - 1) == ModP('-2147483524', 2 ** 31 - 1) == ModP(123, 2 ** 31 - 1)
+
+
 def test_instantiation_with_complex():
     p = 2 ** 31 - 19
     assert ModP(1, p) * (2 + 3j) == ModP(2, p) + finite_field_sqrt(ModP(-1, p)) * ModP(3, p) == ModP(2 + 3j, p)
 
 
 def test_instantiation_with_complex_requires_field_extension():
     p = 2 ** 31 - 1
@@ -151,18 +155,18 @@
     assert abs(ModP(-1, 10007)) > abs(ModP(0, 10007))
 
 
 def test_hash():
     hash(ModP(12345, 10007))
 
 
-def test_extended_euclideal_algorithm():
+def test_extended_euclidean_algorithm():
     for i in range(10):
         a, b = random.randint(1, 1000), random.randint(1, 1000)
-        s, t, gcd = extended_euclideal_algorithm(a, b)
+        s, t, gcd = extended_euclidean_algorithm(a, b)
         assert a * s + b * t == gcd
 
 
 def test_reconstruction_MQRR_2147483647():
     assert rationalise(298260199, 2147483647, algorithm=MQRR) == Q(-51071, 36)
```

### Comparing `pyadic-0.2.0/tests/test_padic.py` & `pyadic-0.2.1/tests/test_padic.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,22 @@
 
 
 def test_str_non_zero():
     p, k = 10007, 3
     assert str(PAdic(1 + 2 * p + 3 * p ** 2, p, k)) == "1 + 2*{p} + 3*{p}^2 + O({p}^{k})".format(p=p, k=k)
 
 
+def test_tuple_from_zero_representation():
+    a = PAdic(64, 2, 12)
+    assert a.as_tuple_from_zero == (0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, )
+    a = PAdic(Q(1, 2), 2, 12)
+    with pytest.raises(ValueError):
+        a.as_tuple_from_zero
+
+
 def test_isscalar():
     assert numpy.isscalar(PAdic(3, 7, 1))
 
 
 def test_addition():
     p, k = 10007, 3
     a, b = random.randrange(0, 10000), random.randrange(0, 10000)
@@ -122,19 +130,26 @@
 def test_absolute_value():
     p = 2 ** 31 - 1
     assert PAdic(1, p, 3, -1) > PAdic(1, p, 3, 0) > PAdic(1, p, 3, 1)
     assert PAdic(1, p, 3, 1) < PAdic(1, p, 3, 0) < PAdic(1, p, 3, -1)
     assert abs(PAdic(1, p, 3, 0)) == abs(PAdic(2, p, 3, 0))
 
 
-def test_rationalisation_padic():
+def test_rationalisation_padic_integer():
     assert rationalise(PAdic(Q(7, 13), 2147483647, 12), algorithm=LGRR) == Q(7, 13)
     assert rationalise(PAdic(Q(7, 13), 2147483647, 12), algorithm=MQRR) == Q(7, 13)
 
 
+def test_rationalisation_padic_number():
+    assert rationalise(PAdic(Q(3, 8), 2, 12), algorithm=LGRR) == Q(3, 8)
+    assert rationalise(PAdic(Q(3, 8), 2, 12), algorithm=MQRR) == Q(3, 8)
+    assert rationalise(PAdic(Q(49, 2), 7, 12), algorithm=LGRR) == Q(49, 2)
+    assert rationalise(PAdic(Q(49, 2), 7, 12), algorithm=MQRR) == Q(49, 2)
+
+
 def test_fixed_relative_precision_is_more_stable_but_not_O_guaranteed():
     p = 2 ** 31 - 1
     x = PAdic(1, p, 3)
     y = PAdic(1 - p, p, 3)
     pyadic.padic.fixed_relative_precision = False
     assert (1 / (x - y) - 1 / (x - y)).n == 1                   # fewer digits in result
     assert str(1 / (x - y) - 1 / (x - y)) == "O(2147483647)"    # but precision of result is correctly tracked to O(p)
```

