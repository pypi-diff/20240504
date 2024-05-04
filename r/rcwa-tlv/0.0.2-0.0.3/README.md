# Comparing `tmp/rcwa_tlv-0.0.2.tar.gz` & `tmp/rcwa_tlv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcwa_tlv-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rcwa_tlv-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rcwa_tlv-0.0.2.tar` & `rcwa_tlv-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1109 2024-04-24 14:03:13.173831 rcwa_tlv-0.0.2/README.md
--rw-r--r--   0        0        0      776 2024-04-24 14:16:03.310502 rcwa_tlv-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      141 2024-04-29 13:22:45.879796 rcwa_tlv-0.0.2/src/rcwa_tlv/__init__.py
--rw-r--r--   0        0        0      308 2024-04-24 11:08:07.976197 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/device.py
--rw-r--r--   0        0        0       38 2024-04-19 11:41:39.425074 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/normal_fields.py
--rw-r--r--   0        0        0     1762 2024-04-27 15:37:18.813112 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/shapes.py
--rw-r--r--   0        0        0      693 2024-04-24 11:10:05.357323 rcwa_tlv-0.0.2/src/rcwa_tlv/devices/source.py
--rw-r--r--   0        0        0     4146 2024-04-27 04:47:19.202885 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/Si.txt
--rw-r--r--   0        0        0      279 2024-04-27 04:38:11.772145 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/SiO2.txt
--rw-r--r--   0        0        0      370 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/TiO2.txt
--rw-r--r--   0        0        0       57 2024-04-27 05:06:13.312988 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-27 10:24:36.008784 rcwa_tlv-0.0.2/src/rcwa_tlv/materials/materials.py
--rw-r--r--   0        0        0    13637 2024-04-29 13:22:22.967728 rcwa_tlv-0.0.2/src/rcwa_tlv/rcwa.py
--rw-r--r--   0        0        0     1431 2024-04-24 07:00:20.140807 rcwa_tlv-0.0.2/src/rcwa_tlv/utils/convmat.py
--rw-r--r--   0        0        0      598 2024-04-27 16:10:11.507347 rcwa_tlv-0.0.2/src/rcwa_tlv/utils/normal_vector.py
--rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 rcwa_tlv-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1147 2024-05-04 08:13:51.358007 rcwa_tlv-0.0.3/README.md
+-rw-r--r--   0        0        0      776 2024-04-24 14:16:03.310502 rcwa_tlv-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      141 2024-05-04 12:49:47.474620 rcwa_tlv-0.0.3/src/rcwa_tlv/__init__.py
+-rw-r--r--   0        0        0      308 2024-04-24 11:08:07.976197 rcwa_tlv-0.0.3/src/rcwa_tlv/devices/device.py
+-rw-r--r--   0        0        0       38 2024-04-19 11:41:39.425074 rcwa_tlv-0.0.3/src/rcwa_tlv/devices/normal_fields.py
+-rw-r--r--   0        0        0     1762 2024-04-27 15:37:18.813112 rcwa_tlv-0.0.3/src/rcwa_tlv/devices/shapes.py
+-rw-r--r--   0        0        0      693 2024-04-24 11:10:05.357323 rcwa_tlv-0.0.3/src/rcwa_tlv/devices/source.py
+-rw-r--r--   0        0        0     4146 2024-04-27 04:47:19.202885 rcwa_tlv-0.0.3/src/rcwa_tlv/materials/Si.txt
+-rw-r--r--   0        0        0      279 2024-04-27 04:38:11.772145 rcwa_tlv-0.0.3/src/rcwa_tlv/materials/SiO2.txt
+-rw-r--r--   0        0        0      370 2023-11-21 15:43:58.000000 rcwa_tlv-0.0.3/src/rcwa_tlv/materials/TiO2.txt
+-rw-r--r--   0        0        0       57 2024-04-27 05:06:13.312988 rcwa_tlv-0.0.3/src/rcwa_tlv/materials/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-27 10:24:36.008784 rcwa_tlv-0.0.3/src/rcwa_tlv/materials/materials.py
+-rw-r--r--   0        0        0    20284 2024-05-04 11:53:34.355902 rcwa_tlv-0.0.3/src/rcwa_tlv/rcwa.py
+-rw-r--r--   0        0        0     1431 2024-05-03 13:58:47.418523 rcwa_tlv-0.0.3/src/rcwa_tlv/utils/convmat.py
+-rw-r--r--   0        0        0      698 2024-05-04 11:47:59.421206 rcwa_tlv-0.0.3/src/rcwa_tlv/utils/normal_vector.py
+-rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 rcwa_tlv-0.0.3/PKG-INFO
```

### Comparing `rcwa_tlv-0.0.2/README.md` & `rcwa_tlv-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 rcwa = RCWA(device, source, gamma=0.7, apply_nv=False, dtype=np.float32)
 
 result = rcwa()
 
 ```
 
 ## References:
-
+https://doi.org/10.1364/JOSA.71.000811
```

