# Comparing `tmp/syngular-0.2.0.tar.gz` & `tmp/syngular-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngular-0.2.0.tar", last modified: Wed Dec 27 10:34:46 2023, max compression
+gzip compressed data, was "syngular-0.2.1.tar", last modified: Sat May  4 18:30:02 2024, max compression
```

## Comparing `syngular-0.2.0.tar` & `syngular-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,27 @@
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/.github/
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/.github/workflows/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1321 2021-09-15 11:33:10.000000 syngular-0.2.0/.github/workflows/continuous_integration.yml
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       67 2021-07-14 17:26:37.000000 syngular-0.2.0/.gitignore
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    35149 2021-07-16 21:33:14.000000 syngular-0.2.0/LICENSE.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1889 2023-12-27 10:34:46.970841 syngular-0.2.0/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1141 2023-12-27 10:24:00.000000 syngular-0.2.0/README.md
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        9 2022-10-21 11:21:25.000000 syngular-0.2.0/apt.txt
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/examples/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     7291 2023-03-01 20:30:38.000000 syngular-0.2.0/examples/Examples.ipynb
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       14 2022-10-21 11:06:30.000000 syngular-0.2.0/runtime.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      203 2023-12-27 10:34:46.970841 syngular-0.2.0/setup.cfg
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1165 2023-12-27 10:34:23.000000 syngular-0.2.0/setup.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/syngular/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      317 2023-12-22 08:37:17.000000 syngular-0.2.0/syngular/__init__.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4146 2023-12-22 10:53:25.000000 syngular-0.2.0/syngular/field.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    15181 2023-12-22 10:47:07.000000 syngular-0.2.0/syngular/ideal.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     9487 2023-12-19 22:36:22.000000 syngular-0.2.0/syngular/ideal_algorithms.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      585 2021-07-16 21:33:14.000000 syngular-0.2.0/syngular/qring.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     2014 2022-11-15 18:16:23.000000 syngular-0.2.0/syngular/ring.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     2499 2023-12-22 09:51:23.000000 syngular-0.2.0/syngular/tools.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)    16923 2023-12-22 18:33:52.000000 syngular-0.2.0/syngular/variety.py
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/syngular.egg-info/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1889 2023-12-27 10:34:46.000000 syngular-0.2.0/syngular.egg-info/PKG-INFO
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      545 2023-12-27 10:34:46.000000 syngular-0.2.0/syngular.egg-info/SOURCES.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        1 2023-12-27 10:34:46.000000 syngular-0.2.0/syngular.egg-info/dependency_links.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)       30 2023-12-27 10:34:46.000000 syngular-0.2.0/syngular.egg-info/requires.txt
--rw-rw-r--   0 gdl       (1000) gdl       (1000)        9 2023-12-27 10:34:46.000000 syngular-0.2.0/syngular.egg-info/top_level.txt
-drwxrwxr-x   0 gdl       (1000) gdl       (1000)        0 2023-12-27 10:34:46.970841 syngular-0.2.0/tests/
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     4842 2023-12-22 11:37:06.000000 syngular-0.2.0/tests/test_ideal.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1009 2021-11-15 11:52:59.000000 syngular-0.2.0/tests/test_ideal_algorithms.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)      263 2021-07-16 21:33:14.000000 syngular-0.2.0/tests/test_ring.py
--rw-rw-r--   0 gdl       (1000) gdl       (1000)     1255 2021-07-16 21:33:14.000000 syngular-0.2.0/update-badges.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:30:02.662756 syngular-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-04 18:29:53.000000 syngular-0.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-04 18:30:02.662756 syngular-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-04 18:29:53.000000 syngular-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-04 18:30:02.662756 syngular-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-04 18:29:53.000000 syngular-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:30:02.662756 syngular-0.2.1/syngular/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15274 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/ideal_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/qring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-05-04 18:29:53.000000 syngular-0.2.1/syngular/variety.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:30:02.662756 syngular-0.2.1/syngular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-04 18:30:02.000000 syngular-0.2.1/syngular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 18:30:02.000000 syngular-0.2.1/syngular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 18:30:02.000000 syngular-0.2.1/syngular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 18:30:02.000000 syngular-0.2.1/syngular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 18:30:02.000000 syngular-0.2.1/syngular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 18:30:02.662756 syngular-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-04 18:29:53.000000 syngular-0.2.1/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-04 18:29:53.000000 syngular-0.2.1/tests/test_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-04 18:29:53.000000 syngular-0.2.1/tests/test_ideal_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-04 18:29:53.000000 syngular-0.2.1/tests/test_ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-05-04 18:29:53.000000 syngular-0.2.1/tests/test_variety.py
```

### Comparing `syngular-0.2.0/LICENSE.txt` & `syngular-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `syngular-0.2.0/setup.py` & `syngular-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='syngular',
-    version='v0.2.0',
+    version='v0.2.1',
     license='GNU General Public License v3.0',
     description='An Object-Oriented Python Interface to Singular',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Giuseppe De Laurentis',
     author_email='g.dl@hotmail.it',
     url='https://github.com/GDeLaurentis/syngular',
```

