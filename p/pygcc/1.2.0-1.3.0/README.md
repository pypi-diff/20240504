# Comparing `tmp/pygcc-1.2.0.tar.gz` & `tmp/pygcc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygcc-1.2.0.tar", max compression
+gzip compressed data, was "pygcc-1.3.0.tar", max compression
```

## Comparing `pygcc-1.2.0.tar` & `pygcc-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35792 2022-01-20 19:48:58.516069 pygcc-1.2.0/LICENSE
--rw-r--r--   0        0        0     1433 2023-09-10 17:02:29.714646 pygcc-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3628 2022-03-10 22:56:30.225111 pygcc-1.2.0/README.md
--rw-r--r--   0        0        0      481 2022-05-13 19:26:30.592131 pygcc-1.2.0/src/pygcc/__init__.py
--rw-r--r--   0        0        0     1793 2021-06-23 20:36:07.331002 pygcc-1.2.0/src/pygcc/clay_elements.dat
--rw-r--r--   0        0        0    61512 2022-04-26 07:02:24.850743 pygcc-1.2.0/src/pygcc/clay_thermocalc.py
--rw-r--r--   0        0        0    38273 2021-09-21 05:00:37.795582 pygcc-1.2.0/src/pygcc/default_db/berman.dat
--rw-r--r--   0        0        0   650624 2021-06-14 18:23:45.896568 pygcc-1.2.0/src/pygcc/default_db/data0.dat
--rw-r--r--   0        0        0   416877 2023-06-12 20:52:36.333777 pygcc-1.2.0/src/pygcc/default_db/speq21.dat
--rw-r--r--   0        0        0   417082 2023-06-12 20:53:05.982471 pygcc-1.2.0/src/pygcc/default_db/speq21_dimer.dat
--rw-r--r--   0        0        0   417553 2023-06-12 20:52:25.409478 pygcc-1.2.0/src/pygcc/default_db/speq23.dat
--rw-r--r--   0        0        0   417758 2023-06-12 20:45:47.228862 pygcc-1.2.0/src/pygcc/default_db/speq23_dimer.dat
--rw-r--r--   0        0        0   144262 2022-04-02 03:44:55.192486 pygcc-1.2.0/src/pygcc/default_db/supcrtbl.dat
--rw-r--r--   0        0        0   622490 2023-06-13 14:48:23.552105 pygcc-1.2.0/src/pygcc/default_db/thermo.2021.dat
--rw-r--r--   0        0        0  1692441 2021-05-04 22:59:52.541244 pygcc-1.2.0/src/pygcc/default_db/thermo.com.dat
--rw-r--r--   0        0        0  1717648 2023-08-19 03:48:55.901134 pygcc-1.2.0/src/pygcc/default_db/thermo.com.tdat
--rw-r--r--   0        0        0   154654 2022-03-21 16:01:06.000000 pygcc-1.2.0/src/pygcc/default_db/thermo_cemdata_mar.tdat
--rw-r--r--   0        0        0  1719612 2023-08-19 03:48:39.655785 pygcc-1.2.0/src/pygcc/default_db/thermo_latest.tdat
--rw-r--r--   0        0        0    73151 2022-11-22 05:19:27.977208 pygcc-1.2.0/src/pygcc/ion_size.txt
--rw-r--r--   0        0        0   193151 2021-07-23 18:15:49.972438 pygcc-1.2.0/src/pygcc/PeriodicTableJSON.json
--rw-r--r--   0        0        0   286893 2023-09-10 03:05:54.240064 pygcc-1.2.0/src/pygcc/pygcc_utils.py
--rw-r--r--   0        0        0    70267 2023-09-10 18:53:08.405131 pygcc-1.2.0/src/pygcc/read_db.py
--rw-r--r--   0        0        0    60171 2022-11-15 02:24:37.257067 pygcc-1.2.0/src/pygcc/solid_solution.py
--rw-r--r--   0        0        0    52859 2022-11-15 02:23:54.114715 pygcc-1.2.0/src/pygcc/species_eos.py
--rw-r--r--   0        0        0   142259 2022-09-19 16:54:07.029818 pygcc-1.2.0/src/pygcc/water_eos.py
--rw-r--r--   0        0        0     4601 2023-09-10 18:54:27.174498 pygcc-1.2.0/setup.py
--rw-r--r--   0        0        0     4979 2023-09-10 18:54:27.175495 pygcc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35792 2022-01-20 19:48:58.516069 pygcc-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1433 2024-05-04 00:21:58.600038 pygcc-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3628 2022-03-10 22:56:30.225111 pygcc-1.3.0/README.md
+-rw-r--r--   0        0        0      411 2024-05-03 23:45:03.923556 pygcc-1.3.0/src/pygcc/__init__.py
+-rw-r--r--   0        0        0     1793 2021-06-23 20:36:07.331002 pygcc-1.3.0/src/pygcc/clay_elements.dat
+-rw-r--r--   0        0        0    61512 2022-04-26 07:02:24.850743 pygcc-1.3.0/src/pygcc/clay_thermocalc.py
+-rw-r--r--   0        0        0    38273 2021-09-21 05:00:37.795582 pygcc-1.3.0/src/pygcc/default_db/berman.dat
+-rw-r--r--   0        0        0   650624 2021-06-14 18:23:45.896568 pygcc-1.3.0/src/pygcc/default_db/data0.dat
+-rw-r--r--   0        0        0   416877 2023-06-12 20:52:36.333777 pygcc-1.3.0/src/pygcc/default_db/speq21.dat
+-rw-r--r--   0        0        0   417082 2023-06-12 20:53:05.982471 pygcc-1.3.0/src/pygcc/default_db/speq21_dimer.dat
+-rw-r--r--   0        0        0   417553 2023-06-12 20:52:25.409478 pygcc-1.3.0/src/pygcc/default_db/speq23.dat
+-rw-r--r--   0        0        0   417758 2023-06-12 20:45:47.228862 pygcc-1.3.0/src/pygcc/default_db/speq23_dimer.dat
+-rw-r--r--   0        0        0   144262 2022-04-02 03:44:55.192486 pygcc-1.3.0/src/pygcc/default_db/supcrtbl.dat
+-rw-r--r--   0        0        0   622490 2023-06-13 14:48:23.552105 pygcc-1.3.0/src/pygcc/default_db/thermo.2021.dat
+-rw-r--r--   0        0        0  1692441 2021-05-04 22:59:52.541244 pygcc-1.3.0/src/pygcc/default_db/thermo.com.dat
+-rw-r--r--   0        0        0  1717648 2023-08-19 03:48:55.901134 pygcc-1.3.0/src/pygcc/default_db/thermo.com.tdat
+-rw-r--r--   0        0        0   154654 2022-03-21 16:01:06.000000 pygcc-1.3.0/src/pygcc/default_db/thermo_cemdata_mar.tdat
+-rw-r--r--   0        0        0  1719612 2023-08-19 03:48:39.655785 pygcc-1.3.0/src/pygcc/default_db/thermo_latest.tdat
+-rw-r--r--   0        0        0    73151 2022-11-22 05:19:27.977208 pygcc-1.3.0/src/pygcc/ion_size.txt
+-rw-r--r--   0        0        0   193151 2021-07-23 18:15:49.972438 pygcc-1.3.0/src/pygcc/PeriodicTableJSON.json
+-rw-r--r--   0        0        0   286957 2024-05-03 23:45:47.813247 pygcc-1.3.0/src/pygcc/pygcc_utils.py
+-rw-r--r--   0        0        0    70267 2023-09-10 18:53:08.405131 pygcc-1.3.0/src/pygcc/read_db.py
+-rw-r--r--   0        0        0    60171 2022-11-15 02:24:37.257067 pygcc-1.3.0/src/pygcc/solid_solution.py
+-rw-r--r--   0        0        0    52859 2022-11-15 02:23:54.114715 pygcc-1.3.0/src/pygcc/species_eos.py
+-rw-r--r--   0        0        0   165148 2024-05-03 23:44:30.740260 pygcc-1.3.0/src/pygcc/water_eos.py
+-rw-r--r--   0        0        0     4601 2024-05-04 01:58:06.747245 pygcc-1.3.0/setup.py
+-rw-r--r--   0        0        0     4979 2024-05-04 01:58:06.748243 pygcc-1.3.0/PKG-INFO
```

### Comparing `pygcc-1.2.0/LICENSE` & `pygcc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/pyproject.toml` & `pygcc-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b74 6f6f 6c2e 706f 6574 7279 5d0d 0a6e  [tool.poetry]..n
 00000010: 616d 6520 3d20 2270 7967 6363 220d 0a76  ame = "pygcc"..v