### Comparing `rcwa_tlv-0.0.2/pyproject.toml` & `rcwa_tlv-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/devices/shapes.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/devices/shapes.py`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/devices/source.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/devices/source.py`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/materials/Si.txt` & `rcwa_tlv-0.0.3/src/rcwa_tlv/materials/Si.txt`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/materials/materials.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/materials/materials.py`

 * *Files identical despite different names*

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/rcwa.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/rcwa.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,31 +12,28 @@
     def __init__(
             self,
             device: Device,
             source: Source,
             gamma: float = 1.,
             apply_nv: bool = False,
             dtype: Literal['np.float32', 'np.float64'] = np.float32,
-            renormalize: bool = True,
+            renormalize: bool = False,
     ):
         self.source = source
         self.device = device
         self.gamma = gamma
         self.apply_nv = apply_nv
         self.renormalize = renormalize
         self.result = None
 
         self.dtype = dtype
         self.cdtype = np.complex128 if dtype == np.float64 else np.complex64
         self.idtype = np.int64 if dtype == np.float64 else np.int32
 
-        # if apply_nv:
-        #     raise NotImplementedError("NV is not yet implemented.")
-
-    def __call__(self, *args, apply_nv=None, **kwargs) -> dict:
+    def __call__(self, *args, apply_nv=None, verbose=True, **kwargs) -> dict:
         ur1 = self.device.ur1
         er1 = self.device.er1
         ur2 = self.device.ur2
         er2 = self.device.er2
         gamma = self.gamma
         polarization_vec = self.source.polarization_vec
         self.apply_nv = apply_nv if apply_nv is not None else self.apply_nv
@@ -128,38 +125,32 @@
             1j * (k_inc[2] * polarization_vec[1] - k_inc[1] * polarization_vec[2]) * delta / self.device.ur1,
             1j * (k_inc[0] * polarization_vec[2] - k_inc[2] * polarization_vec[0]) * delta / self.device.ur1
         ]).astype(self.cdtype)
 
         # Initialize matrices
         i_mat = np.diag(np.ones(n_nonzero, dtype=self.cdtype))
         o_mat = np.diag(np.zeros(n_nonzero, dtype=self.cdtype))
