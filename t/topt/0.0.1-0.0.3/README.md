# Comparing `tmp/topt-0.0.1.tar.gz` & `tmp/topt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topt-0.0.1.tar", max compression
+gzip compressed data, was "topt-0.0.3.tar", max compression
```

## Comparing `topt-0.0.1.tar` & `topt-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0    11358 2024-05-03 03:21:01.771066 topt-0.0.1/LICENSE
--rw-r--r--   0        0        0       90 2024-05-03 03:26:31.931702 topt-0.0.1/README.md
--rw-r--r--   0        0        0     3804 2024-05-03 03:21:16.259919 topt-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      180 2024-05-03 03:18:20.778706 topt-0.0.1/topt/__init__.py
--rw-r--r--   0        0        0     1129 2024-05-03 03:18:44.707462 topt-0.0.1/topt/converter.py
--rw-r--r--   0        0        0    16382 2024-05-03 03:25:16.066475 topt-0.0.1/topt/optimizer.py
--rw-r--r--   0        0        0        0 2024-05-03 03:02:35.695303 topt-0.0.1/topt/py.typed
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 topt-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-03 03:21:01.771066 topt-0.0.3/LICENSE
+-rw-r--r--   0        0        0       89 2024-05-03 03:47:21.050827 topt-0.0.3/README.md
+-rw-r--r--   0        0        0     3851 2024-05-04 19:59:18.166274 topt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-05-03 03:18:20.778706 topt-0.0.3/topt/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-04 15:04:06.690779 topt-0.0.3/topt/converter.py
+-rw-r--r--   0        0        0      680 2024-05-04 15:22:24.553666 topt-0.0.3/topt/converter_test.py
+-rw-r--r--   0        0        0    16879 2024-05-04 20:01:13.252775 topt-0.0.3/topt/optimizer.py
+-rw-r--r--   0        0        0     8135 2024-05-04 19:58:36.576443 topt-0.0.3/topt/optimizer_test.py
+-rw-r--r--   0        0        0        0 2024-05-03 03:02:35.695303 topt-0.0.3/topt/py.typed
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 topt-0.0.3/PKG-INFO
```

### Comparing `topt-0.0.1/LICENSE` & `topt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topt-0.0.1/pyproject.toml` & `topt-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "topt"
-version = "0.0.1"
+version = "0.0.3"
 description = "Tools for optimizing trajectories with direct collocation."
 license = "Apache-2.0"
 authors = ["Michael A. Perlin <mika.perlin@gmail.com>"]
 readme = "README.md"
+repository = "https://github.com/perlinm/topt"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "Natural Language :: English",
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Scientific/Engineering :: Physics",
 ]
```

### Comparing `topt-0.0.1/topt/converter.py` & `topt-0.0.3/topt/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-"""
-Methods to convert complex-valued arrays into their real-valued counterparts.
+"""Methods to convert complex-valued arrays into their real-valued counterparts.
 
 Vector: v = v_R + i v_I --> [ v_R, v_I ]
 
 Matrix: M = M_R + i M_I --> ⌈ M_R, -M_I ⌉
                             ⌊ M_I,  M_R ⌋
 
-So that: M @ v = (M_R @ v_R - M_I @ v_I) + i (M_I v_R + M_R v_I)
+So that: M v = (M_R v_R - M_I v_I) + i (M_I v_R + M_R v_I)
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import jax.numpy as np
```

### Comparing `topt-0.0.1/topt/optimizer.py` & `topt-0.0.3/topt/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,22 +31,23 @@
 SplitParamFunc = Callable[[ArrayLike, Array, Array], Array]
 
 
 def optimize_trajectory(
     initial_state: Array,
     initial_params: Array,
     generator: Callable[[ArrayLike, Array, Array], Array],
-    time_span: float | tuple[float, float, float],
+    time_span: float,
     num_time_steps: int,
     objective: SplitTrajectoryFunc,
     *constraints: SplitTrajectoryFunc | tuple[SplitTrajectoryFunc, ArrayLike, ArrayLike],
     num_static_params: int = 0,
     objective_grad: SplitTrajectoryFunc | None = None,
     objective_hess: SplitTrajectoryFunc | None = None,
     generator_jac: SplitParamFunc | None = None,
+    time_bounds: tuple[float, float] | None = None,
     tol: float = 1e-4,  # error tolerance passed to IPOPT
 ) -> scipy.optimize.OptimizeResult:
     """Optimize a trajectory with direct collocation.
 
     This method represets a trajectory by discretizing time, and storing a vector (state, control
     parameters, etc.) at each time point.  Optimization constraints enforce that neighboring
     vectors in time satisfy linear equations of motion.  These dynamical constraints, together with
@@ -61,31 +62,30 @@
         time_span: the total time for which to evolve, either as a fixed value or a tuple that
             specifies (initial_value, lower_bound, upper_bound).
         num_time_steps: number of time steps with which to discretize the trajectory.
         objective: an objective function (to be minimized) of the entire trajectory.
         constraints (optional): additional constraints to enforce for the trajectory.  Each
             constraint may be specified as a function that must equal zero, or as a tuple that
             specifies (function, lower_bounds, upper_bounds).
-        num_static_params (optional): the number of static (not-time-varying) parameters.
+        num_static_params: the number of static (not-time-varying) parameters.
         objective_grad: the gradient of the objective function.
         objective_hess: the hessian of the objective function.
         generator_jac: the jacobian of the generator of time evolution.
+        time_bounds: lower and upper bounds on the allowed time span.  If bounds are not
+            provided, the time span is constrained to a fixed value.
         tol: an error tolerance passed to IPOPT.
 
     The objective and constraint functions must both accept four arrays corresponding to
         (state, dynamic_params, static_params, time_span).
     These functions must likewise return an array.
     """
     num_dynamic_params = initial_params.size - num_static_params