### Comparing `syngular-0.2.0/syngular/field.py` & `syngular-0.2.1/syngular/field.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def set(self, *args):
         """(name, characteristic, digits)"""
         self.name = args[0]
         self.characteristic = args[1]
         self.digits = args[2]
 
     def __str__(self):
-        return "({}, {}, {})".format(self.name, self.characteristic, self.digits)
+        return "('{}', {}, {})".format(self.name, self.characteristic, self.digits)
 
     def __repr__(self):
         return str(self)
 
     def __call__(self, other):
         """Cast to field."""
         if self.name == "mpc":
@@ -104,25 +104,34 @@
         if self.name == 'mpc':
             return '(complex,{},I)'.format(self.digits - 5)
         elif self.name in ['finite field', 'padic']:
             return str(self.characteristic)
         else:
             return None
 
-    @property
-    def sqrt(self):
+    def sqrt(self, val):
         if self.name == "finite field":
-            return finite_field_sqrt
+            if not isinstance(val, ModP):
+                val = self(val)
+            return finite_field_sqrt(val)
         elif self.name == "padic":
-            return padic_sqrt
+            if not isinstance(val, PAdic):
+                val = self(val)
+            return padic_sqrt(val)
         elif self.name == "mpc":
-            return mpmath.sqrt
+            return mpmath.sqrt(val)
         else:
             raise Exception(f"Field not understood: {self.field.name}")
 
+    @property
+    def j(self):
+        return self.sqrt(-1)
+
+    i = I = j
+
     def random_element(self, shape=(1, )):
         if shape == (1, ):
             if self.name == "padic":
                 p, k = self.characteristic, self.digits
                 return PAdic(random.randrange(0, p ** k - 1), p, k)
             elif self.name == "finite field":
                 p = self.characteristic
@@ -131,12 +140,37 @@
                 return mpmath.mpc(str(Q(random.randrange(-100, 101), random.randrange(1, 201))),
                                   str(Q(random.randrange(-100, 101), random.randrange(1, 201))))
             else:
                 raise NotImplementedError
         else:
             raise NotImplementedError
 