-        a_mat = np.block([  # type:ignore
-            [i_mat, o_mat],
-            [o_mat, i_mat],
-            [
-                -(1j * kx_mat @ ky_mat) @ np.linalg.inv(ur1 * kz_ref_mat),
-                -(1j * (ky_mat ** 2 + kz_ref_mat ** 2)) @ np.linalg.inv(ur1 * kz_ref_mat)
-            ],
-            [
-                (1j * (kx_mat ** 2 + kz_ref_mat ** 2)) @ np.linalg.inv(ur1 * kz_ref_mat),
-                (1j * kx_mat @ ky_mat) @ np.linalg.inv(ur1 * kz_ref_mat)
-            ]
-        ])
-        b_mat = np.block([  # type:ignore
-            [i_mat, o_mat],
-            [o_mat, i_mat],
-            [
-                (1j * kx_mat @ ky_mat) @ np.linalg.inv(ur2 * kz_trn_mat),
-                (1j * (ky_mat ** 2 + kz_trn_mat ** 2)) @ np.linalg.inv(ur2 * kz_trn_mat)
-            ],
-            [
-                -(1j * (kx_mat ** 2 + kz_trn_mat ** 2)) @ np.linalg.inv(ur2 * kz_trn_mat),
-                -(1j * kx_mat @ ky_mat) @ np.linalg.inv(ur2 * kz_trn_mat)
-            ]
-        ])
+
+        # prepare mid-way calculations to save time
+        kxky_mat = kx_mat @ ky_mat
+        kykx_mat = ky_mat @ kx_mat
+        kxkx_mat = kx_mat @ kx_mat
+        kyky_mat = ky_mat @ ky_mat
+        j_kxky_mat = 1j * kxky_mat
+        kx_sqr_mat = kx_mat ** 2
+        ky_sqr_mat = ky_mat ** 2
+        kz_ref_sqr_mat = kz_ref_mat ** 2
+        kz_trn_sqr_mat = kz_trn_mat ** 2
+
+        a_mat = self._a_mat(
+            ur1, i_mat, o_mat, j_kxky_mat, kz_ref_mat, ky_sqr_mat, kx_sqr_mat, kz_ref_sqr_mat, verbose=verbose
+        )
+        b_mat = self._b_mat(
+            ur2, i_mat, o_mat, j_kxky_mat, kz_trn_mat, ky_sqr_mat, kx_sqr_mat, kz_trn_sqr_mat, verbose=verbose
+        )
 
         f_mat = np.zeros((4 * n_nonzero, 4 * n_nonzero, n_layers), dtype=self.cdtype)
         x_mat = np.zeros((2 * n_nonzero, 2 * n_nonzero, n_layers), dtype=self.cdtype)
         p_mat = np.zeros((2 * n_nonzero, 2 * n_nonzero, n_layers), dtype=self.cdtype)
         q_mat = np.zeros((2 * n_nonzero, 2 * n_nonzero, n_layers), dtype=self.cdtype)
 
         # Compute matrices for each layer