-    if isinstance(time_span, float):
-        time_lb = time_ub = time_span
-    else:
-        time_span, time_lb, time_ub = time_span
+    time_lb, time_ub = time_bounds if time_bounds is not None else (time_span, time_span)
 
-    # build initial trajectory
+    # build an initial trajectory that satisfies equations of motion
     initial_trajectory = build_trajectory(
         initial_state, initial_params, generator, time_span, num_time_steps, num_static_params
     )
 
     # collect objective function, constraint functions, and derivatives thereof
     splitter = functools.partial(
         split_trajectory,
@@ -176,25 +176,31 @@
 def build_trajectory(
     initial_state: Array,
     params: Array,
     generator: Callable[[ArrayLike, Array, Array], Array],
     time_span: ArrayLike,
     num_time_steps: int,
     num_static_params: int,
+    *,
+    rtol: float = 1e-3,  # default for scipy.integrate.solve_ivp
+    atol: float = 1e-6,  # default for scipy.integrate.solve_ivp
 ) -> Array:
     """Build the trajectory of a state satisfying equations of motion."""
     num_dynamic_params = params.size - num_static_params
     dynamic_params = params[:num_dynamic_params]
     static_params = params[num_dynamic_params:]
 
+    times = np.linspace(0, time_span, num_time_steps + 1)[1:]
     result = scipy.integrate.solve_ivp(
         lambda time, state: generator(time, dynamic_params, static_params) @ state,
-        (0, time_span),
+        (0, times[-1]),
         initial_state,
-        t_eval=np.linspace(0, time_span, num_time_steps + 1)[1:],
+        t_eval=times,
+        rtol=rtol,
+        atol=atol,
     )
     states = result.y.T
 
     dynamic_params = np.broadcast_to(dynamic_params, (num_time_steps, num_dynamic_params))
     time_span = np.array([time_span])
     return np.concatenate([states.ravel(), dynamic_params.ravel(), static_params, time_span])
 
@@ -215,48 +221,44 @@
     )
 
 
 def get_derivatives(
     function: SplitTrajectoryFunc,
     splitter: Callable[[Array], tuple[Array, Array, Array, Array]],
     *,
-    forward_mode: bool = False,
     jac: SplitTrajectoryFunc | None = None,
     hess: SplitTrajectoryFunc | None = None,
 ) -> dict[str, Callable[[Array], Array]]:
     """Compile a function of all trajectory data, as well as its derivatives."""
 
     def with_full_trajectory(function: SplitTrajectoryFunc) -> Callable[[Array], Array]:
         return lambda trajectory: function(*splitter(trajectory))
 
     _function = with_full_trajectory(function)
-    if jac is not None:
-        _function_jac = with_full_trajectory(jac)
-    else:
-        jax_jac = jax.jacfwd if forward_mode else jax.jacrev
-        _function_jac = jax_jac(_function)  # type:ignore[operator]
-    if hess is not None:
-        _function_hess = with_full_trajectory(hess)
-    else:
-        _function_hess = jax.jacrev(_function)
+    _function_jac = with_full_trajectory(jac) if jac is not None else jax.jacrev(_function)
+    _function_hess = (
+        with_full_trajectory(hess)
+        if hess is not None
+        else jax.jacrev(_function_jac)  # type:ignore[arg-type]
+    )
     return {
         "fun": jax.jit(_function),
-        "jac": jax.jit(_function_jac),
-        "hess": jax.jit(_function_hess),
+        "jac": jax.jit(_function_jac),  # type:ignore[arg-type]
+        "hess": jax.jit(_function_hess),  # type:ignore[arg-type]
     }
 
 
 def get_dynamical_constraints(
     initial_state: Array,
     generator: Callable[[ArrayLike, Array, Array], Array],
     num_time_steps: int,
     num_dynamic_params: int,
     num_static_params: int,
     generator_jac: SplitParamFunc | None = None,
-) -> dict[str, Callable[[Array], ArrayLike]]:
+) -> dict[str, Callable[[Array], Array]]:
     """Build constraints (and derivatives thereof) induced by equations of motion."""
     state_dim = initial_state.size
     states_size = state_dim * num_time_steps
     dynamic_params_size = num_dynamic_params * num_time_steps
     trajectory_size = states_size + dynamic_params_size + num_static_params + 1
 
     # function to split a trajectory into its components