+    def epsilon(self, shape=(1, ), ):
+        if shape == (1, ):
+            if not hasattr(self, "_ε"):
+                if self.name == "padic":
+                    self._ε = self.characteristic
+                elif self.name == "finite field":
+                    raise ValueError("Finite field infinitesimal does not exist.")
+                elif self.name == "mpc":
+                    self._ε = mpmath.mpf('1e-30')
+                else:
+                    raise NotImplementedError
+            return self._ε
+        else:
+            raise NotImplementedError
+
+    @property
+    def ε(self):
+        if not hasattr(self, "_ε"):
+            self._ε = self.epsilon
+        return self._ε
+
+    @ε.setter
+    def ε(self, temp_ε):
+        self._ε = temp_ε
+
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
 
 
 field = Field()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `syngular-0.2.0/syngular/ideal.py` & `syngular-0.2.1/syngular/ideal.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,14 +336,18 @@
     def delete_cached_properties(self):
         for cached_property in self._get_cached_properties_names():
             delattr(self, cached_property)
 
     def generators_eval(self, **kwargs):
         return [eval(generator.replace("^", "**"), kwargs) for generator in self.generators]
 
+    @property
+    def is_unit_ideal(self):
+        return self == Ideal(self.ring, ('1', ))
+
 
 def reduce(poly, ideal):
     return ideal.reduce(poly)
 
 
 def monomial_to_exponents(variables, monomial):
     """Converts a monomial in the variables of a polynomial ring into a numpy.array of exponents."""
```

### Comparing `syngular-0.2.0/syngular/ideal_algorithms.py` & `syngular-0.2.1/syngular/ideal_algorithms.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,16 +118,18 @@
         else:
             raise ValueError
         string = execute_singular_command(self.singular_commands_EXTCONT2.format(**{"extended_ideal": self.extension(U, ordering),
                                                                                     "f_polys_factors": ','.join(self.extension_contraction_fpoly(U, ordering)), "r": r, "r2": r2}))
         Ideal = self.__class__
         return int(string.split("\n")[1]), Ideal(r, [entry.replace(",", "") for entry in string.split("\n")[3:]])
 
-    def primeTestDLP(self, verbose=False, timeout_fpoly=10, timeout_dim=600):
-        """Returns True if the ideal is prime, False if it is not. Raises Inconclusive if it can't decide. Assumes equidimensionality of input ideal."""
+    def primeTestDLP(self, verbose=False, timeout_fpoly=10, timeout_dim=600, iterated_degbound_computation=False):
+        """Returns True if the ideal is prime, False if it is not. Raises Inconclusive if it can't decide. Assumes equidimensionality of input ideal.
+        Experimental new feature with iterated_degbound_computation=True, may help when ideal is prime and deg-unbounded computation fails.
+        """
         import syngular
         # algorithm works over rings, if in a qring convert to the full ring.
         self.to_full_ring()
         # first step: find zero dimensional projections which are linear in the dependent variables, i.e. are a single point.
         linear_projection_indepSetIndices = []
         for i in range(len(self.indepSets)):
             if verbose:
@@ -181,24 +183,43 @@
         smallest_fpoly_factors = f_polys_factors[max_lengths.index(min(max_lengths))]
         if smallest_fpoly_factors == ['- TIMEDOUT - probably very very long ' * 80]:
             raise Inconclusive
         if verbose:
             print(f"\r smallest f poly factors: {smallest_fpoly_factors}", end="                    \n")
         # check that the dimensionality drops when adding each of these factors separately (and hence drops for <ideal, f^s>)
         syngular.TIMEOUT.set(timeout_dim)
+        self.codim  # just cache it
         for i, factor in enumerate(smallest_fpoly_factors):
             if verbose:
-                print(f"\r at factor {i}: {factor}.", end="                                    ")
+                print(f"\r at factor {i}: {factor}.", end="                                       \n")
             X = deepcopy(self)
             X.generators += [factor]
             X.delete_cached_properties()
-            # print(X)
-            # print(self.indepSet.count(0), X.indepSet.count(0))
-            if self.indepSet.count(0) >= X.indepSet.count(0):
-                return False
+
+            # Experimental - Assumes codim w/ deg bound <= true codim.
+            # Helps termiante the prime test early, IF the result is True.
+            for deg_bound in [4, 6, 8, 10, 12, 14, 16, 18] * iterated_degbound_computation:
+                syngular.DEGBOUND.set(deg_bound)
+                X.delete_cached_properties()
+                if self.codim < X.codim:
+                    if verbose:
+                        print(f"deg_bound {deg_bound} computation was conclusive.", end="\n")
+                    break
+                else:
+                    if verbose:
+                        print(f"deg_bound {deg_bound} computation was inconclusive.", end="\n")
+
+            else:  # loop completed without encountering a break
+                if verbose:
+                    print("deg_bound reset to zero. Performing full computation.", end="\n")
+                syngular.DEGBOUND.set(0)
+                # if self.indepSet.count(0) >= X.indepSet.count(0):   # deprecated, equivalent to next line.
+                if self.codim >= X.codim:
+                    return False
+        syngular.DEGBOUND.set(0)  # Reset it to zero
         return True
 
     def test_primality(self, *args, **kwargs):
         """Tests if an ideal is prime. Not to be confused with primary."""
         # eventually check assumptions and decide which test to use
         return self.primeTestDLP(*args, **kwargs)