-00000020: 6572 7369 6f6e 203d 2022 312e 322e 3022  ersion = "1.2.0"
+00000020: 6572 7369 6f6e 203d 2022 312e 332e 3022  ersion = "1.3.0"
 00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000040: 2241 2074 6f6f 6c20 666f 7220 7468 6572  "A tool for ther
 00000050: 6d6f 6479 6e61 6d69 6320 6361 6c63 756c  modynamic calcul
 00000060: 6174 696f 6e73 2061 6e64 2067 656f 6368  ations and geoch
 00000070: 656d 6963 616c 2064 6174 6162 6173 6520  emical database 
 00000080: 6765 6e65 7261 7469 6f6e 220d 0a61 7574  generation"..aut
 00000090: 686f 7273 203d 205b 2241 6465 6461 706f  hors = ["Adedapo
```

### Comparing `pygcc-1.2.0/README.md` & `pygcc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/clay_elements.dat` & `pygcc-1.3.0/src/pygcc/clay_elements.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/clay_thermocalc.py` & `pygcc-1.3.0/src/pygcc/clay_thermocalc.py`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/berman.dat` & `pygcc-1.3.0/src/pygcc/default_db/berman.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/data0.dat` & `pygcc-1.3.0/src/pygcc/default_db/data0.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/speq21.dat` & `pygcc-1.3.0/src/pygcc/default_db/speq21.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/speq21_dimer.dat` & `pygcc-1.3.0/src/pygcc/default_db/speq21_dimer.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/speq23.dat` & `pygcc-1.3.0/src/pygcc/default_db/speq23.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/speq23_dimer.dat` & `pygcc-1.3.0/src/pygcc/default_db/speq23_dimer.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/supcrtbl.dat` & `pygcc-1.3.0/src/pygcc/default_db/supcrtbl.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/thermo.2021.dat` & `pygcc-1.3.0/src/pygcc/default_db/thermo.2021.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/thermo.com.dat` & `pygcc-1.3.0/src/pygcc/default_db/thermo.com.dat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/thermo.com.tdat` & `pygcc-1.3.0/src/pygcc/default_db/thermo.com.tdat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/thermo_cemdata_mar.tdat` & `pygcc-1.3.0/src/pygcc/default_db/thermo_cemdata_mar.tdat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/default_db/thermo_latest.tdat` & `pygcc-1.3.0/src/pygcc/default_db/thermo_latest.tdat`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/ion_size.txt` & `pygcc-1.3.0/src/pygcc/ion_size.txt`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/PeriodicTableJSON.json` & `pygcc-1.3.0/src/pygcc/PeriodicTableJSON.json`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/pygcc_utils.py` & `pygcc-1.3.0/src/pygcc/pygcc_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 from .read_db import db_reader
 from .water_eos import iapws95, ZhangDuan, water_dielec, readIAPWS95data, convert_temperature
+from .water_eos import  Driesner_NaCl, concentration_converter
 from .species_eos import heatcap, supcrtaq
 from .solid_solution import solidsolution_thermo
 from .clay_thermocalc import calclogKclays
 import warnings
 import re
 import os
 import json
```

### Comparing `pygcc-1.2.0/src/pygcc/read_db.py` & `pygcc-1.3.0/src/pygcc/read_db.py`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/solid_solution.py` & `pygcc-1.3.0/src/pygcc/solid_solution.py`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/species_eos.py` & `pygcc-1.3.0/src/pygcc/species_eos.py`

 * *Files identical despite different names*

### Comparing `pygcc-1.2.0/src/pygcc/water_eos.py` & `pygcc-1.3.0/src/pygcc/water_eos.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 Functions implemented here include water equation of state and dielectric properties
 """
 
 import numpy as np, math
 from scipy.optimize import root_scalar, fsolve, brentq
 from scipy.linalg import lu_factor, lu_solve
+from numpy import exp, log10, log
 
 eps = 2.220446049250313e-16
 J_to_cal = 4.184
 np.random.seed(4321)
 
 def convert_temperature(T, Out_Unit = 'C'):
     """
@@ -3022,7 +3023,449 @@
         # convert Bdhh from kJ kg^1/2 mol^-3/2 Angstrom^-1 to cal kg^1/2 mol^-3/2 cm^-1  10^-9
         Bdhh = Bdhh*1000/J_to_cal*0.10
         # E, rhohat, Ah, Bh, bdot, Adhh, Adhv, Bdhh, Bdhv, dEdP_T, dEdT_P, dEdT_r, dEdr_T, drdP_T
 
         return E, rhohat, Ah, Bh, bdot, Adhh, Adhv, Bdhh, Bdhv, dEdP_T, dEdT_P
 
 
+def concentration_converter(val = 1.0, In_Unit='x_wt', Out_Unit='x_wt'):
+    """This function converts concentration between several units like wt%, mole fraction, molality and volume
+    Values must be in fraction except it is molality
+
+    Parameters
+    ----------
+    val : float
+        Values to convert
+    In_Unit : String
+        unit of input concentration
+    Out_Unit : String
+        expected output concentration
+
+    Returns
+    -------
+    Out : float
+        Converted values
+    """
+    #Accepted units for input and output are:
+    phase_markers = ['x_wt', 'x_mol', 'x_vol', 'x_molal', 'x_mol_kgsol']
+
+    MwH2O = 18.01528
+    MwNaCl = 58.44280
+    rhoH2O = 1
+    rhoNaCl = 2.16
+    if not (In_Unit in phase_markers and Out_Unit in phase_markers):
+        return None
+
+    if In_Unit == Out_Unit or val == 0.:
+        return val
+
+    if In_Unit != 'x_molal' and In_Unit != 'x_mol_kgsol' and val > 1.:
+        print('x_convert func values above 1 (>100% NaCl)')
+        return None
+    if In_Unit == "x_wt":
+        if Out_Unit == 'x_mol':
+            return val/MwNaCl/(val/MwNaCl+(1.-val)/MwH2O)
+        elif Out_Unit == 'x_vol':
+            return val/rhoNaCl/(val/rhoNaCl+(1.-val)/rhoH2O)
+        else:
+            return val*1000./MwNaCl/(1.-val)
+    elif In_Unit == 'x_mol':
+        if Out_Unit == 'x_wt':
+            return val*MwNaCl/(val*MwNaCl+(1.-val)*MwH2O)
+        elif Out_Unit == 'x_vol':
+            return MwNaCl*val/rhoNaCl/(MwNaCl*val/rhoNaCl+(1.-val)*MwH2O/rhoH2O)
+        else:
+            x_tmp = val*MwNaCl/(val*MwNaCl+(1.-val)*MwH2O)
+            return 1000.*x_tmp/MwNaCl/(1.-x_tmp)
+    elif In_Unit == 'x_vol':
+        if Out_Unit == 'x_wt':
+            return val*rhoNaCl/(val*rhoNaCl+(1.-val)*rhoH2O)
+        elif Out_Unit == 'x_mol':
+            return val*rhoNaCl/MwNaCl/(val*rhoNaCl/MwNaCl+(1.-val)*(rhoH2O/MwH2O))
+        else:
+            x_tmp = val*rhoNaCl/(val*rhoNaCl+(1.-val)*rhoH2O)
+            return 1000*x_tmp/MwNaCl/(1.-x_tmp)
+    elif In_Unit == 'x_mol_kgsol':
+        if Out_Unit == 'x_mol':
+            x_tmp = val*MwNaCl/(1000)
+            return x_tmp/MwNaCl/(x_tmp/MwNaCl+(1.-x_tmp)/MwH2O)
+    else:
+        if Out_Unit == 'x_wt':
+            return val*MwNaCl/(1000.+val*MwNaCl)
+        elif Out_Unit == 'x_mol':
+            x_tmp = val*MwNaCl/(1000.+val*MwNaCl)
+            return x_tmp/MwNaCl/(x_tmp/MwNaCl+(1.-x_tmp)/MwH2O)
+        else:
+            x_tmp = val*MwNaCl/(1000.+val*MwNaCl)
+            return x_tmp/rhoNaCl/(x_tmp/rhoNaCl+(1.-x_tmp)*rhoH2O)
+
+
+
+class Driesner_NaCl:
+    """
+    Implementation of Driesner and Heinrich PTx Formulation for H2O-NaCl system
+
+    Parameters
+    ----------
+        T : float
+            Temperature [°C]  \n
+        P : float
+            Pressure [bar]  \n
+        xNaCl : float
+            mole fraction of NaCl in H2O [-]  \n
+
+    Returns
+    ----------
+        The calculated instance has the following potential properties:  \n
+        PVLH : float
+            Pressure of vapor + liquid + halite coexistence [bar]  \n
+        Pcrit : float
+            Critical pressure (of a H2O–NaCl mixture) [bar]  \n
+        Xcrit : float
+            Critical Composition  [-]  \n
+        xL_NaCl  : float
+            Composition of halite-saturated liquid (halite liquidus) Hypothetical [-]  \n
+        xV_NaCl  : float
+            Composition of halite-saturated vapor [-] \n
+        xVL_Liq  : float
+            Composition of liquid at vapor + liquid coexistence [-] \n
+        xVL_Vap  : float
+            Composition of vapor at vapor+liquid coexistence [-]  \n
+        rho  : float
+            Liquid NaCl density [kg/m3]  \n
+        vm  : float
+            molar volume [mol/m3]  \n
+        TstarH  : float
+            Scaled temperature for enthalpy correlation [°C]  \n
+        H  : float
+            Specific enthalpy of an H2O–NaCl solution [J/kg]  \n
+        Cp  : float
+            Isobaric heat capacity [J/kg/K]  \n
+        mu  : float
+            viscosity [Pa-s]  \n
+            
+    Usage:
+    ----------
+        The general usage of Driesner_NaCl is as follows:  \n
+        (1) For water-NaCl properties at any Temperature and Pressure:  \n
+            water_salt = Driesner_NaCl(T = T, P = P),   \n
+            where T is temperature in celsius and P is pressure in bar
+    Examples
+    --------
+    >>> water_salt = Driesner_NaCl(T = 400., P = 150)
+    >>> water_salt.PVLH, water_salt.xL_NaCl, water_salt.xV_NaCl, water_salt.xVL_Liq, water_salt.xVL_Vap, water_salt.Xcrit
+        176.12604181993797,
+         0.21548565081529097,
+         1.1606891909548725e-05,
+         0.27785803505887324,
+         1.1606891909548725e-05,
+         0.006832050956381021
+
+    >>> water_salt = Driesner_NaCl(T = 400., P = 150, xNaCl = 0.00919)
+    >>> water_salt.PVLH, water_salt.xL_NaCl, water_salt.xV_NaCl, water_salt.xVL_Liq, water_salt.xVL_Vap, water_salt.rho, water_salt.vm, water_salt.H, water_salt.mu, water_salt.Cp
+        (176.12604181993797,
+         0.21548565081529097,
+         1.1606891909548725e-05,
+         0.27785803505887324,
+         1.1606891909548725e-05,
+         0.06932873574838519,
+         265.2138005082347,
+         2934.6231778877977,
+         2.4596312351131325e-05,
+         4394.068874696437)
+        
+    References
+    ----------
+        (1) Driesner, T, and Heinrich, C. A. (2007). The system H2O–NaCl. Part I: Correlation formulae for phase relations in 
+            temperature–pressure–composition space from 0 to 1000 C, 0 to 5000 bar, and 0 to 1 XNaCl. Geochimica et Cosmochimica Acta. 71(20), 4880-4901.
+            https://doi.org/10.1016/j.gca.2006.01.033
+        (2) Driesner, T. (2007). "The system H2O-NaCl. II. Correlations for molar volume, enthalpy, and isobaric heat capacity from 0 to 1000 °C, 1 to 5000 bar,
+        #     and 0 to 1 X-NaCl." Geochimica et Cosmochimica Acta 71(20): 4902-4919.
+
+    """
+
+    kwargs = {"T": None,
+              "P": None,
+              "xNaCl": None
+              }
+    def __init__(self, **kwargs):
+        self.kwargs = Driesner_NaCl.kwargs.copy()
+        self.__calc__(**kwargs)
+
+    def __calc__(self, **kwargs):
+        self.kwargs.update(kwargs)
+        """initialization """
+        self.TC = self.kwargs["T"]
+        self.P = self.kwargs["P"]
+        self.xNaCl = self.kwargs["xNaCl"]
+        self.Pc = 220.54915  #  220.54915  # bars
+        self.Tc = 373.976  # 373.946 # C
+
+        """Check if inputs are enough to define state"""
+        if self.TC and self.P is None and self.xNaCl is None:
+            self.mode = "T"
+        elif self.TC and self.P and self.xNaCl is None:
+            self.mode = "T_P"
+        else:
+            self.mode = "T_P_x"
+            
+        if self.mode == "T":
+            Driesner_calc = self.Driesner_NaCl(self.TC, self.Pc)
+            self.PVLH, self.Pcrit, self.Xcrit = Driesner_calc['PVLH'], Driesner_calc['Pcrt'], Driesner_calc['Xcrt']
+        elif self.mode == "T_P" or self.mode == "T_P_x":
+            if self.mode == "T_P_x":
+                Driesner_calc = self.Driesner_NaClII(self.TC, self.P, self.xNaCl)
+                self.vm, self.rho, self.TstarH = Driesner_calc['vm'], Driesner_calc['rho'], Driesner_calc['Tref']#, Driesner_calc['q2']
+                Driesner_calc = self.enthalpy_mu_heatcap(self.TC, self.P, self.xNaCl)
+                self.H, self.mu, self.Cp = Driesner_calc[0], Driesner_calc[1], Driesner_calc[-1]
+            Driesner_calc = self.Driesner_NaCl(self.TC, self.P)
+            self.PVLH, self.xL_NaCl, self.xV_NaCl = Driesner_calc['PVLH'], Driesner_calc['xL_NaCl'], Driesner_calc['xV_NaCl']
+            self.xVL_Liq, self.xVL_Vap = Driesner_calc['xVL_Liq'], Driesner_calc['xVL_Vap']
+            self.Pcrit, self.Xcrit = Driesner_calc['Pcrt'], Driesner_calc['Xcrt']
+    
+    def Driesner_NaCl(self, T, P):
+        # (Driesner and Heinrich, 2007).
+        Ttriple_NaCl = 800.7 # C
+        Ptriple_NaCl = 5e-4  # bar
+        alpha = 2.4726e-2
+        bsubl = 1.18061e4
+        bboil = 0.941812e4
+    
+        # Eq. (1): NaCl melting curve - melting pressure
+        Thm_func = lambda P: (P - Ptriple_NaCl)*alpha + Ttriple_NaCl
+    
+        # Eq. (2): NaCl sublimation and boiling curve - vapor pressure
+        bfunc = lambda T:  np.where(T < Ttriple_NaCl, bsubl,  bboil)
+        PNaCl_func = lambda T, b: 10**(log10(Ptriple_NaCl) + b*((Ttriple_NaCl + 273.15)**-1 - (T + 273.15)**-1))
+    
+    
+        # Electronic Annex EA-2: The critical curve, Eqs. (5b,c, 7a,b).
+        # NBS/NRC-84 or IAPWS-84
+        Pc = 220.54915  #  220.54915  # bars
+        Tc = 373.976  # 373.946 # C
+        # IAPWS-95
+        # Pc = 220.54915  # bars
+        # Tc = 373.946 # C
+        cn = np.array([-2.36, 1.28534e-1, -2.3707e-2, 3.20089e-3, -1.38917e-4, 1.02789e-7,
+                       -4.8376e-11, 2.36, -1.31417e-2, 2.98491e-3, -1.30114e-4, 0, 0, -4.88336e-4])
+        di = np.array([8.00000e-05, 1.00000e-05, -1.37125e-07, 9.46822e-10, -3.50549e-12,
+                       6.57369e-15, -4.89423e-18, 7.77761e-2, 2.7042e-4, -4.244821e-7, 2.580872e-10])
+        cnA = np.array([1, 1.5, 2, 2.5, 3, 4, 5, 1, 2, 2.5, 3, 12, 13, 14])
+        Pfunc_below_Tcrt = lambda x: Pc + np.sum(cn[:7]*(Tc - x)**cnA[:7])
+        Pfunc_above_Tcrt = lambda x: Pc + np.sum(cn[7:11]*(x - Tc)**cnA[7:11])
+        Pfunc_above_500 = lambda x: np.sum(cn[11:]*(x - 500)**(cnA[11:] - 12))
+        cn[11] = Pfunc_above_Tcrt(500)
+        cn[12] = derivative(Pfunc_above_Tcrt, 500, h = 0.0001)
+        #cn[12] = Pfunc_above_Tcrt(500)
+        Xfunc_below_600 = lambda x: np.sum(di[:7]*(x - Tc)**np.arange(8)[1:])
+        Xfunc_above_600 = lambda x: np.sum(di[7:]*(x - 600)**(np.arange(7, len(di)) - 7))
+        Pcrt_func = lambda x: Pfunc_below_Tcrt(x) if (x < Tc) else Pfunc_above_500(x) if (x > 500) else Pfunc_above_Tcrt(x)
+        Xcrt_func = lambda x: 0 if x < Tc else Xfunc_below_600(x) if x < 600 else Xfunc_above_600(x)
+    
+    
+        # Electronic Annex EA-3: The halite liquidus - L + H , Eq. (8),
+        # for isobars from 500 to 5000 bar in 500 bar intervals, and from 10 C to the melting temperature of NaCl.
+        eifunc = lambda P: [0.0989944 + 3.30796e-6*P - 4.71759e-10*P**2,
+                             0.00947257 - 8.66460e-6*P + 1.69417e-9*P**2,
+                             0.610863 - 1.51716e-5*P + 1.19290e-8*P**2,
+                             -1.64994 + 2.03441e-4*P - 6.46015e-8*P**2,
+                             3.36474 - 1.54023e-4*P + 8.17048e-8*P**2]
+        ei_func = lambda P: np.array(eifunc(P) + [1.0 - eifunc(P)[0] - eifunc(P)[1] - \
+                                                  eifunc(P)[2] - eifunc(P)[3] - eifunc(P)[4]])
+        
+        xL_NaClSat_func = lambda T, P: np.sum(ei_func(P)*(T/Thm_func(P))**np.arange(len(ei_func(P)))) \
+            if np.sum(ei_func(P)*(T/Thm_func(P))**np.arange(len(ei_func(P)))) <= 1 else 1
+    
+    
+        # Electronic Annex EA-4: Halite saturated vapor composition - V + H coexistence, Eq. (9),
+        # for isobars from 50 to 350 bar in 50 bar intervals.
+        k = [-0.235694, -0.188838, 0.004, 0.0552466, 0.66918, 396.848, 45.0, -3.2719e-7, 141.699,
+             -0.292631, -0.00139991, 1.95965e-6, -7.3653e-10, 0.904411, 0.000769766, -1.18658e-6]
+        j_func = lambda T: np.array([k[0] + k[1]*exp(-k[2]*T),
+                                     k[4] + (k[3] - k[4])/(1 + exp((T - k[5])/k[6])) + k[7]*(T + k[8])**2,
+                                     k[9] + k[10]*T + k[11]*T**2 + k[12]*T**3,
+                                     k[13] + k[14]*T + k[15]*T**2])
+        P_bar_func = lambda T, P: (P - PNaCl_func(T, bfunc(T)))/(Pcrt_func(T) - PNaCl_func(T, bfunc(T)))
+        logKbar_func = lambda T, P: (1 + j_func(T)[0]*(1 - P_bar_func(T, P))**j_func(T)[1] +  \
+                                     j_func(T)[2]*(1 - P_bar_func(T, P)) + j_func(T)[3]*(1 - P_bar_func(T, P))**2 - \
+                                         (1 + j_func(T)[0] + j_func(T)[2] + j_func(T)[3])*(1 - P_bar_func(T, P))**3)
+        
+        logKprime_func = lambda T, P: (log10(xL_NaClSat_func(T, PNaCl_func(T, bfunc(T)))) + \
+                                       logKbar_func(T, P)*(log10(PNaCl_func(T, bfunc(T))/Pcrt_func(T)) - \
+                                                           log10(xL_NaClSat_func(T, PNaCl_func(T, bfunc(T)))) ) )
+        
+        logKprime_func = lambda T, P: (log10(xL_NaClSat_func(T, PNaCl_func(T, bfunc(T)) )) + \
+                                       logKbar_func(T, P)*(log10(PNaCl_func(T, bfunc(T))/Pcrt_func(T)) - \
+                                                           log10(xL_NaClSat_func(T, PNaCl_func(T, bfunc(T)) )) ) )
+        
+        xV_NaClSat_func = lambda T, P: xL_NaClSat_func(T, P)/10**(logKprime_func(T, P) - log10(PNaCl_func(T, bfunc(T))/P ))
+        
+        
+        # Electronic Annex EA-5: The V+L+H coexistence surface, Eq. (10) combined with Eqs. (8, 9).
+        f = [4.64e-3, 5.0e-7, 1.69078e1, -2.69148e2, 7.63204e3, -4.95636e4, 2.33119e5, -5.13556e5, 5.49708e5, -2.84628e5, 0]
+        f[10] = Ptriple_NaCl - (f[0] + f[1] + f[2] + f[3] + f[4] + f[5] + f[6] + f[7] + f[8] + f[9])
+        PVLH_func = lambda T: np.sum(f*(T / Ttriple_NaCl)**np.arange(len(f)))
+    
+    
+        # Electronic Annex EA-5: Isotherms of the V+L coexistence surface, Eqs. (11, 12-17).
+        # the pressure limit ranges from pressure at V+L+H coexistence (Eq. (10)), and at the boiling pressure of
+        # water (if the temperature is smaller than the critical temperature of water) or at the critical pressure
+        # (if the temperature is higher that the critical temperature of water).
+        
+        h = [0, 1.68486e-3, 2.19379e-4, 4.3858e2, 1.84508e1, -5.6765e-10,
+             6.73704e-6, 1.44951e-7, 3.84904e2, 7.07477e0, 6.06896e-5, 7.62859e-3]
+        g0var_func = lambda T, P: [PVLH_func(T) if T < Ttriple_NaCl else PNaCl_func(T, bfunc(T)),
+                                   xL_NaClSat_func(T, P) if T < Ttriple_NaCl else 1,
+                                   iapws95(T = T).P if T < Tc else Pc]
+        g_func = lambda T, P: np.array([0,
+                                        h[2] + ((h[1] - h[2])/(1 + np.exp((T - h[3])/h[4]))) + h[5]*T**2,
+                                        h[7] + ((h[6] - h[7])/(1 + np.exp((T - h[8])/h[9]))) + h[10]*np.exp(-h[11]*T)])
+        
+        g0_func = lambda T, P, *x: ((x[1] + g_func(T, P)[1] * (x[0] - x[2]) + \
+                                     g_func(T, P)[2] * ((Pcrt_func(T) - x[2])**2 - \
+                                                        (Pcrt_func(T) - x[0])**2)) / \
+                                    ((Pcrt_func(T) - x[0])**0.5 - (Pcrt_func(T) - x[2])**0.5)) \
+            if T <= Tc else ((x[1] - Xcrt_func(T) - g_func(T, P)[1] * (Pcrt_func(T) - x[0]) - \
+                              g_func(T, P)[2] * (Pcrt_func(T) - x[0])**2) / (Pcrt_func(T) - x[0])**0.5)
+        
+        P_Pcrt_func =  lambda T, P:  Pcrt_func(T) if Pcrt_func(T) < P else P
+        
+        
+        xVL_LiqNaCl_func = lambda T, P:  (g0_func(T, P, *g0var_func(T, P))*((Pcrt_func(T) - P_Pcrt_func(T, P))**0.5 - \
+                                                                            (Pcrt_func(T) - g0var_func(T, P)[2])**0.5) - \
+            g_func(T, P)[1]*((Pcrt_func(T) - g0var_func(T, P)[2]) - (Pcrt_func(T) - P_Pcrt_func(T, P))) - \
+                g_func(T, P)[2]*((Pcrt_func(T) - g0var_func(T, P)[2])**2 - (Pcrt_func(T) - P_Pcrt_func(T, P)) ** 2) ) \
+            if T <= Tc else (Xcrt_func(T) + g0_func(T, P, *g0var_func(T, P))*(Pcrt_func(T) - P_Pcrt_func(T, P))**0.5 + \
+                                                             g_func(T, P)[1]*(Pcrt_func(T) - P_Pcrt_func(T, P)) + \
+                                                                 g_func(T, P)[2]*(Pcrt_func(T) - P_Pcrt_func(T, P))**2 )
+        
+        
+        xVL_VapNaCl_func = lambda T, P: (xVL_LiqNaCl_func(T, P)/10**(logKprime_func(T, P) - \
+                                                                     log10(PNaCl_func(T, bfunc(T))/P ))) \
+            if P > PVLH_func(T) else (xL_NaClSat_func(T, P)/10**(logKprime_func(T, P) - \
+                                                                 log10(PNaCl_func(T, bfunc(T))/P )))
+        
+        res = {'PVLH': PVLH_func(T),
+               'Pcrt': Pcrt_func(T),
+               'Xcrt': Xcrt_func(T),
+               'xL_NaCl': xL_NaClSat_func(T, P), 
+               'xV_NaCl': xV_NaClSat_func(T, P), 
+               'xVL_Liq': xVL_LiqNaCl_func(T, P), 
+               'xVL_Vap': xVL_VapNaCl_func(T, P)}
+        
+        return res
+
+
+    def Driesner_NaClII(self, T, P, xNaCl):
+
+        calc = self.Driesner_NaCl(T, P)
+        # self.PVLH, self.xL_NaCl, self.xV_NaCl = driesnier_calc['PVLH'], driesnier_calc['xL_NaCl'], driesnier_calc['xV_NaCl']
+        # self.xVL_Liq, self.xVL_Vap = driesnier_calc['xVL_Liq'], driesnier_calc['xVL_Vap']
+        mwH2O = 18.015268
+        mwNaCl = 58.4428
+        n11 = lambda P : -54.2958 - 45.7623 * exp(-9.44785e-4 * P)
+        n21 = lambda P : -2.6142 - 0.000239092 * P
+        n22 = lambda P : 0.0356828 + 4.37235 * 10**-6 * P + 2.0566e-9 * P**2
+        n300 = lambda P : 7.60664e6 / ((P + 472.051)**2)
+        n301 = lambda P : -50 - 86.1446 * exp(-6.21128e-4 * P)
+        n302 = lambda P : 294.318 * exp(-5.66735e-3 * P)
+        n310 = lambda P : -0.0732761 * exp(-2.3772 * 10**-3 * P) - 5.2948e-5 * P
+        n311 = lambda P : -47.2747 + 24.3653 * exp(-1.25533e-3 * P)
+        n312 = lambda P : -0.278529 - 0.00081381 * P
+        n30 = lambda P, xNaCl : n300(P) * (exp(n301(P) * xNaCl) - 1) + n302(P) * xNaCl
+        n31 = lambda P, xNaCl : n310(P) * exp(n311(P) * xNaCl) + n312(P) * xNaCl
+        
+        n10 = lambda P : 330.47 + 0.942876 * P**0.5 + 0.0817193 * P - 2.47556e-8 * P**2 + 3.45052e-10 * P**3
+        n12 = lambda P : -n11(P) - n10(P)
+        n20 = lambda P : 1 - n21(P) * n22(P)**0.5
+        n23 = lambda P : -0.0370751 + 0.00237723 * P**0.5 + 5.42049e-5 * P + 5.84709e-9 * P**2 - \
+            5.99373e-13 * P**3 - n20(P) - n21(P) * (1 + n22(P))**0.5
+        n1 = lambda P, xNaCl : n10(P) + n11(P) * (1 - xNaCl) + n12(P) * (1 - xNaCl)**2
+        n2 = lambda P, xNaCl : n20(P) + n21(P) * (xNaCl + n22(P))**0.5 + n23(P) * xNaCl
+        d = lambda T, P, xNaCl : n30(P, xNaCl) * exp(n31(P, xNaCl) * T)
+        Tref_vmH2ONaCl = lambda T, P, xNaCl : n1(P, xNaCl) + n2(P, xNaCl) * T + d(T, P, xNaCl)
+    
+        #function for low P region, eq. 17 from Driesner 2007
+        #used for extrapolation of the molar volume
+        def vm_extrapolation(T, P, xNaCl):
+            v = calc['xL_NaCl'] 
+            if T <= 373.946:
+                pTmp = iapws95(T = T).P
+        
+            if xNaCl == 0:
+                return 0
+            elif T <= 200 and P < pTmp:
+                t_Ref = Tref_vmH2ONaCl(T, P, xNaCl)
+                vm_Sat = mwH2O / iapws95(T = T).rhosl * 1000
+                vm_Wat = mwH2O / iapws95(T = T, P = P).rho * 1000
+        
+                if vm_Sat < vm_Wat:
+                    o2 = 2.0125e-7 + 3.29977e-9 * exp(-4.31279 * log10(P)) - 1.17748e-7 * log10(P) + 7.58009e-8 * (log10(P))**2
+                    vm1 = mwH2O / iapws95(T = T).rhosl * 1000
+                    vm2 = mwH2O / iapws95(T = T - 0.01).rhosl * 1000
+                    o1 = (vm1 - vm2) / 0.01 - 3 * o2 * t_Ref**2
+                    o0 = vm1 - o1 * t_Ref - o2 * t_Ref**3
+                    return o0 + o2 * t_Ref**3 + o1 * t_Ref
+        
+            elif T >= 600 and P <= 350:
+                v = calc['xVL_Liq']
+                if math.floor(xNaCl*1e6)/1e6 >= math.floor(v*1e6)/1e6:
+        
+                    #local function to estimate density of vapor phase neccesery for V_extrapol funtion
+                    vmextreme_water = lambda T, P, x : mwH2O / iapws95(T = Tref_vmH2ONaCl(x, T, P), P = P).rho
+                    rhoNaCl_Vextreme = lambda T, P, x : (mwH2O * (1 - x) + mwNaCl * x) / vmextreme_water(T, P, x)* 1000.0
+        
+                    vm1000 = (mwH2O * (1 - xNaCl) + mwNaCl * xNaCl) / rhoNaCl_Vextreme(T, 1000, xNaCl) * 1000
+                    vm1 = (mwH2O * (1 - xNaCl) + mwNaCl * xNaCl) / rhoNaCl_Vextreme(T, 390.147, xNaCl) * 1000
+                    vm2 = (mwH2O * (1 - xNaCl) + mwNaCl * xNaCl) / rhoNaCl_Vextreme(T, 390.137, xNaCl) * 1000
+        
+                    dVdP390 = (vm1 - vm2) * 1e-2
+                    o4 = (vm1 - vm1000 + dVdP390 * 1609.853) / (log(1390.147 / 2000) - 2390.147 / 1390.147)
+                    o3 = vm1 - o4 * log(1390.147) - 390.147 * dVdP390 + 390.147 / 1390.147 * o4
+                    o5 = dVdP390 - o4 / (1390.147)
+        
+                    return o3 + o4 * log(P + 1000) + o5 * P
+                else:
+                    return 0
+            else:
+                return 0
+    
+        vm_H2ONaCl = lambda T, P, xNaCl : (mwH2O / (
+            iapws95(T = Tref_vmH2ONaCl(T, P, xNaCl), P = P).rho*0.001)) \
+            if vm_extrapolation(T, P, xNaCl) == 0 else vm_extrapolation(T, P, xNaCl)  #cm3/mol
+    
+        rho_H2ONaCl = lambda T, P, xNaCl : (mwH2O * (1 - xNaCl) + mwNaCl * xNaCl) / vm_H2ONaCl(T, P, xNaCl)
+        
+        def Tref_Enthalpy(xNaCl, T, P): #Th* for enthalpy
+        
+            xH2O = 1 - xNaCl
+            q11 = -32.1724 + 0.0621255 * P
+            q21 = -1.69513 - 4.52781e-4 * P - 6.04279e-8 * P**2
+            q22 = 0.0612567 + 1.88082e-5 * P
+            q10 = 47.9048 - 9.36994e-3 * P + 6.51059e-6 * P**2
+            q_twoNaCl = 0.241022 + 3.45087e-5 * P - 4.28356e-9 * P**2
+            q12 = -q11 - q10
+            q20 = 1 - q21 * q22**0.5
+            q23 = q_twoNaCl - q20 - q21 * (1 + q22)**0.5
+        
+            q1 = q10 + q11 * xH2O + q12 * xH2O**2
+            q2 = q20 + q21 * (xNaCl + q22)**0.5 + q23 * xNaCl
+        
+            tStar = q1 + q2 * T + 273.15
+        
+            return tStar, q2
+        
+        res = {'vm': vm_H2ONaCl(T, P, xNaCl)[0],
+               'rho': rho_H2ONaCl(T, P, xNaCl)[0],
+               'Tref': Tref_Enthalpy(xNaCl, T, P)[0],
+               'q2': Tref_Enthalpy(xNaCl, T, P)[-1]
+               }
+        return res
+        
+    def enthalpy_mu_heatcap(self, T, P, xNaCl):
+        """ Enthalpy in J/g, viscosity in Pas and Cp in Joules per kilogram Kelvin   """
+        calc = self.Driesner_NaClII(T, P, xNaCl)
+        tStar, q2 = calc['Tref'], calc['q2']
+        tStar = tStar - 273.15
+        prop_H2O = iapws95(T = tStar, P = P, Out_Unit = 'kilogram', FullEOSppt = True)
+        return prop_H2O.H[0], prop_H2O.mu[0], prop_H2O.Cp[0]*q2*1000  #/(1 + xNaCl)
+
```

### Comparing `pygcc-1.2.0/setup.py` & `pygcc-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'matplotlib>=3.2,<4.0',
  'numpy>=1.19.2,<2.0.0',
  'pandas>=1.0,<2.0',
  'scipy>=1.2,<2.0']
 
 setup_kwargs = {
     'name': 'pygcc',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'A tool for thermodynamic calculations and geochemical database generation',
     'long_description': '# `pygcc`\n\n<img src="_static/PyGCC_logo_vector.jpg" alt="pygcc Logo" width="40%" align="right">\n\nA tool for thermodynamic calculations and geochemical database generation\n\n[![pyGeochemCalc Documentation](https://readthedocs.org/projects/pygcc/badge/?version=latest)](https://pygcc.readthedocs.io/en/latest/?badge=latest)\n[![License: GNU General Public License v3.0](https://img.shields.io/badge/License-GNU%20General%20Public%20License%20v3.0-blue.svg?style=flat)](https://bitbucket.org/Tutolo-RTG/pygcc/src/master/LICENSE)\n\n\npyGeochemCalc (pygcc) is a python-based program for thermodynamic calculations and producing the \nGeochemist\'s Workbench (GWB), EQ3/6, TOUGHREACT, and PFLOTRAN thermodynamic database from \nambient to deep Earth temperature and pressure conditions\n\n\npygcc is developed for use in the geochemical community by providing a consolidated \nset of existing and newly implemented functions for calculating the thermodynamic properties \nof gas, aqueous, and mineral (including solid solutions and variable-formula clays) species, \nas well as reactions amongst these species, over a broad range of temperature and pressure \nconditions, but is also well suited to being modularly introduced into other modeling tools \nas desired. The documentation is continually evolving, and more examples and tutorials will gradually be added (feel free to\nrequest features or examples; see [Contributing](#contributing) below).\n\n## Installation\n\n[![PyPI](https://img.shields.io/pypi/v/pygcc.svg?style=flat)](https://pypi.org/project/pygcc/)\n[![Compatible Python Versions](https://img.shields.io/pypi/pyversions/pygcc.svg?style=flat)](https://pypi.python.org/pypi/pygcc/)\n[![pygcc downloads](https://img.shields.io/pypi/dm/pygcc.svg?style=flat)](https://pypistats.org/packages/pygcc)\n\n```bash\n$ pip install pygcc\n```\n\n## Examples\n\nCheck out the documentation for galleries of examples [General Usage](https://pygcc.readthedocs.io/en/latest/Example_1.html), \n[Integration with GWB](https://pygcc.readthedocs.io/en/latest/Example_2.html) and [Integration with EQ3/6](https://pygcc.readthedocs.io/en/latest/Example_3.html). \nIf you would prefer to flip through notebooks on Bitbucket, these same examples can be found in the folder [`docs/`](https://bitbucket.org/Tutolo-RTG/pygcc/src/master/docs/).\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. \nBy contributing to this project, you agree to abide by its terms. For more information, see the [documentation](https://pygcc.readthedocs.io/), \nparticularly the [Contributing page](https://pygcc.readthedocs.io/en/latest/contributing.html) and \n[Code of Conduct](https://pygcc.readthedocs.io/en/latest/conduct.html). \n\n## License\n\n`pygcc` was created by Adedapo Awolayo and Benjamin Tutolo. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Citation\n\nIf you use pygcc for your research, citation of the software would be appreciated. It helps to quantify the impact of \npygcc, and build the pygcc community. For information on citing pygcc, \n[see the relevant docs page](https://pygcc.readthedocs.io/en/latest/pygcc_overview.html#citation-and-contact-information-a-class-anchor-id-section-6-a)\n\n## Credits\n`pygcc Logo` was designed by [`Yury Klyukin`](https://www.linkedin.com/in/yury-klyukin-68517ba2/), `pygcc` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Adedapo Awolayo and Benjamin Tutolo',
     'author_email': None,
     'maintainer': 'Adedapo Awolayo and Benjamin Tutolo',
     'maintainer_email': 'benjamin.tutolo@ucalgary.ca',
     'url': 'https://bitbucket.org/Tutolo-RTG/pygcc/src/master/',
```

### Comparing `pygcc-1.2.0/PKG-INFO` & `pygcc-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygcc
-Version: 1.2.0
+Version: 1.3.0
 Summary: A tool for thermodynamic calculations and geochemical database generation
 Home-page: https://bitbucket.org/Tutolo-RTG/pygcc/src/master/
 License: GNU General Public License v3.0
 Keywords: Geochemistry,Thermodynamic database,Thermodynamic calculations,Solid-solutions,Density extrapolation
 Author: Adedapo Awolayo and Benjamin Tutolo
 Maintainer: Adedapo Awolayo and Benjamin Tutolo
 Maintainer-email: benjamin.tutolo@ucalgary.ca
```

