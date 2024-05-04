# Comparing `tmp/scikit_fingerprints-1.2.0.tar.gz` & `tmp/scikit_fingerprints-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_fingerprints-1.2.0.tar", max compression
+gzip compressed data, was "scikit_fingerprints-1.4.0.tar", max compression
```

## Comparing `scikit_fingerprints-1.2.0.tar` & `scikit_fingerprints-1.4.0.tar`

### file list

```diff
@@ -1,31 +1,45 @@
--rw-r--r--   0        0        0     1116 2024-03-26 21:45:13.956891 scikit_fingerprints-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     2659 2024-03-26 21:45:13.956891 scikit_fingerprints-1.2.0/README.md
--rw-r--r--   0        0        0     1250 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/__init__.py
--rw-r--r--   0        0        0      941 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/__init__.py
--rw-r--r--   0        0        0     1701 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/atom_pair.py
--rw-r--r--   0        0        0     1155 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/autocorr.py
--rw-r--r--   0        0        0     1134 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/avalon.py
--rw-r--r--   0        0        0     4092 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/base.py
--rw-r--r--   0        0        0     3981 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/e3fp_fp.py
--rw-r--r--   0        0        0     3056 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/ecfp.py
--rw-r--r--   0        0        0     1413 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/erg.py
--rw-r--r--   0        0        0     1269 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/estate.py
--rw-r--r--   0        0        0     1054 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/getaway.py
--rw-r--r--   0        0        0      886 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/maccs.py
--rw-r--r--   0        0        0     5903 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/map4.py
--rw-r--r--   0        0        0     2046 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/mhfp.py
--rw-r--r--   0        0        0      911 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/morse.py
--rw-r--r--   0        0        0     1153 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/pattern.py
--rw-r--r--   0        0        0     2030 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/pharmacophore.py
--rw-r--r--   0        0        0     1421 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/physiochemical_properties.py
--rw-r--r--   0        0        0    41593 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/pubchem.py
--rw-r--r--   0        0        0      903 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/rdf.py
--rw-r--r--   0        0        0     1788 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/rdk.py
--rw-r--r--   0        0        0     1636 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/secfp.py
--rw-r--r--   0        0        0     1765 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/topological_torsion.py
--rw-r--r--   0        0        0     1042 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/fingerprints/whim.py
--rw-r--r--   0        0        0     4109 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/preprocessing.py
--rw-r--r--   0        0        0     1500 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/utils.py
--rw-r--r--   0        0        0      916 2024-03-26 21:45:13.960891 scikit_fingerprints-1.2.0/skfp/validators.py
--rw-r--r--   0        0        0     3618 1970-01-01 00:00:00.000000 scikit_fingerprints-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1116 2024-05-04 20:40:05.660851 scikit_fingerprints-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     3243 2024-05-04 20:40:05.660851 scikit_fingerprints-1.4.0/README.md
+-rwxr-xr-x   0        0        0     1437 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/__init__.py
+-rw-r--r--   0        0        0     6701 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_fp_transformer.py
+-rw-r--r--   0        0        0     1704 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_preprocessor.py
+-rw-r--r--   0        0        0     4439 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/bases/base_substructure_fp.py
+-rw-r--r--   0        0        0     1268 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/__init__.py
+-rw-r--r--   0        0        0     9801 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/atom_pair.py
+-rw-r--r--   0        0        0     1535 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/autocorr.py
+-rw-r--r--   0        0        0     4375 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/avalon.py
+-rw-r--r--   0        0        0     8690 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/e3fp_fp.py
+-rw-r--r--   0        0        0     3095 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/ecfp.py
+-rw-r--r--   0        0        0     8229 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/erg.py
+-rw-r--r--   0        0        0     1513 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/estate.py
+-rw-r--r--   0        0        0     1439 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/getaway.py
+-rw-r--r--   0        0        0     7279 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/ghose_crippen.py
+-rw-r--r--   0        0        0   235066 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/klekota_roth.py
+-rw-r--r--   0        0        0    28051 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/laggner.py
+-rw-r--r--   0        0        0     2455 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/layered.py
+-rw-r--r--   0        0        0     6344 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/lingo.py
+-rw-r--r--   0        0        0     1091 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/maccs.py
+-rw-r--r--   0        0        0     6806 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/map.py
+-rw-r--r--   0        0        0     3115 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/mhfp.py
+-rw-r--r--   0        0        0     1421 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/mordred_fp.py
+-rw-r--r--   0        0        0     1069 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/morse.py
+-rw-r--r--   0        0        0     1631 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pattern.py
+-rw-r--r--   0        0        0     2683 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pharmacophore.py
+-rw-r--r--   0        0        0     1785 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/physiochemical_properties.py
+-rw-r--r--   0        0        0    41700 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/pubchem.py
+-rw-r--r--   0        0        0     1061 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/rdf.py
+-rw-r--r--   0        0        0     2898 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/rdk.py
+-rw-r--r--   0        0        0     2751 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/secfp.py
+-rw-r--r--   0        0        0     2194 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/topological_torsion.py
+-rw-r--r--   0        0        0     7561 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/usr.py
+-rw-r--r--   0        0        0     8145 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/usrcat.py
+-rw-r--r--   0        0        0     1427 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/fingerprints/whim.py
+-rw-r--r--   0        0        0     3787 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/parallel.py
+-rw-r--r--   0        0        0      133 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/__init__.py
+-rw-r--r--   0        0        0    14959 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/conformer_generator.py
+-rw-r--r--   0        0        0     2494 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/preprocessing/mol_to_from_smiles.py
+-rw-r--r--   0        0        0      243 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/rdkit_logging.py
+-rw-r--r--   0        0        0     1118 2024-05-04 20:40:05.664851 scikit_fingerprints-1.4.0/skfp/validators.py
+-rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 scikit_fingerprints-1.4.0/PKG-INFO
```

### Comparing `scikit_fingerprints-1.2.0/LICENSE.md` & `scikit_fingerprints-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scikit_fingerprints-1.2.0/README.md` & `scikit_fingerprints-1.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,76 @@
 # scikit-fingerprints
 
 A Python library for efficient computation of molecular fingerprints
 
