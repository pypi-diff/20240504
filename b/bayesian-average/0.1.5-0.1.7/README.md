# Comparing `tmp/bayesian_average-0.1.5.tar.gz` & `tmp/bayesian_average-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesian_average-0.1.5.tar", last modified: Tue Apr 30 20:52:27 2024, max compression
+gzip compressed data, was "bayesian_average-0.1.7.tar", last modified: Sat May  4 11:23:01 2024, max compression
```

## Comparing `bayesian_average-0.1.5.tar` & `bayesian_average-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:52:27.090153 bayesian_average-0.1.5/
--rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.1.5/LICENSE.txt
--rw-r--r--   0 martino    (501) staff       (20)     4141 2024-04-30 20:52:27.089873 bayesian_average-0.1.5/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)     3955 2024-04-30 20:52:12.000000 bayesian_average-0.1.5/README.md
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:52:27.088995 bayesian_average-0.1.5/bayesian_average/
--rw-rw-r--   0 martino    (501) staff       (20)     4054 2024-04-30 20:52:20.000000 bayesian_average-0.1.5/bayesian_average/__init__.py
--rw-r--r--   0 martino    (501) staff       (20)       21 2024-04-30 20:51:51.000000 bayesian_average-0.1.5/bayesian_average/_version.py
--rw-rw-r--   0 martino    (501) staff       (20)     6563 2024-04-30 20:32:56.000000 bayesian_average-0.1.5/bayesian_average/average.py
-drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-04-30 20:52:27.089604 bayesian_average-0.1.5/bayesian_average.egg-info/
--rw-r--r--   0 martino    (501) staff       (20)     4141 2024-04-30 20:52:27.000000 bayesian_average-0.1.5/bayesian_average.egg-info/PKG-INFO
--rw-r--r--   0 martino    (501) staff       (20)      276 2024-04-30 20:52:27.000000 bayesian_average-0.1.5/bayesian_average.egg-info/SOURCES.txt
--rw-r--r--   0 martino    (501) staff       (20)        1 2024-04-30 20:52:27.000000 bayesian_average-0.1.5/bayesian_average.egg-info/dependency_links.txt
--rw-r--r--   0 martino    (501) staff       (20)       17 2024-04-30 20:52:27.000000 bayesian_average-0.1.5/bayesian_average.egg-info/top_level.txt
--rw-r--r--   0 martino    (501) staff       (20)       38 2024-04-30 20:52:27.090196 bayesian_average-0.1.5/setup.cfg
--rw-r--r--   0 martino    (501) staff       (20)      460 2024-04-30 19:16:24.000000 bayesian_average-0.1.5/setup.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.098336 bayesian_average-0.1.7/
+-rw-rw-r--   0 martino    (501) staff       (20)     1274 2024-03-28 16:44:26.000000 bayesian_average-0.1.7/LICENSE.txt
+-rw-r--r--   0 martino    (501) staff       (20)     4156 2024-05-04 11:23:01.098100 bayesian_average-0.1.7/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)     3955 2024-05-04 11:16:11.000000 bayesian_average-0.1.7/README.md
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.097133 bayesian_average-0.1.7/bayesian_average/
+-rw-r--r--   0 martino    (501) staff       (20)      993 2024-05-04 11:01:49.000000 bayesian_average-0.1.7/bayesian_average/__init__.py
+-rw-r--r--   0 martino    (501) staff       (20)       21 2024-05-04 11:02:49.000000 bayesian_average-0.1.7/bayesian_average/_version.py
+-rw-r--r--   0 martino    (501) staff       (20)     6467 2024-05-02 08:29:12.000000 bayesian_average-0.1.7/bayesian_average/average.py
+drwxr-xr-x   0 martino    (501) staff       (20)        0 2024-05-04 11:23:01.097874 bayesian_average-0.1.7/bayesian_average.egg-info/
+-rw-r--r--   0 martino    (501) staff       (20)     4156 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/PKG-INFO
+-rw-r--r--   0 martino    (501) staff       (20)      276 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/SOURCES.txt
+-rw-r--r--   0 martino    (501) staff       (20)        1 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/dependency_links.txt
+-rw-r--r--   0 martino    (501) staff       (20)       17 2024-05-04 11:23:01.000000 bayesian_average-0.1.7/bayesian_average.egg-info/top_level.txt
+-rw-r--r--   0 martino    (501) staff       (20)       38 2024-05-04 11:23:01.098387 bayesian_average-0.1.7/setup.cfg
+-rw-r--r--   0 martino    (501) staff       (20)      622 2024-05-04 11:22:52.000000 bayesian_average-0.1.7/setup.py
```

### Comparing `bayesian_average-0.1.5/LICENSE.txt` & `bayesian_average-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bayesian_average-0.1.5/PKG-INFO` & `bayesian_average-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: bayesian_average
-Version: 0.1.5
-Summary: Python package to calculate the weighted average with Bayesian methods
-Author: Marleen Maxton
+Version: 0.1.7
+Summary: __doc__
+Author: Marleen Maxton, Martino Trassinelli
 License: X11
+Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-
 # Bayesian average
 
 ### Version:
-0.1.5
+0.1.7
 
 ### Authors
-Martino TrassinelliCNRS, Institute of NanoSciences of Parisemail: trassinelli AT insp.jussieu.fremail: m.trassinelli AT gmail.com
-
-Marleen MaxtonMax Planck Institute Heidelbergemail:
+Martino Trassinelli\
+CNRS, Institute of NanoSciences of Paris\
+email: trassinelli AT insp.jussieu.fr\
+email: m.trassinelli AT gmail.com
+
+Marleen Maxton\
+Max Planck Institute Heidelberg\
+email:
 
 ### Homepage
 https://github.com/martinit18/bayesian_average
 
 
 ### License
 Type: X11, see `LICENCE.txt`
@@ -57,23 +62,26 @@
 ```
 ba.plot_average(data,sigma,jwa_val=True,plot_data=True)
 ```
 The option `jwa_val=True` is on on as default. `plot_data=True` show the input data in addition.
 
 ## Details of the vailable weighted averages
 
-- `jwa`: **Jeffreys weighted average** (main average, RECOMENDED, see Ref.[1]).    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to $1/\sigma'$.
+- `jwa`: **Jeffreys weighted average** (main average, RECOMENDED, see Ref.[1]).\
+    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to $1/\sigma'$.
     Because of the non-normalisability of the final probability distribution, this weighted average results 
-    correspond to the  limit case with prior bounds $[\sigma, \sigma_\mathrm{max}]$ with $\sigma_\mathrm{max} 	o \infty$ and where $\sigma$ is the value provided by the user.
+    correspond to the  limit case with prior bounds $[\sigma, \sigma_\mathrm{max}]$ with $\sigma_\mathrm{max} \to \infty$ and where $\sigma$ is the value provided by the user.
     The final probability distribution is, however not a proper probability distribution.
