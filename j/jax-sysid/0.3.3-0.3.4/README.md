# Comparing `tmp/jax_sysid-0.3.3.tar.gz` & `tmp/jax_sysid-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax_sysid-0.3.3.tar", last modified: Wed Apr 24 15:04:29 2024, max compression
+gzip compressed data, was "jax_sysid-0.3.4.tar", last modified: Fri May  3 10:40:25 2024, max compression
```

## Comparing `jax_sysid-0.3.3.tar` & `jax_sysid-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 15:04:29.915399 jax_sysid-0.3.3/
--rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.3.3/LICENSE.txt
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-24 15:04:29.915204 jax_sysid-0.3.3/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)    12152 2024-03-07 06:02:39.000000 jax_sysid-0.3.3/README.md
--rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-04-24 15:04:05.000000 jax_sysid-0.3.3/pyproject.toml
--rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-04-24 15:04:29.915437 jax_sysid-0.3.3/setup.cfg
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 15:04:29.913301 jax_sysid-0.3.3/src/
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 15:04:29.914134 jax_sysid-0.3.3/src/jax_sysid/
--rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.3.3/src/jax_sysid/__init__.py
--rw-r--r--   0 bemporad   (501) staff       (20)    65286 2024-04-24 15:03:12.000000 jax_sysid-0.3.3/src/jax_sysid/models.py
--rw-r--r--   0 bemporad   (501) staff       (20)    11300 2024-04-24 13:40:59.000000 jax_sysid-0.3.3/src/jax_sysid/utils.py
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 15:04:29.914999 jax_sysid-0.3.3/src/jax_sysid.egg-info/
--rw-r--r--   0 bemporad   (501) staff       (20)    12952 2024-04-24 15:04:29.000000 jax_sysid-0.3.3/src/jax_sysid.egg-info/PKG-INFO
--rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-04-24 15:04:29.000000 jax_sysid-0.3.3/src/jax_sysid.egg-info/SOURCES.txt
--rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-04-24 15:04:29.000000 jax_sysid-0.3.3/src/jax_sysid.egg-info/dependency_links.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-04-24 15:04:29.000000 jax_sysid-0.3.3/src/jax_sysid.egg-info/requires.txt
--rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-04-24 15:04:29.000000 jax_sysid-0.3.3/src/jax_sysid.egg-info/top_level.txt
-drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-04-24 15:04:29.914841 jax_sysid-0.3.3/tests/
--rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.3.3/tests/test_models.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-03 10:40:25.893172 jax_sysid-0.3.4/
+-rw-r--r--   0 bemporad   (501) staff       (20)    11345 2024-03-01 16:55:21.000000 jax_sysid-0.3.4/LICENSE.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)    14105 2024-05-03 10:40:25.892957 jax_sysid-0.3.4/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)    13305 2024-05-03 10:38:17.000000 jax_sysid-0.3.4/README.md
+-rw-r--r--   0 bemporad   (501) staff       (20)      801 2024-05-03 10:38:33.000000 jax_sysid-0.3.4/pyproject.toml
+-rw-r--r--   0 bemporad   (501) staff       (20)       38 2024-05-03 10:40:25.893211 jax_sysid-0.3.4/setup.cfg
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-03 10:40:25.890935 jax_sysid-0.3.4/src/
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-03 10:40:25.891878 jax_sysid-0.3.4/src/jax_sysid/
+-rw-r--r--   0 bemporad   (501) staff       (20)        0 2023-01-10 11:29:35.000000 jax_sysid-0.3.4/src/jax_sysid/__init__.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    69345 2024-05-02 19:11:43.000000 jax_sysid-0.3.4/src/jax_sysid/models.py
+-rw-r--r--   0 bemporad   (501) staff       (20)    11403 2024-05-03 09:46:56.000000 jax_sysid-0.3.4/src/jax_sysid/utils.py
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-03 10:40:25.892746 jax_sysid-0.3.4/src/jax_sysid.egg-info/
+-rw-r--r--   0 bemporad   (501) staff       (20)    14105 2024-05-03 10:40:25.000000 jax_sysid-0.3.4/src/jax_sysid.egg-info/PKG-INFO
+-rw-r--r--   0 bemporad   (501) staff       (20)      314 2024-05-03 10:40:25.000000 jax_sysid-0.3.4/src/jax_sysid.egg-info/SOURCES.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)        1 2024-05-03 10:40:25.000000 jax_sysid-0.3.4/src/jax_sysid.egg-info/dependency_links.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       49 2024-05-03 10:40:25.000000 jax_sysid-0.3.4/src/jax_sysid.egg-info/requires.txt
+-rw-r--r--   0 bemporad   (501) staff       (20)       10 2024-05-03 10:40:25.000000 jax_sysid-0.3.4/src/jax_sysid.egg-info/top_level.txt
+drwxr-xr-x   0 bemporad   (501) staff       (20)        0 2024-05-03 10:40:25.892586 jax_sysid-0.3.4/tests/
+-rw-r--r--   0 bemporad   (501) staff       (20)     5280 2024-03-06 15:24:05.000000 jax_sysid-0.3.4/tests/test_models.py
```

### Comparing `jax_sysid-0.3.3/LICENSE.txt` & `jax_sysid-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jax_sysid-0.3.3/PKG-INFO` & `jax_sysid-0.3.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.3.3
+Version: 0.3.4
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -302,14 +302,28 @@
 By default, **jax-sysid** minimizes the classical mean squared error
 
 $$
 	{\mathcal L}(\hat Y,Y)=\frac{1}{N}\sum_{k=0}^{N-1}
 	\|y_k-\hat y_k\|_2^2
 $$
 