+Click [HERE](https://scikit-fingerprints.github.io/scikit-fingerprints/) to see the Documentation.
 
 ## Table of Contents
+
 - [Description](#description)
 - [General Project Vision](#general-project-vision)
 - [Library Description](#library-description)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Technologies Used](#technologies-used)
 - [Contributing](#contributing)
 - [License](#license)
 
 ---
 
 ## Description
 
-Molecular fingerprints are crucial in various scientific fields, including drug discovery, materials science, and chemical analysis. However, existing Python libraries for computing molecular fingerprints often lack performance, user-friendliness, and support for modern programming standards. This project aims to address these shortcomings by creating an efficient and accessible Python library for molecular fingerprint computation.
+Molecular fingerprints are crucial in various scientific fields, including drug discovery, materials science, and
+chemical analysis. However, existing Python libraries for computing molecular fingerprints often lack performance,
+user-friendliness, and support for modern programming standards. This project aims to address these shortcomings by
+creating an efficient and accessible Python library for molecular fingerprint computation.
+
+## Supported platforms
+
+|                      | `python3.9`   | `python3.10` | `python3.11` | `python3.12` |
+|----------------------|---------------|--------------|--------------|--------------|
+| **Ubuntu - latest**  | ✅             | ✅            | ✅            | ✅            |
+| **Windows - latest** | ✅             | ✅            | ✅            | ✅            |
+| **macOS - latest**   | only macOS 13 | ✅            | ✅            | ✅            |
 
 ## Installation
 
 You can install the library using pip:
 
 ```bash
 pip install scikit-fingerprints
 ```
 
 ## General Project Vision
- 
-The primary goal of this project was to develop a Python library that simplifies the computation of widely-used molecular fingerprints, such as Morgan's fingerprint, MACCS fingerprint, and others. This library has the following key features:
 
-- **User-Friendly Interface:** The library was designed to provide an intuitive interface, making it easy to integrate into machine learning workflows.
+The primary goal of this project was to develop a Python library that simplifies the computation of widely-used
+molecular fingerprints, such as Morgan's fingerprint, MACCS fingerprint, and others. This library has the following key
+features:
+
+- **User-Friendly Interface:** The library was designed to provide an intuitive interface, making it easy to integrate
+  into machine learning workflows.
 
-- **Performance Optimization:** We implemented molecular fingerprint computation algorithms using concurrent programming techniques to maximize performance. Large datasets of molecules are processed in parallel for improved efficiency.
+- **Performance Optimization:** We implemented molecular fingerprint computation algorithms using concurrent programming
+  techniques to maximize performance. Large datasets of molecules are processed in parallel for improved efficiency.
 
-- **Compatibility:** The library's interface was inspired by popular data science libraries like Scikit-Learn, ensuring compatibility and familiarity for users familiar with these tools.
+- **Compatibility:** The library's interface was inspired by popular data science libraries like Scikit-Learn, ensuring
+  compatibility and familiarity for users familiar with these tools.
 
 - **Extensibility:** Users should be able to customize and extend the library to suit their specific needs.
 
 ## Library Description
 
-- The library offers various functions that accept molecule descriptors (e.g., SMILES) and fingerprint parameters, returning the specified fingerprints.
+- The library offers various functions that accept molecule descriptors (e.g., SMILES) and fingerprint parameters,
+  returning the specified fingerprints.
 - It's open-source and available for installation via pip.
 - The library has been designed for ease of use, minimizing the need for extensive training.
 - Compatibility with the standard Python ML stack, based on Scikit-Learn interfaces, has been a top priority.
 
 ## Contributing
 
-Please read [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details on our code of conduct, and the process for submitting pull requests to us.
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details on our code of
+conduct, and the process for submitting pull requests to us.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikit_fingerprints-1.2.0/pyproject.toml` & `scikit_fingerprints-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scikit-fingerprints"
-version = "1.2.0"
+version = "1.4.0"
 description = "Library for effective molecular fingerprints calculation"
 authors = [
     "Scikit-Fingerprints Development Team <scikitfingerprints@gmail.com>",
     "Jakub Adamczyk <jakub.adamczyk10@gmail.com>",
     "Przemyslaw Kukla <przemek.kukla0703@gmail.com>",
     "Piotr Ludynia <piotrztych@gmail.com>",
     "Michal Szafarczyk <adammichal657@gmail.com>",
@@ -19,45 +19,56 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 datasketch = "*"
 e3fp = "*"
 joblib = "*"
+mordredcommunity = "*"
 numpy = "^1.20.0"
 pandas = "*"
 rdkit = "*"
 scikit-learn = "*"
 scipy = "*"
 tqdm = "*"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
+coverage = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pre-commit = "*"
 pytest = "*"
+pytest-cov = "*"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 mypy = "*"
 pre-commit = "*"
 pytest = "*"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
+pydata-sphinx-theme = "*"
 sphinx = "*"
 
+[tool.poetry.group.eval]
+optional = true
+
+[tool.poetry.group.eval.dependencies]
+lightgbm = "*"
+ogb = "*"
+
 [tool.pytest.ini_options]
 python_files = "*.py"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/__init__.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,28 @@
 from .autocorr import AutocorrFingerprint
 from .avalon import AvalonFingerprint
 from .e3fp_fp import E3FPFingerprint
 from .ecfp import ECFPFingerprint
 from .erg import ERGFingerprint
 from .estate import EStateFingerprint
 from .getaway import GETAWAYFingerprint
+from .ghose_crippen import GhoseCrippenFingerprint
+from .klekota_roth import KlekotaRothFingerprint
+from .laggner import LaggnerFingerprint
+from .layered import LayeredFingerprint
+from .lingo import LingoFingerprint
 from .maccs import MACCSFingerprint
-from .map4 import MAP4Fingerprint
+from .map import MAPFingerprint
 from .mhfp import MHFPFingerprint
+from .mordred_fp import MordredFingerprint
 from .morse import MORSEFingerprint
 from .pattern import PatternFingerprint
 from .pharmacophore import PharmacophoreFingerprint
 from .physiochemical_properties import PhysiochemicalPropertiesFingerprint
 from .pubchem import PubChemFingerprint
 from .rdf import RDFFingerprint
 from .rdk import RDKitFingerprint
 from .secfp import SECFPFingerprint
 from .topological_torsion import TopologicalTorsionFingerprint
+from .usr import USRFingerprint
+from .usrcat import USRCATFingerprint
 from .whim import WHIMFingerprint
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/atom_pair.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/estate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,53 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
+from sklearn.utils._param_validation import StrOptions
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
-class AtomPairFingerprint(FingerprintTransformer):
-    """Atom pair fingerprint."""
+class EStateFingerprint(BaseFingerprintTransformer):
+    """EState fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "variant": [StrOptions({"bit", "count", "sum"})],
+    }
 
     def __init__(
         self,
-        fp_size: int = 2048,
-        min_distance: int = 1,
-        max_distance: int = 30,
-        include_chirality: bool = False,
-        use_2D: bool = True,
-        count: bool = False,
+        variant: str = "sum",
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
-            count=count,
+            n_features_out=79,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
-        self.fp_size = fp_size
-        self.min_distance = min_distance
-        self.max_distance = max_distance
-        self.include_chirality = include_chirality
-        self.use_2D = use_2D
+        self.variant = variant
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.rdFingerprintGenerator import GetAtomPairGenerator
+        from rdkit.Chem.EState.Fingerprinter import FingerprintMol
 
         X = ensure_mols(X)
 
-        gen = GetAtomPairGenerator(
-            fpSize=self.fp_size,
-            minDistance=self.min_distance,
-            maxDistance=self.max_distance,
-            includeChirality=self.include_chirality,
-            use2D=self.use_2D,
-            countSimulation=self.count,
-        )
-        if self.count:
-            X = [gen.GetCountFingerprintAsNumPy(x) for x in X]
-        else:
-            X = [gen.GetFingerprintAsNumPy(x) for x in X]
+        X = np.array([FingerprintMol(x) for x in X])
+        if self.variant == "bit":
+            X = (X[:, 0] > 0).astype(np.uint8)
+        elif self.variant == "count":
+            X = (X[:, 0]).astype(np.uint32)
+        else:  # "sum" variant
+            X = X[:, 1]
 
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/estate.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/physiochemical_properties.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,61 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from numbers import Integral
+from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
+from sklearn.utils import Interval
+from sklearn.utils._param_validation import StrOptions
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
-class EStateFingerprint(FingerprintTransformer):
-    """EState fingerprint."""
+class PhysiochemicalPropertiesFingerprint(BaseFingerprintTransformer):
+    """Physiochemical properties fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "fp_size": [Interval(Integral, 1, None, closed="left")],
+        "variant": [StrOptions({"BP", "BT"})],
+    }
 
     def __init__(
         self,
-        variant: str = "sum",
+        fp_size: int = 2048,
+        variant: str = "BP",
+        count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
-        if variant not in ["bit", "count", "sum"]:
-            raise ValueError("Variant must be one of: 'bit', 'count', 'sum'")
-
         super().__init__(
-            n_jobs=n_jobs,
+            n_features_out=fp_size,
+            count=count,
             sparse=sparse,
+            n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
+        self.fp_size = fp_size
         self.variant = variant
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.EState.Fingerprinter import FingerprintMol
+        from rdkit.Chem.AtomPairs.Sheridan import GetBPFingerprint, GetBTFingerprint
 
         X = ensure_mols(X)
 
-        X = np.array([FingerprintMol(x) for x in X])
-        if self.variant == "bit":
-            X = X[:, 0] > 0
-        elif self.variant == "count":
-            X = (X[:, 0]).astype(int)
-        else:  # "sum" variant
-            X = X[:, 1]
+        if self.variant == "BP":
+            X = [GetBPFingerprint(mol) for mol in X]
+        else:  # "BT" variant
+            X = [GetBTFingerprint(mol) for mol in X]
+
+        X = self._hash_fingerprint_bits(
+            X, fp_size=self.fp_size, count=self.count, sparse=self.sparse
+        )
 
-        return csr_array(X) if self.sparse else np.array(X)
+        return X
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/map4.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,98 @@
+import hashlib
 import itertools
+import struct
 from collections import defaultdict
-from typing import Dict, List, Optional, Sequence, Union
+from collections.abc import Sequence
+from numbers import Integral
+from typing import Optional, Union
 
 import numpy as np
 from datasketch import MinHash
 from rdkit.Chem import MolToSmiles, PathToSubmol
 from rdkit.Chem.rdchem import Mol
 from rdkit.Chem.rdmolops import FindAtomEnvironmentOfRadiusN, GetDistanceMatrix
 from scipy.sparse import csr_array
+from sklearn.utils import Interval
+from sklearn.utils._param_validation import StrOptions
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 """
 Code inspired by the original work of the authors of the MAP4 Fingerprint:
 https://github.com/reymond-group/map4
 """
 
 
-class MAP4Fingerprint(FingerprintTransformer):
-    """MAP4 fingerprint."""
+class MAPFingerprint(BaseFingerprintTransformer):
+    """MAP fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "fp_size": [Interval(Integral, 1, None, closed="left")],
+        "radius": [Interval(Integral, 0, None, closed="left")],
+        "variant": [StrOptions({"bit", "count", "raw_hashes"})],
+    }
 
     def __init__(
         self,
         fp_size: int = 1024,
         radius: int = 2,
         variant: str = "bit",
         sparse: bool = False,
         count: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
         random_state: int = 0,
     ):
-        if variant not in ["bit", "count", "raw_hashes"]:
-            raise ValueError("Variant must be one of: 'bit', 'count', 'raw_hashes'")
-
         super().__init__(
+            n_features_out=fp_size,
             sparse=sparse,
             count=count,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
             random_state=random_state,
         )
         self.fp_size = fp_size
         self.radius = radius
         self.variant = variant
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         X = ensure_mols(X)
         X = np.stack([self._calculate_single_mol_fingerprint(x) for x in X], dtype=int)
 
-        if self.variant in ["bit", "count"]:
-            X = np.mod(X, self.fp_size)
-            X = np.stack([np.bincount(x, minlength=self.fp_size) for x in X])
-            if self.variant == "bit":
-                X = X > 0
+        if self.variant == "bit":
+            X = (X > 0).astype(np.uint8)
+        elif self.variant == "count":
+            X = X.astype(np.uint32)
 
         return csr_array(X) if self.sparse else np.array(X)
 
     def _calculate_single_mol_fingerprint(self, mol: Mol) -> np.ndarray:
         atoms_envs = self._get_atom_envs(mol)
-        atom_env_pairs = self._get_atom_pair_shingles(mol, atoms_envs)
-        encoder = MinHash(num_perm=self.fp_size, seed=self.random_state)
-        encoder.update_batch(atom_env_pairs)
-        fp = encoder.digest()
+        shingles = self._get_atom_pair_shingles(mol, atoms_envs)
+
+        if self.variant == "raw_hashes":
+            encoder = MinHash(num_perm=self.fp_size, seed=self.random_state)
+            encoder.update_batch(shingles)
+            fp = encoder.digest()
+        else:
+            # bit/count folded version from original MAP4 and MHFP implementation
+            hashes = [self._get_hash(shingle) for shingle in shingles]
+            bits = [hash_val % self.fp_size for hash_val in hashes]
+            fp = np.bincount(bits, minlength=self.fp_size)
+
         return fp
 
-    def _get_atom_envs(self, mol: Mol) -> Dict[int, List[Optional[str]]]:
+    def _get_atom_envs(self, mol: Mol) -> dict[int, list[Optional[str]]]:
         """
         For each atom get its environment, i.e. radius-hop neighborhood.
         """
         atoms_env = defaultdict(list)
         for atom in mol.GetAtoms():
             idx = atom.GetIdx()
             atom_envs = [
@@ -88,45 +108,42 @@
         """
         Get the radius-hop neighborhood for a given atom. If there is no neighborhood
         of a given radius, e.g. 2-hop neighborhood for [Li]F with just two atoms,
         returns None.
         """
         try:
             env = FindAtomEnvironmentOfRadiusN(mol, atom_idx, n_radius)
-        except ValueError as e:
-            # this error happens if radius is larger than possible
-            if "bad atom index" in str(e):
-                return None
-            else:
-                raise
+        except ValueError:
+            # "bad atom index" error happens if radius is larger than possible
+            return None
 
-        atom_map: Dict[int, int] = dict()
+        atom_map: dict[int, int] = dict()
 
         submol = PathToSubmol(mol, env, atomMap=atom_map)
 
         if atom_idx in atom_map:
             return MolToSmiles(
                 submol,
                 rootedAtAtom=atom_map[atom_idx],
                 canonical=True,
                 isomericSmiles=False,
             )
         else:
             return None
 
-    def _get_atom_pair_shingles(self, mol: Mol, atoms_envs: dict) -> List[bytes]:
+    def _get_atom_pair_shingles(self, mol: Mol, atoms_envs: dict) -> list[bytes]:
         """
-        Gets a list of atom-pair molecular shingles - circular structures written
-        as SMILES, separated by the bond distance between the two atoms along the
+        Gets a list of atom molecular shingles - circular structures around atom pairs,
+        written as SMILES, separated by the bond distance between the two atoms along the
         shortest path.
         """
-        atom_pairs = []
+        shingles = []
         distance_matrix = GetDistanceMatrix(mol)
         num_atoms = mol.GetNumAtoms()
-        shingle_dict: Dict[str, int] = defaultdict(int)
+        shingle_dict: dict[str, int] = defaultdict(int)
 
         # Iterate through all pairs of atoms and radius. Shingles are stored in format:
         # (radius i neighborhood of atom A) | (distance between atoms A and B) | (radius i neighborhood of atom B)
         #
         # If we want to count the shingles, we increment their value in shingle_dict
         # After nested for-loop, all shingles, with their respective counts, will be added to atom_pairs list.
         for idx_1, idx_2 in itertools.combinations(range(num_atoms), 2):
@@ -145,20 +162,28 @@
 
                 ordered = sorted([env_a_radius, env_b_radius])
                 shingle = f"{ordered[0]}|{dist}|{ordered[1]}"
 
                 if self.count:
                     shingle_dict[shingle] += 1
                 else:
-                    atom_pairs.append(shingle.encode("utf-8"))
+                    shingles.append(shingle)
 
         if self.count:
             # shingle in format:
             # (radius i neighborhood of atom A) | (distance between atoms A and B) | \
             # (radius i neighborhood of atom B) | (shingle count)
-            new_atom_pairs = [
-                f"{shingle}|{shingle_count}".encode()
+            shingle_count = [
+                f"{shingle}|{shingle_count}"
                 for shingle, shingle_count in shingle_dict.items()
             ]
-            atom_pairs.extend(new_atom_pairs)
+            shingles.extend(shingle_count)
+
+        # convert strings to bytes for hashing
+        shingles = [shingle.encode() for shingle in shingles]
+
+        return shingles
 
-        return atom_pairs
+    def _get_hash(self, shingle: bytes) -> int:
+        hash_bytes = hashlib.sha1(shingle, usedforsecurity=False).digest()
+        hash_value = struct.unpack("<I", hash_bytes[:4])[0]
+        return hash_value
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/mhfp.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/secfp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,89 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from numbers import Integral
+from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
+from sklearn.utils import Interval
+from sklearn.utils._param_validation import InvalidParameterError
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
-class MHFPFingerprint(FingerprintTransformer):
-    """MinHashed FingerPrint (MHFP) transformer."""
+class SECFPFingerprint(BaseFingerprintTransformer):
+    """SECFP fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "fp_size": [Interval(Integral, 1, None, closed="left")],
+        "radius": [Interval(Integral, 1, None, closed="left")],
+        "min_radius": [Interval(Integral, 1, None, closed="left")],
+        "rings": ["boolean"],
+        "isomeric": ["boolean"],
+        "kekulize": ["boolean"],
+    }
 
     def __init__(
         self,
         fp_size: int = 2048,
         radius: int = 3,
         min_radius: int = 1,
         rings: bool = True,
         isomeric: bool = False,
         kekulize: bool = True,
-        variant: str = "bit",
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
-        if variant not in ["bit", "count", "raw_hashes"]:
-            raise ValueError("Variant must be one of: 'bit', 'count', 'raw_hashes'")
-
         super().__init__(
+            n_features_out=fp_size,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
         self.fp_size = fp_size
         self.radius = radius
         self.min_radius = min_radius
         self.rings = rings
         self.isomeric = isomeric
         self.kekulize = kekulize
-        self.variant = variant
+
+    def _validate_params(self) -> None:
+        super()._validate_params()
+        if self.radius < self.min_radius:
+            raise InvalidParameterError(
+                f"The radius parameter of {self.__class__.__name__} must be "
+                f"greater or equal to min_radius, got: "
+                f"min_radius={self.min_radius}, radius={self.radius}"
+            )
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.rdMHFPFingerprint import MHFPEncoder
 
         X = ensure_mols(X)
 
-        # outputs raw hash values, not feature vectors!
+        # bulk function does not work
         encoder = MHFPEncoder(self.fp_size, self.random_state)
-        X = MHFPEncoder.EncodeMolsBulk(
-            encoder,
-            X,
-            radius=self.radius,
-            min_radius=self.min_radius,
-            rings=self.rings,
-            isomeric=self.isomeric,
-            kekulize=self.kekulize,
-        )
-        X = np.array(X)
-
-        if self.variant in ["bit", "count"]:
-            X = np.mod(X, self.fp_size)
-            X = np.stack([np.bincount(x, minlength=self.fp_size) for x in X])
-            if self.variant == "bit":
-                X = X > 0
-
-        return csr_array(X) if self.sparse else np.array(X)
+        X = [
+            encoder.EncodeSECFPMol(
+                x,
+                length=self.fp_size,
+                radius=self.radius,
+                min_radius=self.min_radius,
+                rings=self.rings,
+                isomeric=self.isomeric,
+                kekulize=self.kekulize,
+            )
+            for x in X
+        ]
+
+        if self.sparse:
+            return csr_array(X, dtype=np.uint8)
+        else:
+            return np.array(X, dtype=np.uint8)
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/morse.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/morse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import require_mols_with_conf_ids
 
 
-class MORSEFingerprint(FingerprintTransformer):
+class MORSEFingerprint(BaseFingerprintTransformer):
     """MORSE fingerprint."""
 
     def __init__(
         self,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
+            n_features_out=224,
+            requires_conformers=True,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
 
-    def _calculate_fingerprint(
-        self, X: Sequence[Union[str, Mol]]
-    ) -> Union[np.ndarray, csr_array]:
+    def _calculate_fingerprint(self, X: Sequence[Mol]) -> Union[np.ndarray, csr_array]:
         from rdkit.Chem.rdMolDescriptors import CalcMORSE
 
         X = require_mols_with_conf_ids(X)
-        X = [CalcMORSE(mol, confId=mol.conf_id) for mol in X]
+        X = [CalcMORSE(mol, confId=mol.GetIntProp("conf_id")) for mol in X]
         return csr_array(X) if self.sparse else np.array(X)
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/physiochemical_properties.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/mordred_fp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-from typing import Optional, Sequence, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
+from mordred import Calculator, descriptors
 from rdkit.Chem import Mol
 from scipy.sparse import csr_array
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 
-class PhysiochemicalPropertiesFingerprint(FingerprintTransformer):
-    """Physiochemical properties fingerprint."""
+class MordredFingerprint(BaseFingerprintTransformer):
+    """Mordred fingerprint."""
+
+    _parameter_constraints: dict = {
+        **BaseFingerprintTransformer._parameter_constraints,
+        "use_3D": ["boolean"],
+    }
 
     def __init__(
         self,
-        fp_size: int = 2048,
-        variant: str = "BP",
-        count: bool = False,
+        use_3D: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
-        if variant not in ["BP", "BT"]:
-            raise ValueError("Variant must be one of: 'BP', 'BT'")
-
+        n_features_out = 1826 if use_3D else 1613
         super().__init__(
-            count=count,
+            n_features_out=n_features_out,
+            requires_conformers=use_3D,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
-        self.fp_size = fp_size
-        self.variant = variant
+        self.use_3D = use_3D
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
-        from rdkit.Chem.AtomPairs.Sheridan import GetBPFingerprint, GetBTFingerprint
-
         X = ensure_mols(X)
 
-        if self.variant == "BP":
-            X = [GetBPFingerprint(mol) for mol in X]
-        else:  # "BT" variant
-            X = [GetBTFingerprint(mol) for mol in X]
+        calc = Calculator(descriptors, ignore_3D=not self.use_3D)
+        X = [calc(x) for x in X]
 
-        X = self._hash_fingerprint_bits(
-            X, fp_size=self.fp_size, count=self.count, sparse=self.sparse
+        return (
+            csr_array(X, dtype=np.float32)
+            if self.sparse
+            else np.array(X, dtype=np.float32)
         )
-
-        return X
```

### Comparing `scikit_fingerprints-1.2.0/skfp/fingerprints/pubchem.py` & `scikit_fingerprints-1.4.0/skfp/fingerprints/pubchem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 from collections import defaultdict
-from typing import Dict, List, Optional, Sequence, Tuple, Union
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
-import scipy.sparse
 from rdkit.Chem import AddHs, Mol
 from scipy.sparse import csr_array
 
-from skfp.fingerprints.base import FingerprintTransformer
+from skfp.bases import BaseFingerprintTransformer
 from skfp.validators import ensure_mols
 
 """
 Note: this fingerprint may give slightly different vectors than PubChem API!
 This is because we use aromaticity models from RDKit, and ring features may
 be counted differently due to this. This is typically only a very small subset
 of bits, though. In particular, all SMARTS patterns exactly follow the original
 NCGC (NIH) Java code.
 """
 
 
-class PubChemFingerprint(FingerprintTransformer):
+class PubChemFingerprint(BaseFingerprintTransformer):
     """PubChem fingerprint."""
 
     def __init__(
         self,
         count: bool = False,
         sparse: bool = False,
         n_jobs: Optional[int] = None,
+        batch_size: Optional[int] = None,
         verbose: int = 0,
     ):
         super().__init__(
+            n_features_out=881,
             count=count,
             sparse=sparse,
             n_jobs=n_jobs,
+            batch_size=batch_size,
             verbose=verbose,
         )
 
     def _calculate_fingerprint(
         self, X: Sequence[Union[str, Mol]]
     ) -> Union[np.ndarray, csr_array]:
         X = ensure_mols(X)
 
         X = [self._get_pubchem_fingerprint(x) for x in X]
-        return scipy.sparse.vstack(X) if self.sparse else np.vstack(X)
+        return csr_array(X) if self.sparse else np.vstack(X)
 
     def _get_pubchem_fingerprint(self, mol: Mol) -> Union[np.ndarray, csr_array]:
         # PubChem's definition requires hydrogens to be present
         mol = AddHs(mol)
 
         atom_counts = self._get_atom_counts(mol)
         ring_counts = self._get_ESSSR_ring_counts(mol)
@@ -259,35 +262,37 @@
                     "Yb",
                     "Tc",
                     "U",
                 ]
             ]
             ring_features = self._get_ring_count_features(ring_counts)
 
-        x = (
+        X = np.array(
             atom_features
             + ring_features
             + atom_pair_counts
             + simple_neigh_counts
             + detailed_neigh_counts
             + simple_smarts_counts
-            + complex_smarts_counts
+            + complex_smarts_counts,
         )
-        X = csr_array(x) if self.sparse else np.array(x)
 
-        return (X > 0) if not self.count else X
+        if self.count:
+            return X.astype(np.uint32)
+        else:
+            return (X > 0).astype(np.uint8)
 
-    def _get_atom_counts(self, mol: Mol) -> Dict[str, int]:
-        counts: Dict[str, int] = defaultdict(int)
+    def _get_atom_counts(self, mol: Mol) -> dict[str, int]:
+        counts: dict[str, int] = defaultdict(int)
         for atom in mol.GetAtoms():
             counts[atom.GetSymbol()] += 1
         return counts
 
-    def _get_ESSSR_ring_counts(self, mol: Mol) -> Dict[str, int]:
-        counts: Dict[str, int] = defaultdict(int)
+    def _get_ESSSR_ring_counts(self, mol: Mol) -> dict[str, int]:
+        counts: dict[str, int] = defaultdict(int)
 
         ring_info = mol.GetRingInfo()
         for ring in ring_info.BondRings():
             ring = self._get_ring_stats(mol, ring)
             size = ring["size"]
 
             counts[f"ring_size_{size}"] += 1
@@ -316,16 +321,16 @@
 
             counts[f"ring_aromatic_{size}"] += ring["aromatic"]
             counts[f"ring_hetero_aromatic_{size}"] += ring["hetero_aromatic"]
 
         return counts
 
     def _get_ring_stats(
-        self, mol: Mol, ring: Tuple[int]
-    ) -> Dict[str, Union[int, bool]]:
+        self, mol: Mol, ring: tuple[int]
+    ) -> dict[str, Union[int, bool]]:
         from rdkit.Chem import BondType
 
         stats = {
             "size": 0,
             "aromatic": True,
             "hetero_aromatic": True,
             "saturated_or_aromatic": True,
@@ -351,15 +356,15 @@
             stats["has_nitrogen"] |= (atom_1_type == "N") | (atom_2_type == "N")
             stats["has_heteroatom"] |= (atom_1_type == "C") | (atom_2_type == "H")
 
         stats["hetero_aromatic"] = ~stats["carbon_only"] & stats["aromatic"]
 
         return stats
 
-    def _get_ring_binary_features(self, ring_counts: Dict[str, int]) -> List[int]:
+    def _get_ring_binary_features(self, ring_counts: dict[str, int]) -> list[int]:
         # for each ring size, we have different number of binary features, for multiple
         # count thresholds, e.g. for 7-atom rings we have 2 sets of features (>=1, >=2),
         # and for 5-atom rings we have 5 sets
         ring_size_count_thresholds = {
             3: [1, 2],
             4: [1, 2],
             5: [1, 2, 3, 4, 5],
@@ -401,15 +406,15 @@
             num_hetero_aromatic_rings >= 4,
         ]
         features.extend(aromatic_ring_features)
 
         features = [int(feat) for feat in features]
         return features
 
-    def _get_ring_count_features(self, ring_counts: Dict[str, int]) -> List[int]:
+    def _get_ring_count_features(self, ring_counts: dict[str, int]) -> list[int]:
         # for each ring size, we count all
         features = []
 
         num_aromatic_rings = 0
         num_hetero_aromatic_rings = 0
 
         for size in range(3, 11):
@@ -427,15 +432,15 @@
             num_hetero_aromatic_rings += ring_counts[f"ring_hetero_aromatic_{size}"]
 
         features.append(num_aromatic_rings)
         features.append(num_hetero_aromatic_rings)
 
         return features
 
-    def _get_atom_pair_counts(self, mol: Mol) -> List[int]:
+    def _get_atom_pair_counts(self, mol: Mol) -> list[int]:
         smarts_list = [
             "[Li]~[H]",
             "[Li]~[Li]",
             "[Li]~[B]",
             "[Li]~[#6]",
             "[Li]~[#8]",
             "[Li]~[F]",
@@ -496,15 +501,15 @@
             "[#15]~[H]",
             "[#15]~[#15]",
             "[As]~[H]",
             "[As]~[As]",
         ]
         return self._get_smarts_match_counts(mol, smarts_list)
 
-    def _get_simple_neighborhoods_counts(self, mol: Mol) -> List[int]:
+    def _get_simple_neighborhoods_counts(self, mol: Mol) -> list[int]:
         smarts_list = [
             "[#6](~Br)(~[#6])",
             "[#6](~Br)(~[#6])(~[#6])",
             "[#6](~[Br])([H])",
             "[#6](~[Br])(:[c])",
             "[#6](~[Br])(:[n])",
             "[#6](~[#6])(~[#6])",
@@ -590,15 +595,15 @@
             "[#16](~[#6])(~[#6])",
             "[#16](~[#6])([H])",
             "[#16](~[#6])(~[#8])",
             "[Si](~[#6])(~[#6])",
         ]
         return self._get_smarts_match_counts(mol, smarts_list)
 
-    def _get_detailed_neighborhoods_counts(self, mol: Mol) -> List[int]:
+    def _get_detailed_neighborhoods_counts(self, mol: Mol) -> list[int]:
         smarts_list = [
             "[#6]=,:[#6]",
             "[#6]#[#6]",
             "[#6]=,:[#7]",
             "[#6]#[#7]",
             "[#6]=,:[#8]",
             "[#6]=,:[#16]",
@@ -639,15 +644,15 @@
             "[#15](-,:[#8])(=,:[#8])",
             "[#16](-,:[#6])(=,:[#8])",
             "[#16](-,:[#8])(=,:[#8])",
             "[#16](=,:[#8])(=,:[#8])",
         ]
         return self._get_smarts_match_counts(mol, smarts_list)
 
-    def _get_simple_smarts_patterns_counts(self, mol: Mol) -> List[int]:
+    def _get_simple_smarts_patterns_counts(self, mol: Mol) -> list[int]:
         smarts_list = [
             "[#6]-,:[#6]-,:[#6]#[#6]",
             "[#8]-,:[#6]-,:[#6]=,:[#7]",
             "[#8]-,:[#6]-,:[#6]=,:[#8]",
             "[#7]:[#6]-,:[#16]-[#1]",
             "[#7]-,:[#6]-,:[#6]=,:[#6]",
             "[#8]=,:[#16]-,:[#6]-,:[#6]",
@@ -897,15 +902,15 @@
             "[#6]-,:[#6](-,:[#6])-,:[#6]-,:[#6]-,:[#6]",
             "[#6]-,:[#6]-,:[#6](-,:[#6])-,:[#6]-,:[#6]",
             "[#6]-,:[#6](-,:[#6])(-,:[#6])-,:[#6]-,:[#6]",
             "[#6]-,:[#6](-,:[#6])-,:[#6](-,:[#6])-,:[#6]",
         ]
         return self._get_smarts_match_counts(mol, smarts_list)
 
-    def _get_complex_smarts_patterns_counts(self, mol: Mol) -> List[int]:
+    def _get_complex_smarts_patterns_counts(self, mol: Mol) -> list[int]:
         smarts_list = [
             "[#6]c1ccc([#6])cc1",
             "[#6]c1ccc([#8])cc1",
             "[#6]c1ccc([#16])cc1",
             "[#6]c1ccc([#7])cc1",
             "[#6]c1ccc(Cl)cc1",
             "[#6]c1ccc(Br)cc1",
@@ -1070,14 +1075,14 @@
             "[#7][#6]1[#6](Br)[#6][#6][#6]1",
             "Cl[#6]1[#6](Cl)[#6][#6][#6]1",
             "Cl[#6]1[#6](Br)[#6][#6][#6]1",
             "Br[#6]1[#6](Br)[#6][#6][#6]1",
         ]
         return self._get_smarts_match_counts(mol, smarts_list)
 
-    def _get_smarts_match_counts(self, mol: Mol, smarts_list: List[str]) -> List[int]:
+    def _get_smarts_match_counts(self, mol: Mol, smarts_list: list[str]) -> list[int]:
         from rdkit.Chem import MolFromSmarts
 
         return [
             len(mol.GetSubstructMatches(MolFromSmarts(smarts)))
             for smarts in smarts_list
         ]
```

### Comparing `scikit_fingerprints-1.2.0/skfp/validators.py` & `scikit_fingerprints-1.4.0/skfp/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import Any, Sequence
+from collections.abc import Sequence
+from typing import Any
 
-from rdkit.Chem import Mol, MolFromSmiles
+from rdkit.Chem import Mol, MolFromSmiles, MolToSmiles
+from rdkit.Chem.PropertyMol import PropertyMol
 
 
 def ensure_mols(X: Sequence[Any]) -> Sequence[Mol]:
-    if not all(isinstance(x, (Mol, str)) for x in X):
-        raise ValueError("Passed value must be either rdkit.Chem.rdChem.Mol or SMILES")
+    if not all(isinstance(x, (Mol, PropertyMol, str)) for x in X):
+        raise ValueError("Passed values must be either rdkit.Chem.rdChem.Mol or SMILES")
 
     X = [MolFromSmiles(x) if isinstance(x, str) else x for x in X]
     return X
 
 
-def require_smiles(X: Sequence[Any]) -> Sequence[str]:
-    if not all(isinstance(x, str) for x in X):
+def ensure_smiles(X: Sequence[Any]) -> Sequence[str]:
+    if not all(isinstance(x, (Mol, PropertyMol, str)) for x in X):
         raise ValueError("Passed values must be SMILES strings")
+    X = [MolToSmiles(x) if isinstance(x, Mol) else x for x in X]
     return X
 
 
 def require_mols_with_conf_ids(X: Sequence[Any]) -> Sequence[Mol]:
-    if not all(isinstance(x, Mol) and hasattr(x, "conf_id") for x in X):
+    if not all(isinstance(x, (Mol, PropertyMol)) and x.HasProp("conf_id") for x in X):
         raise ValueError(
             "Passed data must be molecules (rdkit.Chem.rdChem.Mol instances) "
-            "and each must have conf_id attribute. You can use "
+            "and each must have conf_id property set. You can use "
             "ConformerGenerator to add them."
         )
     return X
```

### Comparing `scikit_fingerprints-1.2.0/PKG-INFO` & `scikit_fingerprints-1.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-fingerprints
-Version: 1.2.0
+Version: 1.4.0
 Summary: Library for effective molecular fingerprints calculation
 Home-page: https://github.com/Arch4ngel21/scikit-fingerprints
 License: MIT
 Author: Scikit-Fingerprints Development Team
 Author-email: scikitfingerprints@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,73 +12,94 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasketch
 Requires-Dist: e3fp
 Requires-Dist: joblib
+Requires-Dist: mordredcommunity
 Requires-Dist: numpy (>=1.20.0,<2.0.0)
 Requires-Dist: pandas
 Requires-Dist: rdkit
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/Arch4ngel21/scikit-fingerprints
 Description-Content-Type: text/markdown
 
 # scikit-fingerprints
 
 A Python library for efficient computation of molecular fingerprints
 
+Click [HERE](https://scikit-fingerprints.github.io/scikit-fingerprints/) to see the Documentation.
 
 ## Table of Contents
+
 - [Description](#description)
 - [General Project Vision](#general-project-vision)
 - [Library Description](#library-description)
 - [Installation](#installation)
 - [Usage](#usage)
 - [Technologies Used](#technologies-used)
 - [Contributing](#contributing)
 - [License](#license)
 
 ---
 
 ## Description
 
-Molecular fingerprints are crucial in various scientific fields, including drug discovery, materials science, and chemical analysis. However, existing Python libraries for computing molecular fingerprints often lack performance, user-friendliness, and support for modern programming standards. This project aims to address these shortcomings by creating an efficient and accessible Python library for molecular fingerprint computation.
+Molecular fingerprints are crucial in various scientific fields, including drug discovery, materials science, and
+chemical analysis. However, existing Python libraries for computing molecular fingerprints often lack performance,
+user-friendliness, and support for modern programming standards. This project aims to address these shortcomings by
+creating an efficient and accessible Python library for molecular fingerprint computation.
+
+## Supported platforms
+
+|                      | `python3.9`   | `python3.10` | `python3.11` | `python3.12` |
+|----------------------|---------------|--------------|--------------|--------------|
+| **Ubuntu - latest**  | ✅             | ✅            | ✅            | ✅            |
+| **Windows - latest** | ✅             | ✅            | ✅            | ✅            |
+| **macOS - latest**   | only macOS 13 | ✅            | ✅            | ✅            |
 
 ## Installation
 
 You can install the library using pip:
 
 ```bash
 pip install scikit-fingerprints
 ```
 
 ## General Project Vision
- 
-The primary goal of this project was to develop a Python library that simplifies the computation of widely-used molecular fingerprints, such as Morgan's fingerprint, MACCS fingerprint, and others. This library has the following key features:
 
-- **User-Friendly Interface:** The library was designed to provide an intuitive interface, making it easy to integrate into machine learning workflows.
+The primary goal of this project was to develop a Python library that simplifies the computation of widely-used
+molecular fingerprints, such as Morgan's fingerprint, MACCS fingerprint, and others. This library has the following key
+features:
+
+- **User-Friendly Interface:** The library was designed to provide an intuitive interface, making it easy to integrate
+  into machine learning workflows.
 
-- **Performance Optimization:** We implemented molecular fingerprint computation algorithms using concurrent programming techniques to maximize performance. Large datasets of molecules are processed in parallel for improved efficiency.
+- **Performance Optimization:** We implemented molecular fingerprint computation algorithms using concurrent programming
+  techniques to maximize performance. Large datasets of molecules are processed in parallel for improved efficiency.
 
-- **Compatibility:** The library's interface was inspired by popular data science libraries like Scikit-Learn, ensuring compatibility and familiarity for users familiar with these tools.
+- **Compatibility:** The library's interface was inspired by popular data science libraries like Scikit-Learn, ensuring
+  compatibility and familiarity for users familiar with these tools.
 
 - **Extensibility:** Users should be able to customize and extend the library to suit their specific needs.
 
 ## Library Description
 
-- The library offers various functions that accept molecule descriptors (e.g., SMILES) and fingerprint parameters, returning the specified fingerprints.
+- The library offers various functions that accept molecule descriptors (e.g., SMILES) and fingerprint parameters,
+  returning the specified fingerprints.
 - It's open-source and available for installation via pip.
 - The library has been designed for ease of use, minimizing the need for extensive training.
 - Compatibility with the standard Python ML stack, based on Scikit-Learn interfaces, has been a top priority.
 
 ## Contributing
 
-Please read [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details on our code of conduct, and the process for submitting pull requests to us.
+Please read [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details on our code of
+conduct, and the process for submitting pull requests to us.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