-- `cwa`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).    The priors of the real uncertainty value are proportional to $\sigma/(\sigma')^2$, where $\sigma$ is the value provided by the user.
+- `cwa`: **Conservative weighted average** (adapted for proper final probability distributions, see Ref.[2]).\
+    The priors of the real uncertainty value are proportional to $\sigma/(\sigma')^2$, where $\sigma$ is the value provided by the user.
     The bounds of the prior are $[\sigma, \sigma_\mathrm{max}]$.
     This is a modified and normalisable version of the non-informative Jeffeys' prior.
-- `wa`: **Standard weighted average**    The standard inverse-variance weighted average useful for comparisons.
+- `wa`: **Standard weighted average**\
+    The standard inverse-variance weighted average useful for comparisons.
 
 
 
 
 ## Refere articles:
-[1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* [2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
-
+[1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
+[2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
```

### Comparing `bayesian_average-0.1.5/README.md` & `bayesian_average-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Bayesian average
 
 ### Version:
-0.1.5
+0.1.7
 
 ### Authors
 Martino Trassinelli\
 CNRS, Institute of NanoSciences of Paris\
 email: trassinelli AT insp.jussieu.fr\
 email: m.trassinelli AT gmail.com
```

### Comparing `bayesian_average-0.1.5/bayesian_average/__init__.py` & `bayesian_average-0.1.7/bayesian_average.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-from .average import jwa, cwa, wa, plot_average
-from ._version import __version__
+Metadata-Version: 2.1
+Name: bayesian_average
+Version: 0.1.7
+Summary: __doc__
+Author: Marleen Maxton, Martino Trassinelli
+License: X11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
-__doc__="""
 # Bayesian average
 
 ### Version:
-0.1.5
+0.1.7
 
 ### Authors
 Martino Trassinelli\
 CNRS, Institute of NanoSciences of Paris\
 email: trassinelli AT insp.jussieu.fr\
 email: m.trassinelli AT gmail.com
 
@@ -76,9 +81,7 @@
 
 
 
 ## Refere articles:
 [1] M. Trassinelli and M. Maxton, *A minimalistic and general weighted average for inconsistent data*, in preparation for *Metrologia* \
 [2] D. S. Sivia and J. Skilling, *Data analysis: a Bayesian tutorial*, 2nd ed 2006, Oxford Univ. Press
 
-
-"""
```

### Comparing `bayesian_average-0.1.5/bayesian_average/average.py` & `bayesian_average-0.1.7/bayesian_average/average.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import numpy as np
-from sympy import log, exp, diff, lambdify, sqrt, pi, erf
-from sympy.abc import mu
-from scipy.optimize import basinhopping
-from matplotlib.pyplot import errorbar, legend, ylabel, show, axvline, plot, gca
-
-
-def wa(data, sigma):
-    """
-    Standard invariance inverse weighted average.
-    Attention! In this case the scattering of the data is not included in the final uncertainty
-    """
-    weights = 1 / np.array(sigma)**2
-    av_value = np.average(data, weights = weights) #find minima of negative loglikelihood
-    sig_value = 1/np.sqrt(np.sum(weights)) #calculate sigma        
-    return av_value, sig_value
-
-def cwa(data, sigma):    
-    """
-    Conservative weighted average proposed by Sivia in 2004 (see references in README file).
-    The priors of the real uncertainty value are proportional to sigma_0/sigma^2, where sigma_0 is the value provided by the user
-    The bounds of the prior are [sigma_0, infinite].
-    This is a modified and normalisable version of the non-informative Jeffeys' prior.
-    """
-    loglike = np.sum([log((1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)]) #loglikelihood function
-    ddloglike = diff(loglike, mu, 2) #second derivative
-    negloglike = lambdify(mu, -loglike)
-    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
-    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)) #calculate sigma        
-    return av_value, sig_value
-
-def jwa(data, sigma):    
-    """
-    Jeffreys weighted average proposed by Trassinelli and Maxton in 2024 (see references in README file).
-    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to 1/sigma'.
-    Because of the non-normalisability of the final probability distribution, this weighted average results 
-    correspond to the  limit case with prior bounds [sigma, sigma_max] with sigma_max -> infinite. 
-    The final probability distribution is, however not a proper probability distribution.
-    """
-    loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
-    ddloglike = diff(loglike, mu, 2) #second derivative
-    negloglike = lambdify(mu, -loglike)
-    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
-    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)).evalf() #calculate sigma        
-    return av_value, sig_value
-
-def plot_average(data, sigma, plot_data = False, wa_val = False, cwa_val = False, jwa_val = True, 
-                 wa_loglike = False, cwa_loglike = False, jwa_loglike = True, 
-                 legendon = True, normalize = False):
-    """
-    This is the main plot function of the library.
-
-    Three weighted average are available:
-        - wa: standard weigted average
-        - jwa: Jeffreys weighted average
-        - cwa: conservative weighted average
-
-    Please select the items you want to plot.
-    xxx indicates wa, jwa or cwa.
-        - plot_data: plot the input data with the input errorbar
-        - xxx_val: plot the weighted average and the corresponding uncertainty
-        - xxx_like: plot the corresponding likelihood
-
-    To have normalised curves of likelihood put `normalize=True'
-
-    """
-
-    if not (plot_data or wa_val or cwa_val or jwa_val or wa_loglike or cwa_loglike or jwa_loglike):
-        print("Please enter at least one thing that you want to plot.")
-    else:
-        x_plot = np.linspace(min(np.array(data) - np.array(sigma)), max(np.array(data) + np.array(sigma)),100)
-        if cwa_val:
-            cwa_av, cwa_sig = cwa(data, sigma)
-            print("Conservative weighted average:", cwa_av, "+-", cwa_sig)
-            axvline(cwa_av, c = "b", label = "Conservative weighted average")
-            axvline(cwa_av - cwa_sig, c='b', ls = "--")
-            axvline(cwa_av + cwa_sig, c='b', ls = "--")
-        if cwa_loglike:
-            loglike = np.sum([log(sqrt(2 / pi) * s_temp * (1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)])
-            loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
-            if normalize:
-                y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'dodgerblue', label = "Conservative final likelihood")
-        if wa_val:
-            wa_av, wa_sig = wa(data, sigma)
-            print("Standard weighted average:", wa_av, "+-", wa_sig)
-            axvline(wa_av, c = "r", label = "Standard weighted average")
-            axvline(wa_av - wa_sig, c='r', ls = "--")
-            axvline(wa_av + wa_sig, c='r', ls = "--")
-        if wa_loglike:
-            loglike = np.sum([log(1/(s_temp * sqrt(2 * pi)) * exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) for x_temp, s_temp in zip(data, sigma)])
-            loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
-            if normalize:
-                y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'orange', label = "Standard likelihood")
-        if jwa_val:
-            jeff_av, jeff_sig = jwa(data, sigma)
-            print("Jeffreys weighted average:", jeff_av, "+-", jeff_sig)
-            axvline(jeff_av, c = "g", label = "Jeffreys final likelihood")
-            axvline(jeff_av - jeff_sig, c='g', ls = "--")
-            axvline(jeff_av + jeff_sig, c='g', ls = "--")
-        if jwa_loglike:
-            loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
-            loglike_lam = lambdify(mu, loglike)
-            y_plot = loglike_lam(x_plot)
-            if normalize:
-                y_plot = (y_plot - min(y_plot))
-                y_plot = y_plot / np.sum(y_plot)
-            plot(x_plot, y_plot, c = 'lime', label = "Jeffreys weighted average")
-        if plot_data:
-            y_min, y_max = gca().get_ylim()
-            y_dist = y_max - y_min
-            y_data = np.linspace(y_min + 0.2 * y_dist, y_min + 0.8 * y_dist, len(data))
-            errorbar(data, y_data, xerr = sigma, ls = "", capsize = 3, marker = ".", label = "data", c = "k")
-        if legendon: legend()
-        if normalize:
-            ylabel("normalized log-likelihood")
-        else:
-            ylabel("log-likelihood")
-        show()
+import numpy as np
+from sympy import log, exp, diff, lambdify, sqrt, pi, erf
+from sympy.abc import mu
+from scipy.optimize import basinhopping
+from matplotlib.pyplot import errorbar, legend, ylabel, show, axvline, plot, gca
+
+
+def wa(data, sigma):
+    """
+    Standard invariance inverse weighted average.
+    Attention! In this case the scattering of the data is not included in the final uncertainty
+    """
+    weights = 1 / np.array(sigma)**2
+    av_value = np.average(data, weights = weights) #find minima of negative loglikelihood
+    sig_value = 1/np.sqrt(np.sum(weights)) #calculate sigma        
+    return av_value, sig_value
+
+def cwa(data, sigma):    
+    """
+    Conservative weighted average proposed by Sivia in 2004 (see references in README file).
+    The priors of the real uncertainty value are proportional to sigma_0/sigma^2, where sigma_0 is the value provided by the user
+    The bounds of the prior are [sigma_0, infinite].
+    This is a modified and normalisable version of the non-informative Jeffeys' prior.
+    """
+    loglike = np.sum([log((1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)]) #loglikelihood function
+    ddloglike = diff(loglike, mu, 2) #second derivative
+    negloglike = lambdify(mu, -loglike)
+    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
+    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)) #calculate sigma        
+    return av_value, sig_value
+
+def jwa(data, sigma):    
+    """
+    Jeffreys weighted average proposed by Trassinelli and Maxton in 2024 (see references in README file).
+    The priors of the real uncertainty value are non-informative Jeffeys' prior proportional to 1/sigma'.
+    Because of the non-normalisability of the final probability distribution, this weighted average results 
+    correspond to the  limit case with prior bounds [sigma, sigma_max] with sigma_max -> infinite. 
+    The final probability distribution is, however not a proper probability distribution.
+    """
+    loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
+    ddloglike = diff(loglike, mu, 2) #second derivative
+    negloglike = lambdify(mu, -loglike)
+    av_value = basinhopping(negloglike, np.average(data)).x[0] #find minima of negative loglikelihood
+    sig_value = 1/sqrt(-ddloglike.subs(mu, av_value)).evalf() #calculate sigma        
+    return av_value, sig_value
+
+def plot_average(data, sigma, plot_data = False, wa_val = False, cwa_val = False, jwa_val = True, 
+                 wa_loglike = False, cwa_loglike = False, jwa_loglike = True, 
+                 legendon = True, showon = False, normalize = False):
+    """
+    This is the main plot function of the library.
+
+    Three weighted average are available:
+        - wa: standard weigted average
+        - jwa: Jeffreys weighted average
+        - cwa: conservative weighted average
+
+    Please select the items you want to plot.
+    xxx indicates wa, jwa or cwa.
+        - plot_data: plot the input data with the input errorbar
+        - xxx_val: plot the weighted average and the corresponding uncertainty
+        - xxx_like: plot the corresponding likelihood
+
+    To have normalised curves of likelihood put `normalize=True'
+
+    """
+
+    if not (plot_data or wa_val or cwa_val or jwa_val or wa_loglike or cwa_loglike or jwa_loglike):
+        print("Please enter at least one thing that you want to plot.")
+    else:
+        x_plot = np.linspace(min(np.array(data) - np.array(sigma)), max(np.array(data) + np.array(sigma)),100)
+        if cwa_val:
+            cwa_av, cwa_sig = cwa(data, sigma)
+            print("Conservative weighted average:", cwa_av, "+-", cwa_sig)
+            axvline(cwa_av, c = "b", label = "Conservative weighted average")
+            axvline(cwa_av - cwa_sig, c='b', ls = "--")
+            axvline(cwa_av + cwa_sig, c='b', ls = "--")
+        if cwa_loglike:
+            loglike = np.sum([log(sqrt(2 / pi) * s_temp * (1 - exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) / (x_temp - mu)**2) for x_temp, s_temp in zip(data, sigma)])
+            loglike_lam = lambdify(mu, loglike)
+            y_plot = loglike_lam(x_plot)
+            if normalize:
+                y_plot = (y_plot - min(y_plot))
+                y_plot = y_plot / np.sum(y_plot)
+            plot(x_plot, y_plot, c = 'dodgerblue', label = "Conservative final likelihood")
+        if wa_val:
+            wa_av, wa_sig = wa(data, sigma)
+            print("Standard weighted average:", wa_av, "+-", wa_sig)
+            axvline(wa_av, c = "r", label = "Standard weighted average")
+            axvline(wa_av - wa_sig, c='r', ls = "--")
+            axvline(wa_av + wa_sig, c='r', ls = "--")
+        if wa_loglike:
+            loglike = np.sum([log(1/(s_temp * sqrt(2 * pi)) * exp(-(x_temp - mu)**2 / (s_temp**2 * 2))) for x_temp, s_temp in zip(data, sigma)])
+            loglike_lam = lambdify(mu, loglike)
+            y_plot = loglike_lam(x_plot)
+            if normalize:
+                y_plot = (y_plot - min(y_plot))
+                y_plot = y_plot / np.sum(y_plot)
+            plot(x_plot, y_plot, c = 'orange', label = "Standard likelihood")
+        if jwa_val:
+            jeff_av, jeff_sig = jwa(data, sigma)
+            print("Jeffreys weighted average:", jeff_av, "+-", jeff_sig)
+            axvline(jeff_av, c = "g", label = "Jeffreys final likelihood")
+            axvline(jeff_av - jeff_sig, c='g', ls = "--")
+            axvline(jeff_av + jeff_sig, c='g', ls = "--")
+        if jwa_loglike:
+            loglike = np.sum([log(erf((x_temp - mu)/(sqrt(2)*s_temp)) / (x_temp-mu)) for x_temp, s_temp in zip(data, sigma)])
+            loglike_lam = lambdify(mu, loglike)
+            y_plot = loglike_lam(x_plot)
+            if normalize:
+                y_plot = (y_plot - min(y_plot))
+                y_plot = y_plot / np.sum(y_plot)
+            plot(x_plot, y_plot, c = 'lime', label = "Jeffreys weighted average")
+        if plot_data:
+            y_min, y_max = gca().get_ylim()
+            y_dist = y_max - y_min
+            y_data = np.linspace(y_min + 0.2 * y_dist, y_min + 0.8 * y_dist, len(data))
+            errorbar(data, y_data, xerr = sigma, ls = "", capsize = 3, marker = ".", label = "data", c = "k")
+        if legendon: legend()
+        if normalize:
+            ylabel("normalized log-likelihood")
+        else:
+            ylabel("log-likelihood")
+        if showon: show()
```