+**jax-sysid** also supports custom regularization terms $r_c(z)$, where $z=(\theta,x_0)$. You can specify such custom regularization function it in the definition of the overall loss. For example, say for some reason you want to impose $\|\theta\|_2^2\leq 1$ as a soft constraint, you can penalize
+
+$$\frac{1}{2} \rho_{\theta} \|\theta\|_2^2 + \rho_{x_0} \|x_0\|_2^2 + \rho_c\max\{\|\theta\|_2^2-1,0\}^2$$
+
+with $\rho_c\gg\rho_\theta$, $\rho_c\gg\rho_{x_0}$, for instance $\rho_c=1000$, $\rho_\theta=0.001$, $\rho_{x0}=0.01$. In Python:
+
+~~~python
+@jax.jit
+def custom_reg_fcn(th,x0):
+    return 1000.*jnp.maximum(jnp.sum(th**2)-1.,0.)**2
+model.loss(rho_x0=0.01, rho_th=0.001, custom_regularization= custom_reg_fcn)
+~~~
+
+
 
 <a name="static"></a>
 ### Static models and nonlinear regression
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
@@ -355,14 +369,21 @@
     
 model = FNN(ny, nu, FY)
 model.loss(rho_th=1.e-4, tau_th=tau_th)
 model.optimization(lbfgs_epochs=500)
 model.fit(Ys, Us)
 ~~~
 
+To include lower and upper bounds on the parameters of the model, use the following additional arguments when specifying the optimization problem:
+
+~~~python
+model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
+~~~
+
+where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples on how to use nonnegative constraints to fit input-convex neural networks.
 
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.3.3/README.md` & `jax_sysid-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -280,14 +280,28 @@
 By default, **jax-sysid** minimizes the classical mean squared error
 
 $$
 	{\mathcal L}(\hat Y,Y)=\frac{1}{N}\sum_{k=0}^{N-1}
 	\|y_k-\hat y_k\|_2^2
 $$
 
+**jax-sysid** also supports custom regularization terms $r_c(z)$, where $z=(\theta,x_0)$. You can specify such custom regularization function it in the definition of the overall loss. For example, say for some reason you want to impose $\|\theta\|_2^2\leq 1$ as a soft constraint, you can penalize
+
+$$\frac{1}{2} \rho_{\theta} \|\theta\|_2^2 + \rho_{x_0} \|x_0\|_2^2 + \rho_c\max\{\|\theta\|_2^2-1,0\}^2$$
+
+with $\rho_c\gg\rho_\theta$, $\rho_c\gg\rho_{x_0}$, for instance $\rho_c=1000$, $\rho_\theta=0.001$, $\rho_{x0}=0.01$. In Python:
+
+~~~python
+@jax.jit
+def custom_reg_fcn(th,x0):
+    return 1000.*jnp.maximum(jnp.sum(th**2)-1.,0.)**2
+model.loss(rho_x0=0.01, rho_th=0.001, custom_regularization= custom_reg_fcn)
+~~~
+
+
 
 <a name="static"></a>
 ### Static models and nonlinear regression
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
@@ -333,14 +347,21 @@
     
 model = FNN(ny, nu, FY)
 model.loss(rho_th=1.e-4, tau_th=tau_th)
 model.optimization(lbfgs_epochs=500)
 model.fit(Ys, Us)
 ~~~
 