```

### Comparing `syngular-0.2.0/syngular/ring.py` & `syngular-0.2.1/syngular/ring.py`

 * *Files identical despite different names*

### Comparing `syngular-0.2.0/syngular/tools.py` & `syngular-0.2.1/syngular/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,7 +40,11 @@
 
 class SingularException(Exception):
     pass
 
 
 class RootNotInFieldError(Exception):
     pass
+
+
+class RootPrecisionError(Exception):
+    pass
```

### Comparing `syngular-0.2.0/syngular/variety.py` & `syngular-0.2.1/syngular/variety.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,70 +5,77 @@
 import re
 import sympy
 import syngular
 
 from copy import copy, deepcopy
 from pyadic import PAdic, ModP
 
-from .tools import RootNotInFieldError
+from .tools import RootNotInFieldError, RootPrecisionError
 
 # this fixes a weird bug where sympy does not respect precision even if mpmath.mp.dps precision is set
 # (sympy seems to use mpmath as backhand)
 equation = sympy.sympify(f"x - 1.{'0' * 290}1")
 sympy.nroots(equation, n=300, maxsteps=500)
 
 
 def retry_to_find_root(max_tries=100):
     def retry_to_find_root_decorator(func):
         @functools.wraps(func)
-        def wrapper(self, field, base_point={}, directions=[], valuations=tuple(), indepSetNbr=None, seed=None, verbose=False):
+        def wrapper(self, field, base_point={}, directions=None, valuations=tuple(), indepSetNbr=None, seed=None, verbose=False):
             if base_point != {} and indepSetNbr is not None:
                 return func(self, field, base_point=base_point, directions=directions, valuations=valuations,
                             indepSetNbr=indepSetNbr, seed=seed, verbose=verbose)
             else:
                 for try_nbr in range(max_tries):
                     try:
                         res = func(self, field, base_point=base_point, directions=directions, valuations=valuations,
                                    indepSetNbr=indepSetNbr, seed=seed, verbose=verbose)
                         break
-                    except RootNotInFieldError as e:
+                    except (RootNotInFieldError, RootPrecisionError) as e:
                         if try_nbr != max_tries - 1:
                             if verbose:
-                                print("Caught RootNotInFieldError, retrying...")
+                                print(f"Caught {type(e).__name__}, retrying...")
                             if seed is not None:  # maintain pseudo-randomness, but change seed, else retring has no effect.
                                 random.seed(seed)
                                 seed += random.randint(10 ** 5, 10**6)
                             continue
                         else:
-                            raise RootNotInFieldError(f"Could not find a root in the field {field} after {max_tries} attempts. {e}")
+                            raise type(e)(f"Could not find a root in the field {field} after {max_tries} attempts. {e}")
                 return res
         return wrapper
     return retry_to_find_root_decorator
 
 
 class Variety_of_Ideal:
 