@@ -291,28 +293,16 @@
             )
             for ss in range(1, num_time_steps)
         ]
 
         return np.concatenate([constraints_init, np.array(constraints_bulk).ravel()])
 
     # compute the jacobian of the generator, if necessary
-
     if generator_jac is None:
-
-        def flat_generator(data: Array) -> Array:
-            time = data[0]
-            dynamic_params = data[1:] if not num_static_params else data[1:-num_static_params]
-            static_params = data[-num_static_params:]
-            return generator(time, dynamic_params, static_params).ravel()
-
-        flat_generator_jac = jax.jacfwd(flat_generator)
-
-        def generator_jac(time: ArrayLike, dynamic_params: Array, static_params: Array) -> Array:
-            time = np.array(time, ndmin=1)
-            return flat_generator_jac(np.concatenate([time, dynamic_params, static_params]))
+        generator_jac = get_generator_jac(generator, num_static_params)
 
     # identify columns of the constraint jacobian that are occupied by data at a certain time index
 
     def get_jacobian_cols(time_index: int) -> Array:
         state_cols = np.arange(state_dim * (time_index - 1), state_dim * (time_index + 1))
         dynamic_param_cols = np.arange(
             states_size + num_dynamic_params * time_index,
@@ -364,18 +354,36 @@
             blocks.append(mat)
 
         return np.vstack(blocks)
 
     return {
         "fun": jax.jit(constraints),
         "jac": jax.jit(jacobian),
-        "hess": lambda _: 0,
+        "hess": jax.jit(jax.jacrev(jacobian)),
     }
 
 
+def get_generator_jac(generator: SplitParamFunc, num_static_params: int) -> SplitParamFunc:
+    """The Jacobian of a generator function."""
+
+    def flat_generator(data: Array) -> Array:
+        time = data[0]
+        dynamic_params = data[1:] if not num_static_params else data[1:-num_static_params]
+        static_params = data[-num_static_params:]
+        return generator(time, dynamic_params, static_params).ravel()
+
+    flat_generator_jac = jax.jacfwd(flat_generator)
+
+    def generator_jac(time: ArrayLike, dynamic_params: Array, static_params: Array) -> Array:
+        time = np.array(time, ndmin=1)
+        return flat_generator_jac(np.concatenate([time, dynamic_params, static_params]))
+
+    return generator_jac
+
+
 def get_time_step_constraint(
     state_init: Array, state_step: Array, generator: Array, time_step: ArrayLike
 ) -> Array:
     """Get the constraint enforcing time evolution by a single time step.
 
     Time evolution is nominally disretized with
         state_step = exp(time_step * generator) @ state_init.
@@ -414,14 +422,14 @@
 
     # derivative with respect to generator arguments
     dG_dT = np.moveaxis(generator_jac.reshape((state_init.size, state_init.size, -1)), 2, 0)
     term_1 = dG_dT @ state_p
     term_2 = dG_dT @ (generator @ state_m) + (generator @ (dG_dT @ state_m).T).T
     param_block = c_1 * term_1 + c_2 * term_2
 
-    # derivative with respect to total time
+    # derivative with respect to the time_span
     term_1 = generator @ state_p
     term_2 = generator @ (generator @ state_m)
     term_3 = param_block[0, :]
     time_block = c_1 / time_span * term_1 + c_2 * 2.0 / time_span * term_2 + time_ratio * term_3
 
     return np.hstack([state_block, param_block[1:, :].T, time_block.reshape(-1, 1)])
```

### Comparing `topt-0.0.1/PKG-INFO` & `topt-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: topt
-Version: 0.0.1
+Version: 0.0.3
 Summary: Tools for optimizing trajectories with direct collocation.
+Home-page: https://github.com/perlinm/topt
 License: Apache-2.0
 Author: Michael A. Perlin
 Author-email: mika.perlin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,14 +17,14 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: dev
 Requires-Dist: checks-superstaq (>=0.5.0) ; extra == "dev"
 Requires-Dist: cyipopt (>=1.4.1)
 Requires-Dist: jax (>=0.4.26)
 Requires-Dist: jaxlib (>=0.4.26)
+Project-URL: Repository, https://github.com/perlinm/topt
 Description-Content-Type: text/markdown
 
 # topt
 
 This package contains tools for trajectory optimization with direct collocation.
 
-
```