+To include lower and upper bounds on the parameters of the model, use the following additional arguments when specifying the optimization problem:
+
+~~~python
+model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
+~~~
+
+where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples on how to use nonnegative constraints to fit input-convex neural networks.
 
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.3.3/pyproject.toml` & `jax_sysid-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jax-sysid"
-version = "0.3.3"
+version = "0.3.4"
 authors = [
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["numpy","scipy","jax","jaxopt","flax","tqdm","matplotlib","pmlb"]
```

### Comparing `jax_sysid-0.3.3/src/jax_sysid/models.py` & `jax_sysid-0.3.4/src/jax_sysid/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     object.lbfgs_epochs = lbfgs_epochs
     object.iprint = iprint
     object.memory = memory
     object.lbfgs_tol = lbfgs_tol
     return object
 
 
-def adam_solver(JdJ, z, solver_iters, adam_eta, iprint):
+def adam_solver(JdJ, z, solver_iters, adam_eta, iprint, params_min=None, params_max=None):
     """
     Solves a nonlinear optimization problem using the Adam optimization algorithm.
 
     Parameters
     ----------
     JdJ : callable
         A function that computes the objective function value and its gradient.
@@ -130,15 +130,21 @@
         A list of numpy arrays representing the initial guess of the optimization variables.
     solver_iters : int
         The number of iterations for the solver.
     adam_eta : float
         The learning rate for the Adam algorithm.
     iprint : int
         Verbosity level. Set to -1 to disable printing.
-
+    params_min : list, optional
+        A list of numpy arrays representing the lower bounds of the optimization variables z.
+        Lower bounds are enforced by clipping the variables during the iterations.
+    params_max : list, optional
+        A list of numpy arrays representing the upper bounds of the optimization variables z.
+        Upper bounds are enforced by clipping the variables during the iterations.
+    
     Returns
     -------
     tuple
         A tuple containing the optimized variables `z` and the objective function value `Jopt`.
     """
     if iprint > -1:
         iters_tqdm = tqdm.tqdm(total=solver_iters, desc='Iterations', ncols=30,
@@ -154,25 +160,42 @@
     m = [np.zeros(zi.shape) for zi in z]
     beta1 = 0.9
     beta2 = 0.99
     beta1t = beta1
     beta2t = beta2
     epsil = 1e-8
 
+    ismin =(params_min is not None)
+    ismax =(params_max is not None)
+    isbounded = ismin or ismax
+    if isbounded:
+        # Clip the initial guess, when required
+        for j in range(nz):
+            if ismin:
+                z[j] = np.maximum(z[j], params_min[j])
+            if ismax:
+                z[j] = np.minimum(z[j], params_max[j])
+        
     for k in range(solver_iters):
         f, df = JdJ(z)
         if fbest > f:
             fbest = f
             zbest = z.copy()
         for j in range(nz):
             m[j] = beta1*m[j] + (1 - beta1) * df[j]
             v[j] = beta2*v[j] + (1 - beta2) * df[j]**2
             # classical Adam step
             z[j] -= adam_eta/(1 - beta1t)*m[j] / \
                 (np.sqrt(v[j]/(1 - beta2t)) + epsil)
+        if isbounded:
+            for j in range(nz):
+                if ismin:
+                    z[j] = np.maximum(z[j], params_min[j])
+                if ismax:
+                    z[j] = np.minimum(z[j], params_max[j])
 
         beta1t *= beta1
         beta2t *= beta2
 
         if iprint > -1:
             str = f"    f = {f: 10.6f}, f* = {fbest: 8.6f}"
             ndf = np.sum([np.linalg.norm(df[i])
@@ -1381,15 +1404,15 @@
         self.tau_th = tau_th
         self.tau_g = tau_g
         self.zero_coeff = zero_coeff
         self.group_lasso_fcn = group_lasso_fcn        
         self.custom_regularization=custom_regularization
         return
 
-    def optimization(self, adam_eta=None, adam_epochs=None, lbfgs_epochs=None, iprint=None, memory=None, lbfgs_tol=None):
+    def optimization(self, adam_eta=None, adam_epochs=None, lbfgs_epochs=None, iprint=None, memory=None, lbfgs_tol=None, params_min=None, params_max=None):
         """Define optimization parameters for the system identification problem.
 
         Parameters
         ----------
         adam_eta : float
             Adam's learning rate (not used by LBFGS).
         adam_epochs : int
@@ -1398,14 +1421,18 @@
             Max number of function evaluations in the following L-BFGS iterations (lbfgs_epochs=0 means pure Adam).
         iprint : int
             How often printing L-BFGS updates (-1 = no printing, not even Adam iterations).
         memory : int
             L-BGFS memory (not used if method = 'Adam').
         lbfsg_tol : float
             Tolerance for L-BFGS-B iterations (not used if method = 'Adam').
+        params_min : list of arrays, optional
+            List of the same structure as self.params of lower bounds for the parameters.
+        params_max : list of arrays, optional
+            List of the same structure as self.params of upper bounds for the parameters.            
         """
         self = optimization_base(self)
 
         if adam_eta is not None:
             self.adam_eta = adam_eta
         if adam_epochs is not None:
             self.adam_epochs = adam_epochs
@@ -1413,14 +1440,16 @@
             self.lbfgs_epochs = lbfgs_epochs
         if iprint is not None:
             self.iprint = iprint
         if memory is not None:
             self.memory = memory
         if lbfgs_tol is not None:
             self.lbfgs_tol = lbfgs_tol
+        self.params_min = params_min
+        self.params_max = params_max
         return
 
     def init(self, params=None):
         """Initialize model parameters
 
         Parameters
         ----------
@@ -1460,15 +1489,24 @@
         Y = vec_reshape(Y)
 
         if self.params is None:
             raise (Exception(
                 "\033[1mPlease use the init method to initialize the parameters of the model\033[0m"))
 
         z = self.params
-
+        
+        if self.params_min is not None and self.params_max is None:
+            self.params_max=list()
+            for i in range(len(z)):
+                self.params_max.append(jnp.ones_like(z[i])*np.inf)
+        if self.params_max is not None and self.params_min is None:
+            self.params_min=list()
+            for i in range(len(z)):
+                self.params_min.append(-jnp.ones_like(z[i])*np.inf)
+            
         tau_th = self.tau_th
         tau_g = self.tau_g
 
         isL1reg = tau_th > 0
         isGroupLasso = (tau_g > 0) and (self.group_lasso_fcn is not None)
         isCustomReg = (self.custom_regularization is not None)
 
@@ -1543,36 +1581,75 @@
                         cost += self.custom_regularization(z)
                     return cost
 
                 def JdJ(z):
                     return jax.value_and_grad(J)(z)
 
                 z, Jopt = adam_solver(
-                    JdJ, z, solver_iters, self.adam_eta, self.iprint)
+                    JdJ, z, solver_iters, self.adam_eta, self.iprint, self.params_min, self.params_max)
 
             elif solver == "LBFGS":
                 # L-BFGS-B params (no L1 regularization)
                 options = lbfgs_options(
                     min(self.iprint, 90), solver_iters, self.lbfgs_tol, self.memory)
 
                 if self.iprint > -1:
                     print(
                         "Solving NLP with L-BFGS (%d optimization variables) ..." % nvars)
 
+                def get_bounds(z,epsil_lasso,params_min,params_max):
+                    # utility function to create bounds for L-BFGS-B when splitting positive and negative parts
+
+                    isbounded = (params_min is not None) or (params_max is not None)
+
+                    lb = list()
+                    if not isbounded:
+                        for i in range(2 * nth):
+                            lb.append(jnp.zeros_like(z[i])+epsil_lasso)
+                        ub=np.inf
+                    else:
+                        # We have bounds on the parameters:
+                        #     lb <= x  <= ub with y,z>=epsil_lasso and x = y-z
+                        #
+                        # Then, we impose:
+                        #       max(0,lb) +epsil_lasso <= y <= max(0,ub) +epsil_lasso
+                        #       max(0,-ub)+epsil_lasso <= z <= max(0,-lb)+epsil_lasso
+                        #
+                        # Note: we could eliminate some variables when the lower and upper bounds
+                        # are both equal to epsil_lasso
+                        ub=list() 
+                        for i in range(nth):
+                            # positive part y
+                            zi=jnp.zeros_like(z[i])
+                            lb.append(jnp.maximum(params_min[i],zi)+epsil_lasso)
+                            ub.append(jnp.maximum(params_max[i],zi)+epsil_lasso)
+                        for i in range(nth):
+                            # negative part z
+                            zi=jnp.zeros_like(z[i])
+                            lb.append(jnp.maximum(-params_max[i],zi)+epsil_lasso)
+                            ub.append(jnp.maximum(-params_min[i],zi)+epsil_lasso)
+                    return (lb,ub)
+
                 if not isGroupLasso:
                     if not isL1reg:
                         def J(z):
                             cost = loss(z) + self.rho_th*l2reg(z)
                             if isCustomReg:
                                 cost += self.custom_regularization(z)
                             return cost
 
-                        solver = jaxopt.ScipyMinimize(
-                            fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
-                        z, state = solver.run(z)
+                        if (self.params_min is None) and (self.params_max is None):
+                            solver = jaxopt.ScipyMinimize(
+                                fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
+                            z, state = solver.run(z)
+                        else:
+                            solver = jaxopt.ScipyBoundedMinimize(
+                                fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
+                            z, state = solver.run(z, bounds = (self.params_min, self.params_max))
+                            
                         iter_num = state.iter_num
                         Jopt = state.fun_val
                     else:
                         # Optimize wrt to split positive and negative part of model parameters
                         @jax.jit
                         def J(z):
                             th = [z1 - z2 for (z1, z2)
@@ -1581,18 +1658,17 @@
                                 z[nth:2 * nth]) + tau_th*linreg(z[0:nth]) + tau_th*linreg(z[nth:2 * nth])
                             if isCustomReg:
                                 cost += self.custom_regularization(th)
                             return cost
 
                         solver = jaxopt.ScipyBoundedMinimize(
                             fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
-                        lb = list()
-                        for i in range(2 * nth):
-                            lb.append(0. * z[i]+epsil_lasso)
-                        z, state = solver.run(z, bounds=(lb, np.inf))
+
+                        bounds = get_bounds(z,epsil_lasso,self.params_min,self.params_max)
+                        z, state = solver.run(z, bounds=bounds)
                         z[0:nth] = [
                             z1 - z2 for (z1, z2) in zip(z[0:nth], z[nth:2 * nth])]
                         iter_num = state.iter_num
                         Jopt = state.fun_val
 
                 else:  # group Lasso
                     @jax.jit
@@ -1607,18 +1683,16 @@
                                     [z1 + z2 for (z1, z2) in zip(z[0:nth], z[nth:2 * nth])])
                         if isCustomReg:
                             cost += self.custom_regularization(th)
                         return cost
 
                     solver = jaxopt.ScipyBoundedMinimize(
                         fun=J, tol=self.lbfgs_tol, method="L-BFGS-B", maxiter=solver_iters, options=options)
-                    lb = list()
-                    for i in range(2 * nth):
-                        lb.append(0. * z[i]+epsil_lasso)
-                    z, state = solver.run(z, bounds=(lb, np.inf))
+                    bounds = get_bounds(z,epsil_lasso,self.params_min,self.params_max)
+                    z, state = solver.run(z, bounds=bounds)
                     z[0:nth] = [
                         z1 - z2 for (z1, z2) in zip(z[0:nth], z[nth:2 * nth])]
                     iter_num = state.iter_num
                     Jopt = state.fun_val
 
                 if self.iprint > -1:
                     print('L-BFGS-B done in %d iterations.' % iter_num)
```

### Comparing `jax_sysid-0.3.3/src/jax_sysid/utils.py` & `jax_sysid-0.3.4/src/jax_sysid/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         Possibly reshaped array
     """
     if len(y.shape) == 1:
         y = y.reshape(-1, 1)
     return y
 
 
-def compute_scores(Y_train, Yhat_train, Y_test, Yhat_test, fit='R2'):
+def compute_scores(Y_train, Yhat_train, Y_test=None, Yhat_test=None, fit='R2'):
     """Compute R2-score, best fit rate, or accuracy score on (possibly multi-dimensional) 
        training and test output data
 
     (C) 2024 A. Bemporad
 
     Parameters
     ----------
@@ -212,15 +212,17 @@
                     score_test[i] = np.mean(
                         Yhat_test[:, i] == Y_test[:, i])*100
             if not use_training:
                 score_train[i] = np.nan
             if not use_test:
                 score_test[i] = np.nan
 
-            text += f"{fit.capitalize()} score: training = {score_train[i]: 5.4f}{unit}, test = {score_test[i]: 5.4f}{unit}"
+            text += f"{fit.capitalize()} score: training = {score_train[i]: 5.4f}{unit}"
+            if use_test:
+                text += f", test = {score_test[i]: 5.4f}{unit}"
             msg += '\n' + text
             # print(text)
         msg += "\n-----\nAverage "
     else:
         if isR2 or isBFR:
             if use_training:
                 nY_train2 = np.sum((Y_train-np.mean(Y_train))**2)
@@ -253,15 +255,17 @@
             if use_test:
                 score_test = np.mean(Yhat_test == Y_test)*100
         if not use_training:
             score_train = np.nan
         if not use_test:
             score_test = np.nan
 
-    msg += f"{fit.capitalize()} score:  training = {np.sum(score_train) / ny: 5.4f}{unit}, test = {np.sum(score_test) / ny: 5.4f}{unit}"
+    msg += f"{fit.capitalize()} score:  training = {np.sum(score_train) / ny: 5.4f}{unit}"
+    if use_test:
+        msg += f", test = {np.sum(score_test) / ny: 5.4f}{unit}"
     return score_train, score_test, msg
 
 
 def print_eigs(A):
     """Print the eigenvalues of a given square matrix.
 
     (C) 2023 A. Bemporad
```

### Comparing `jax_sysid-0.3.3/src/jax_sysid.egg-info/PKG-INFO` & `jax_sysid-0.3.4/src/jax_sysid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-sysid
-Version: 0.3.3
+Version: 0.3.4
 Summary: jax-sysid - A Python package for linear and nonlinear system identification and nonlinear regression using Jax.
 Author-email: Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, http://cse.lab.imtlucca.it/~bemporad/jax-sysid
 Keywords: system identification,subspace identification,nonlinear regression
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -302,14 +302,28 @@
 By default, **jax-sysid** minimizes the classical mean squared error
 
 $$
 	{\mathcal L}(\hat Y,Y)=\frac{1}{N}\sum_{k=0}^{N-1}
 	\|y_k-\hat y_k\|_2^2
 $$
 
+**jax-sysid** also supports custom regularization terms $r_c(z)$, where $z=(\theta,x_0)$. You can specify such custom regularization function it in the definition of the overall loss. For example, say for some reason you want to impose $\|\theta\|_2^2\leq 1$ as a soft constraint, you can penalize
+
+$$\frac{1}{2} \rho_{\theta} \|\theta\|_2^2 + \rho_{x_0} \|x_0\|_2^2 + \rho_c\max\{\|\theta\|_2^2-1,0\}^2$$
+
+with $\rho_c\gg\rho_\theta$, $\rho_c\gg\rho_{x_0}$, for instance $\rho_c=1000$, $\rho_\theta=0.001$, $\rho_{x0}=0.01$. In Python:
+
+~~~python
+@jax.jit
+def custom_reg_fcn(th,x0):
+    return 1000.*jnp.maximum(jnp.sum(th**2)-1.,0.)**2
+model.loss(rho_x0=0.01, rho_th=0.001, custom_regularization= custom_reg_fcn)
+~~~
+
+
 
 <a name="static"></a>
 ### Static models and nonlinear regression
 The same optimization algorithms used to train dynamical models can be used to train static models, i.e., to solve the nonlinear regression problem:
 
 $$  \min_{z}r(z)+\frac{1}{N}\sum_{k=0}^{N-1} \|y_{k}-f(u_k,\theta)\|_2^2$$
 
@@ -355,14 +369,21 @@
     
 model = FNN(ny, nu, FY)
 model.loss(rho_th=1.e-4, tau_th=tau_th)
 model.optimization(lbfgs_epochs=500)
 model.fit(Ys, Us)
 ~~~
 
+To include lower and upper bounds on the parameters of the model, use the following additional arguments when specifying the optimization problem:
+
+~~~python
+model.optimization(lbfgs_epochs=500, params_min=lb, params_max=ub)
+~~~
+
+where `lb` and `ub` are lists of arrays with the same structure as `model.params`. See `example_static_convex.py` for examples on how to use nonnegative constraints to fit input-convex neural networks.
 
                 
 <a name="contributors"><a>
 ## Contributors
 
 This package was coded by Alberto Bemporad.
```

### Comparing `jax_sysid-0.3.3/tests/test_models.py` & `jax_sysid-0.3.4/tests/test_models.py`

 * *Files identical despite different names*