-    @retry_to_find_root(max_tries=10)
-    def point_on_variety(self, field, base_point={}, directions=[], valuations=tuple(), indepSetNbr=None, seed=None, verbose=False):
+    @retry_to_find_root(max_tries=100)
+    def point_on_variety(self, field, base_point={}, directions=None, valuations=tuple(), indepSetNbr=None, seed=None, verbose=False):
         """Generate a representative point on or close to the variety associated to this ideal.
         The point is 'valuations' away from the exact variety, in the directions specified by 'directions'.
         If 'directions' are not provided, pick the first n=codim simplest generators from 'self'.
         If the ideal is not prime, an irreducible branch will be picked at random."""
 
         from .ideal import Ideal
         from .qring import QuotientRing
 
         assert all([valuation > 0 for valuation in valuations])
         self = deepcopy(self)   # don't modify self within this function
 
         random.seed(seed)
 
         # handle directions, i.e. the generators of the sub-ideal of maximal codimension
-        if directions == []:
-            directions = sorted(self.generators, key=lambda x: len(x))[:self.codim]
+        if directions is None or directions == []:
+            directions = []
+            if verbose:
+                print("Directions not provided, obtaining them from ideal generators.")
+            for poly in sorted(self.generators, key=lambda x: len(x)):
+                if Ideal(self.ring, directions + [poly, ]).codim > Ideal(self.ring, directions).codim:
+                    directions += [poly, ]
+                if len(directions) == self.codim:
+                    break
             assert Ideal(self.ring, directions).codim == self.codim
         # extra directions in qring
         if isinstance(self.ring, QuotientRing):
             directions += self.ring.ideal.generators
 
         # handle valuations - if valuations == tuple() return a point exactly on the variety
         if field.name == "padic":
@@ -121,18 +128,19 @@
             if verbose:
                 print(f"\nAt iteration {iteration}")
                 # print(f"base point {base_point}")
                 # print(repr(oSemiNumericalIdeal), oSemiNumericalIdeal.primary_decomposition, oSemiNumericalIdeal.groebner_basis, len(oSemiNumericalIdeal.groebner_basis))
 
             syngular.DEGBOUND.set(0)
 
-            if prime is not None:
-                assert oSemiNumericalIdeal.dim == 0
-            else:
-                assert oSemiNumericalIdeal.dim in [0, -1]
+            if prime is None and oSemiNumericalIdeal.dim == -1:  # this is the ideal generated by '1'
+                raise RootPrecisionError
+            if not oSemiNumericalIdeal.dim == 0:
+                raise Exception("The dimension of the semi-numerical ideal was not zero.")
+
             root_dicts = lex_groebner_solve(oSemiNumericalIdeal.groebner_basis, prime=prime)
             check_solutions(oSemiNumericalIdeal.groebner_basis, root_dicts, prime=prime)
 
             try:
                 root_dict = root_dicts[0]
             except IndexError:
                 if not field.is_algebraically_closed:
```

### Comparing `syngular-0.2.0/tests/test_ideal.py` & `syngular-0.2.1/tests/test_ideal.py`

 * *Files identical despite different names*

### Comparing `syngular-0.2.0/tests/test_ideal_algorithms.py` & `syngular-0.2.1/tests/test_ideal_algorithms.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     with pytest.raises(ValueError):
         I.extension_contraction(U, ordering="Dp") == (1, J)
 
 
 def test_primeTestDLP():
     I = Ideal(Ring('0', ('x1', 'x2'), 'dp'), ['x1*x2'])
     J = Ideal(Ring('0', ('x1', 'x2'), 'dp'), ['x2'])
-    assert I.primeTestDLP(verbose=True) is False
-    assert J.primeTestDLP(verbose=True) is True
+    assert I.test_primality(verbose=True) is False
+    assert I.test_primality(verbose=True, iterated_degbound_computation=True) is False
+    assert J.test_primality(verbose=True) is True
+    assert J.test_primality(verbose=True, iterated_degbound_computation=True) is True
 
 
 def test_primeTestDLP_inconclusive():
     I = Ideal(Ring('0', ('x1', 'x2'), 'dp'), ['x1^2'])
     with pytest.raises(Inconclusive):
-        assert I.primeTestDLP(verbose=True) is False
+        assert I.test_primality(verbose=True) is False
+        assert I.test_primality(verbose=True, iterated_degbound_computation=True) is False
```