@@ -172,26 +163,26 @@
                     [kx_mat @ erky, i_mat - kx_mat @ erkx],
                     [ky_mat @ erky - i_mat, -ky_mat @ erkx]
                 ])
                 if self.apply_nv:
                     delta_nxy = delta_mat[i_layer] @ nvxy_c[i_layer]
                     q_mat[:, :, i_layer] = np.block([  # type:ignore
                         [
-                            kx_mat @ ky_mat - delta_nxy,
-                            er_c_mat[i_layer] - delta_mat[i_layer] @ nvy_c[i_layer] - kx_mat @ kx_mat
+                            kxky_mat - delta_nxy,
+                            er_c_mat[i_layer] - delta_mat[i_layer] @ nvy_c[i_layer] - kxkx_mat
                         ],
                         [
-                            ky_mat @ ky_mat - er_c_mat[i_layer] + delta_mat[i_layer] @ nvx_c[i_layer],
-                            -ky_mat @ kx_mat + delta_nxy
+                            kyky_mat - er_c_mat[i_layer] + delta_mat[i_layer] @ nvx_c[i_layer],
+                            -kykx_mat + delta_nxy
                         ]
                     ])
                 else:
                     q_mat[:, :, i_layer] = np.block([  # type:ignore
-                        [kx_mat @ ky_mat, er_c_mat[i_layer] - kx_mat @ kx_mat],
-                        [ky_mat @ ky_mat - er_c_mat[i_layer], -ky_mat @ kx_mat]
+                        [kxky_mat, er_c_mat[i_layer] - kxkx_mat],
+                        [kyky_mat - er_c_mat[i_layer], -kykx_mat]
                     ])
                 omega_2 = p_mat[:, :, i_layer] @ q_mat[:, :, i_layer]
                 lam, w_mat = np.linalg.eig(omega_2)
                 lam = np.diag(np.sqrt(lam))
                 x_mat[:, :, i_layer] = expm(-lam * k0 * self.device.layers[i_layer]['length_z'])
                 v_mat = q_mat[:, :, i_layer] @ w_mat @ np.linalg.inv(lam)
                 f_mat[:, :, i_layer] = np.block([  # type:ignore
@@ -247,18 +238,31 @@
         # Compute r and t
         txy = t1
         for i_layer in range(n_layers):
             txy = np.linalg.solve(a[:, :, i_layer], x_mat[:, :, i_layer]) @ txy
 
         r[:, 0] = rxy[:n_nonzero]
         r[:, 1] = rxy[n_nonzero:]
-        r[:, 2] = -np.linalg.solve(kz_ref_mat, kx_mat @ r[:, 0] + ky_mat @ r[:, 1])
+
+        try:
+            r[:, 2] = -np.linalg.solve(kz_ref_mat, kx_mat @ r[:, 0] + ky_mat @ r[:, 1])
+        except np.linalg.linalg.LinAlgError:
+            if verbose:
+                print('failed: -np.linalg.solve(kz_ref_mat, kx_mat @ r[:, 0] + ky_mat @ r[:, 1]), trying lstsq')
+            r[:, 2] = -np.linalg.lstsq(kz_ref_mat, kx_mat @ r[:, 0] + ky_mat @ r[:, 1], rcond=None)[0]
+
         t[:, 0] = txy[:n_nonzero]
         t[:, 1] = txy[n_nonzero:]
-        t[:, 2] = -np.linalg.solve(kz_trn_mat, kx_mat @ t[:, 0] + ky_mat @ t[:, 1])
+
+        try:
+            t[:, 2] = -np.linalg.solve(kz_trn_mat, kx_mat @ t[:, 0] + ky_mat @ t[:, 1])
+        except np.linalg.linalg.LinAlgError:
+            if verbose:
+                print('failed: -np.linalg.solve(kz_trn_mat, kx_mat @ t[:, 0] + ky_mat @ t[:, 1]), trying lstsq')
+            t[:, 2] = -np.linalg.lstsq(kz_trn_mat, kx_mat @ t[:, 0] + ky_mat @ t[:, 1], rcond=None)[0]
 
         # Compute diffraction efficiency
         r_squared = np.abs(r[:, 0]) ** 2 + np.abs(r[:, 1]) ** 2 + np.abs(r[:, 2]) ** 2
         t_squared = np.abs(t[:, 0]) ** 2 + np.abs(t[:, 1]) ** 2 + np.abs(t[:, 2]) ** 2
 
         reflectance = np.real(kz_ref_mat / ur1) / np.real(k_inc[2] / ur1) @ r_squared
         transmittance = np.real(kz_trn_mat / ur2) / np.real(k_inc[2] / ur1) @ t_squared
@@ -280,21 +284,174 @@
             'transmittance': transmittance,
             'tot_r': tot_r,
             'tot_t': tot_t,
         }
 
         return self.result
 
+    @staticmethod
+    def _a_mat(ur1, i_mat, o_mat, j_kxky_mat, kz_ref_mat, ky_sqr_mat, kx_sqr_mat, kz_ref_sqr_mat, verbose=True):
+        """
+        a_mat = np.block([  # type:ignore
+            [i_mat, o_mat],
+            [o_mat, i_mat],
+            [
+                -(1j * kx_mat @ ky_mat) @ np.linalg.inv(ur1 * kz_ref_mat),
+                -(1j * (ky_mat ** 2 + kz_ref_mat ** 2)) @ np.linalg.inv(ur1 * kz_ref_mat)
+            ],
+            [
+                (1j * (kx_mat ** 2 + kz_ref_mat ** 2)) @ np.linalg.inv(ur1 * kz_ref_mat),
+                (1j * kx_mat @ ky_mat) @ np.linalg.inv(ur1 * kz_ref_mat)
+            ]
+        ])
+        :param ur1:
+        :param i_mat:
+        :param o_mat:
+        :param j_kxky_mat:
+        :param kz_ref_mat:
+        :param ky_sqr_mat:
+        :param kx_sqr_mat:
+        :param kz_ref_sqr_mat:
+        :param verbose:
+        :return:
+        """
+        ur1_kz_ref_mat = ur1 * kz_ref_mat
+
+        try:
+            kz_inv_mat = np.linalg.inv(ur1_kz_ref_mat)
+            j_kxky_kz_inv_mat = j_kxky_mat @ kz_inv_mat
+
+            a_mat = np.block([  # type:ignore
+                [i_mat, o_mat],
+                [o_mat, i_mat],
+                [-j_kxky_kz_inv_mat, -(1j * (ky_sqr_mat + kz_ref_sqr_mat)) @ kz_inv_mat],
+                [(1j * (kx_sqr_mat + kz_ref_sqr_mat)) @ kz_inv_mat, j_kxky_kz_inv_mat]
+            ])
+        except np.linalg.linalg.LinAlgError:
+            try:
+                if verbose:
+                    print(f'direct inversion of ur1 * kz_ref_mat failed, trying to use np.linalg.solve...')
+
+                a_mat = np.block([  # type:ignore
+                    [i_mat, o_mat],
+                    [o_mat, i_mat],
+                    [
+                        np.linalg.solve(ur1_kz_ref_mat.T, -j_kxky_mat.T).T,
+                        np.linalg.solve(ur1_kz_ref_mat.T, -(1j * (ky_sqr_mat + kz_ref_sqr_mat)).T).T
+                    ],
+                    [
+                        np.linalg.solve(ur1_kz_ref_mat.T, (1j * (kx_sqr_mat + kz_ref_sqr_mat)).T).T,
+                        np.linalg.solve(ur1_kz_ref_mat.T, j_kxky_mat.T).T
+                    ]
+                ])
+            except np.linalg.linalg.LinAlgError:
+                try:
+                    if verbose:
+                        print(f'np.linalg.solve failed, trying np.linalg.lstsq...')
+                    a_mat = np.block([  # type:ignore
+                        [i_mat, o_mat],
+                        [o_mat, i_mat],
+                        [
+                            np.linalg.lstsq(ur1_kz_ref_mat.T, -j_kxky_mat.T, rcond=None)[0].T,
+                            np.linalg.lstsq(ur1_kz_ref_mat.T, -(1j * (ky_sqr_mat + kz_ref_sqr_mat)).T, rcond=None)[0].T
+                        ],
+                        [
+                            np.linalg.lstsq(ur1_kz_ref_mat.T, (1j * (kx_sqr_mat + kz_ref_sqr_mat)).T, rcond=None)[0].T,
+                            np.linalg.lstsq(ur1_kz_ref_mat.T, j_kxky_mat.T, rcond=None)[0].T
+                        ]
+                    ])
+                except np.linalg.linalg.LinAlgError:
+                    raise np.linalg.linalg.LinAlgError('all methods to evaluate a_mat failed')
+
+        return a_mat
+
+    @staticmethod
+    def _b_mat(ur2, i_mat, o_mat, j_kxky_mat, kz_trn_mat, ky_sqr_mat, kx_sqr_mat, kz_trn_sqr_mat, verbose=True):
+        """
+        b_mat = np.block([  # type:ignore
+            [i_mat, o_mat],
+            [o_mat, i_mat],
+            [
+                j_kxky_mat @ np.linalg.inv(ur2 * kz_trn_mat),
+                (1j * (ky_sqr_mat + kz_trn_sqr_mat)) @ np.linalg.inv(ur2 * kz_trn_mat)
+            ],
+            [
+                -(1j * (kx_sqr_mat + kz_trn_sqr_mat)) @ np.linalg.inv(ur2 * kz_trn_mat),
+                -j_kxky_mat @ np.linalg.inv(ur2 * kz_trn_mat)
+            ]
+        ])
+        :param ur2:
+        :param i_mat:
+        :param o_mat:
+        :param j_kxky_mat:
+        :param kz_trn_mat:
+        :param ky_sqr_mat:
+        :param kx_sqr_mat:
+        :param kz_trn_sqr_mat:
+        :param verbose:
+        :return:
+        """
+
+        ur2_kz_trn_mat = ur2 * kz_trn_mat
+
+        try:
+            kz_inv_mat = np.linalg.inv(ur2_kz_trn_mat)
+            j_kxky_kz_inv_mat = j_kxky_mat @ kz_inv_mat
+
+            b_mat = np.block([  # type:ignore
+                [i_mat, o_mat],
+                [o_mat, i_mat],
+                [j_kxky_kz_inv_mat, (1j * (ky_sqr_mat + kz_trn_sqr_mat)) @ kz_inv_mat],
+                [-(1j * (kx_sqr_mat + kz_trn_sqr_mat)) @ kz_inv_mat, -j_kxky_kz_inv_mat]
+            ])
+        except np.linalg.linalg.LinAlgError:
+            try:
+                if verbose:
+                    print(f'direct inversion of ur1 * kz_ref_mat failed, trying to use np.linalg.solve...')
+
+                b_mat = np.block([  # type:ignore
+                    [i_mat, o_mat],
+                    [o_mat, i_mat],
+                    [
+                        np.linalg.solve(ur2_kz_trn_mat.T, j_kxky_mat.T).T,
+                        np.linalg.solve(ur2_kz_trn_mat.T, (1j * (ky_sqr_mat + kz_trn_sqr_mat)).T).T
+                    ],
+                    [
+                        np.linalg.solve(ur2_kz_trn_mat.T, -(1j * (kx_sqr_mat + kz_trn_sqr_mat)).T).T,
+                        np.linalg.solve(ur2_kz_trn_mat.T, -j_kxky_mat.T).T
+                    ]
+                ])
+            except np.linalg.linalg.LinAlgError:
+                try:
+                    if verbose:
+                        print(f'np.linalg.solve failed, trying np.linalg.lstsq...')
+                    b_mat = np.block([  # type:ignore
+                        [i_mat, o_mat],
+                        [o_mat, i_mat],
+                        [
+                            np.linalg.lstsq(ur2_kz_trn_mat.T, j_kxky_mat.T, rcond=None)[0].T,
+                            np.linalg.lstsq(ur2_kz_trn_mat.T, (1j * (ky_sqr_mat + kz_trn_sqr_mat)).T, rcond=None)[0].T
+                        ],
+                        [
+                            np.linalg.lstsq(ur2_kz_trn_mat.T, -(1j * (kx_sqr_mat + kz_trn_sqr_mat)).T, rcond=None)[0].T,
+                            np.linalg.lstsq(ur2_kz_trn_mat.T, -j_kxky_mat.T, rcond=None)[0].T
+                        ]
+                    ])
+                except np.linalg.linalg.LinAlgError:
+                    raise np.linalg.linalg.LinAlgError('all methods to evaluate b_mat failed')
+
+        return b_mat
+
 
 if __name__ == '__main__':
     from time import perf_counter
     from rcwa_tlv.devices.shapes import add_circle
 
-    n_height = 400
-    n_width = 400
+    n_height = 800
+    n_width = 800
     period = 900
     nm2pixels = n_width / period
 
     # reflexion region
     er1 = 1.5 ** 2
     ur1 = 1.0
 
@@ -310,23 +467,24 @@
 
     layer_2 = {
         'er': 7.0 * np.ones((n_height, n_width)),
         # 'ur': 1.0 * np.ones((n_height, n_width)),
         'length_z': 54,
     }
 
-    layers = [layer_1, layer_2]
-    add_circle(layers[0]['er'], (n_height // 2, n_width // 2), 300 * nm2pixels, er1)
-    add_circle(layers[1]['er'], (n_height // 4, n_width // 2), 200 * nm2pixels, er1)
+    # layers = [layer_1, layer_2, layer_2, layer_2, layer_1, layer_2, layer_2, layer_2]
+    layers = [layer_1]
+    add_circle(layers[0]['er'], (n_height // 2, n_width // 2), 300 * nm2pixels, 36.)
+    # add_circle(layers[1]['er'], (n_height // 4, n_width // 2), 200 * nm2pixels, er1)
 
-    device_1 = Device(layers, period_x=period, period_y=period, er1=1.445 ** 2, ur1=1.0, er2=1.0, ur2=1.0, p=11, q=11)
-    source_1 = Source(0.0, 0.0, 700, 1., 0.)
+    device_1 = Device(layers, period_x=period, period_y=period, er1=1.445 ** 2, ur1=1.0, er2=1.0, ur2=1.0, p=9, q=9)
+    source_1 = Source(0.0, 0.0, 400, 1., 0.)
 
-    rcwa = RCWA(device_1, source_1, gamma=0.7, apply_nv=False, dtype=np.float32)
+    rcwa = RCWA(device_1, source_1, gamma=1.0, apply_nv=True, dtype=np.float32)
 
     t1 = perf_counter()
-    rcwa()
+    result = rcwa()
     t2 = perf_counter()
 
-    print(f'rcwa time: {t2 - t1:0.4f}')
+    print(f'rcwa time: {t2 - t1:0.4f}, r: {result["tot_r"]}, t: {result["tot_t"]}')
 
     b = 1
```

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/utils/convmat.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/utils/convmat.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,20 @@
 
     # COMPUTE ARRAY INDICES OF CENTER HARMONIC
     p0 = (nx // 2)
     q0 = (ny // 2)
 
     # x domain:
     x = np.arange(p0, p0 - p, -1)
-    x = np.tile(x[np.newaxis, :], (1, p))
+    x = np.tile(x[np.newaxis, :], (1, q))
     xp = np.arange(p)
     x = x + xp[:, np.newaxis]
-    x = np.tile(x, (p, 1))
+    x = np.tile(x, (q, 1))
 
     # y domain:
     a = np.arange(q)
     y = toeplitz(a, -a)
-    y = np.repeat(np.repeat(y, q, axis=0), q, axis=1) + q0
+    y = np.repeat(np.repeat(y, p, axis=0), p, axis=1) + q0
 
     conv_matrix = matrix_in_fft[y, x]
 
     return conv_matrix
```

### Comparing `rcwa_tlv-0.0.2/src/rcwa_tlv/utils/normal_vector.py` & `rcwa_tlv-0.0.3/src/rcwa_tlv/utils/normal_vector.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 import numpy as np
 
 
 def calc_edges_diffs(img, axis=1):
 
-    diff = np.diff(img, axis=axis)
-    nv = np.zeros_like(img, dtype=np.float32)
-    vectors = np.where(diff == 0, 0, 1 / np.sqrt(2))
-
     if axis == 0:
-        nv[:-1, :] += vectors
-        nv[1:, :] += vectors
+        nv = np.roll(img, shift=1, axis=0) - img
+        nv += img - np.roll(img, shift=-1, axis=0)
     elif axis == 1:
-        nv[:, :-1] += vectors
-        nv[:, 1:] += vectors
+        nv = np.roll(img, shift=1, axis=1) - img
+        nv += img - np.roll(img, shift=-1, axis=1)
     else:
         raise ValueError('axis must be 0 or 1')
 
     return nv
 
 
 def calc_nv_fields(layer):
     abs_layer = np.abs(layer)
     nv_x = calc_edges_diffs(abs_layer, axis=1)
     nv_y = calc_edges_diffs(abs_layer, axis=0)
 
+    norm = np.sqrt(nv_x ** 2 + nv_y ** 2)
+    nv_x = np.where(np.abs(nv_x) > 0, nv_x / norm, 0.)
+    nv_y = np.where(np.abs(nv_y) > 0, nv_y / norm, 0.)
+
     return nv_x, nv_y
```

### Comparing `rcwa_tlv-0.0.2/PKG-INFO` & `rcwa_tlv-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcwa_tlv
-Version: 0.0.2
+Version: 0.0.3
 Summary: RCWA solver for photonic devices
 Author-email: Victor Egorov <victoregorov23@gmail.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -66,9 +66,9 @@
 rcwa = RCWA(device, source, gamma=0.7, apply_nv=False, dtype=np.float32)
 
 result = rcwa()
 
 ```
 
 ## References:
-
+https://doi.org/10.1364/JOSA.71.000811
```

