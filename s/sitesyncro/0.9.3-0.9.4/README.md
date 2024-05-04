# Comparing `tmp/sitesyncro-0.9.3.tar.gz` & `tmp/sitesyncro-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesyncro-0.9.3.tar", last modified: Thu May  2 21:15:18 2024, max compression
+gzip compressed data, was "sitesyncro-0.9.4.tar", last modified: Sat May  4 20:50:15 2024, max compression
```

## Comparing `sitesyncro-0.9.3.tar` & `sitesyncro-0.9.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.793726 sitesyncro-0.9.3/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.3/LICENSE
--rw-rw-rw-   0        0        0    11296 2024-05-02 21:15:18.792662 sitesyncro-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0    10362 2024-05-02 21:07:04.000000 sitesyncro-0.9.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 21:15:18.793726 sitesyncro-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1712 2024-04-28 08:59:27.000000 sitesyncro-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.739438 sitesyncro-0.9.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.755927 sitesyncro-0.9.3/src/sitesyncro/
--rw-rw-rw-   0        0        0    39559 2024-05-02 21:00:25.000000 sitesyncro-0.9.3/src/sitesyncro/Model.py
--rw-rw-rw-   0        0        0    19654 2024-05-02 20:25:50.000000 sitesyncro-0.9.3/src/sitesyncro/Sample.py
--rw-rw-rw-   0        0        0      201 2024-05-02 14:33:18.000000 sitesyncro-0.9.3/src/sitesyncro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.789612 sitesyncro-0.9.3/src/sitesyncro/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.3/src/sitesyncro/utils/__init__.py
--rw-rw-rw-   0        0        0    16865 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_cluster.py
--rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_data.py
--rw-rw-rw-   0        0        0     8495 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_load.py
--rw-rw-rw-   0        0        0     3485 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_mp.py
--rw-rw-rw-   0        0        0    11396 2024-05-02 14:33:18.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_oxcal.py
--rw-rw-rw-   0        0        0    13621 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_phase.py
--rw-rw-rw-   0        0        0     5882 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_plot.py
--rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_radiocarbon.py
--rw-rw-rw-   0        0        0     9217 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_simulate.py
--rw-rw-rw-   0        0        0     6192 2024-05-02 17:55:24.000000 sitesyncro-0.9.3/src/sitesyncro/utils/fnc_stat.py
-drwxrwxrwx   0        0        0        0 2024-05-02 21:15:18.791663 sitesyncro-0.9.3/src/sitesyncro.egg-info/
--rw-rw-rw-   0        0        0    11296 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-02 21:15:18.000000 sitesyncro-0.9.3/src/sitesyncro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0    11296 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10362 2024-05-02 21:07:04.000000 sitesyncro-0.9.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1712 2024-05-03 18:25:42.000000 sitesyncro-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.418664 sitesyncro-0.9.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.468764 sitesyncro-0.9.4/src/sitesyncro/
+-rw-rw-rw-   0        0        0    39742 2024-05-04 15:15:10.000000 sitesyncro-0.9.4/src/sitesyncro/Model.py
+-rw-rw-rw-   0        0        0    19654 2024-05-02 20:25:50.000000 sitesyncro-0.9.4/src/sitesyncro/Sample.py
+-rw-rw-rw-   0        0        0      201 2024-05-03 18:25:30.000000 sitesyncro-0.9.4/src/sitesyncro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.588676 sitesyncro-0.9.4/src/sitesyncro/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.4/src/sitesyncro/utils/__init__.py
+-rw-rw-rw-   0        0        0    16964 2024-05-04 12:34:57.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_cluster.py
+-rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_data.py
+-rw-rw-rw-   0        0        0     8495 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_load.py
+-rw-rw-rw-   0        0        0     3648 2024-05-04 16:21:26.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_mp.py
+-rw-rw-rw-   0        0        0    11396 2024-05-02 14:33:18.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_oxcal.py
+-rw-rw-rw-   0        0        0    13621 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_phase.py
+-rw-rw-rw-   0        0        0     5882 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_plot.py
+-rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_radiocarbon.py
+-rw-rw-rw-   0        0        0     8520 2024-05-04 12:47:58.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_simulate.py
+-rw-rw-rw-   0        0        0     7720 2024-05-04 12:22:34.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_stat.py
+drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.598782 sitesyncro-0.9.4/src/sitesyncro.egg-info/
+-rw-rw-rw-   0        0        0    11296 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      668 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/top_level.txt
```

### Comparing `sitesyncro-0.9.3/LICENSE` & `sitesyncro-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/PKG-INFO` & `sitesyncro-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9.3
+Version: 0.9.4
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sitesyncro-0.9.3/README.md` & `sitesyncro-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/setup.py` & `sitesyncro-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="sitesyncro",
-    version="0.9.3",
+    version="0.9.4",
     description="SiteSyncro - Site-specific chronological modeling and synchronization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/demjanp/SiteSyncro",
     author="Peter Demjan",
     author_email="peter.demjan@gmail.com",
     classifiers=[
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro/Model.py` & `sitesyncro-0.9.4/src/sitesyncro/Model.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 	:type oxcal_url: str
 
 	:param overwrite: Flag indicating whether to overwrite existing data in the model directory (default is False).
 	:type overwrite: bool
 	"""
 	
 	def __init__(self, **kwargs):
-
+		
 		defaults = dict(
 			directory='model',
 			samples=[],
 			curve_name='intcal20.14c',
 			phase_model='sequence',
 			cluster_n=-1,
 			min_years_per_cluster=25,
@@ -83,15 +83,15 @@
 		)
 		
 		# Check arguments
 		for key in kwargs:
 			if key not in defaults:
 				raise Exception("Invalid argument: %s" % key)
 			if type(kwargs[key]) != type(defaults[key]):
-				raise Exception("Invalid argument type for %s: %s" % (key, type(kwargs[key].__name__)))
+				raise Exception("Invalid argument type for %s: %s" % (key, type(kwargs[key]).__name__))
 		
 		overwrite = kwargs.pop('overwrite', False)
 		
 		for sample in kwargs.get('samples', []):
 			if not isinstance(sample, Sample):
 				raise Exception("Invalid sample format: %s. Sample expected." % (type(sample).__name__))
 		
@@ -699,19 +699,28 @@
 		:param directory: The directory for the new model.
 		:type directory: str
 		:return: A new instance of the Model class with the same data as the current model but a different directory.
 		:rtype: Model
 
 		"""
 		
-		samples = dict([(name, self.samples[name].copy()) for name in self.samples])
-		model = Model(directory, samples, self.curve_name, self.phase_model,
-					  self.cluster_n, self.min_years_per_cluster, self.uniform, self.p_value, self.uncertainty_base,
-					  self.oxcal_url
-					  )
+		model = Model(
+			directory = directory,
+			samples = [self.samples[name].copy() for name in self.samples],
+			curve_name = self.curve_name,
+			phase_model = self.phase_model,
+			cluster_n = self.cluster_n,
+			min_years_per_cluster = self.min_years_per_cluster,
+			uniform = self.uniform,
+			p_value = self.p_value,
+			uncertainty_base = self.uncertainty_base,
+			npass = self.npass,
+			convergence = self.convergence,
+			oxcal_url = self.oxcal_url
+		)
 		for key in self._calculated():
 			model._data[key] = getattr(self, key)
 		return model
 	
 	def load(self, directory: str = None) -> bool:
 		"""
 		Loads the model from a JSON file.
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro/Sample.py` & `sitesyncro-0.9.4/src/sitesyncro/Sample.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_cluster.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from scipy.spatial.distance import squareform
 from scipy.stats import norm
 from sklearn.decomposition import PCA
 from sklearn.metrics import silhouette_score
 from tqdm import tqdm
 
 from sitesyncro.utils.fnc_mp import (process_mp)
-from sitesyncro.utils.fnc_simulate import (calculate_parameters, generate_random_distributions)
+from sitesyncro.utils.fnc_simulate import (get_params, generate_random_distributions)
 from sitesyncro.utils.fnc_stat import (calc_sum, samples_to_distributions)
 
 
 def calc_distance_matrix(distributions: List[np.ndarray]) -> np.ndarray:
 	"""
 	Calculate a distance matrix of distributions of calibrated C-14 dates based on probabilities
 	that they represent the same event.
@@ -196,18 +196,18 @@
 		)
 	sil = calc_silhouette(D, clusters)
 	clusters = dict([(label, [samples[idx] for idx in clusters[label]]) for label in clusters])
 	
 	return clusters, means, sil
 
 
-def worker_fnc(params: Any, dates_n: int, t_param1: float, t_param2: float, uncertainties: List[float],
-               uncertainty_base: float, curve: np.ndarray, uniform: bool) -> np.ndarray:
-	distributions = generate_random_distributions(dates_n, t_param1, t_param2, uncertainties, uncertainty_base, curve,
-	                                              uniform)
+def worker_fnc(params: Any, dates_n: int, t_mean: float, t_std: float, uncertainties: List[float],
+				uncertainty_base: float, curve: np.ndarray, uniform: bool) -> np.ndarray:
+	
+	distributions = generate_random_distributions(dates_n, t_mean, t_std, uncertainties, uncertainty_base, curve, uniform)
 	D = calc_distance_matrix(distributions)
 	return D
 
 
 def collect_fnc(data: Any, D_pool: List[np.ndarray], pbar: tqdm) -> None:
 	# data = D
 	D_pool.append(data)
@@ -247,16 +247,15 @@
 	dates_n = len(samples)
 	
 	if dates_n < 3:
 		raise Exception("Insufficient number samples for testing of clustering.")
 	
 	print("Testing clustering of %d distributions" % dates_n)
 	
-	sum_obs = calc_sum(distributions)
-	t_param1, t_param2 = calculate_parameters(model.years, sum_obs, model.uniform)
+	t_mean, t_std = get_params(distributions, model.curve, model.uniform)
 	
 	# Get dating range of all samples
 	rng_min, rng_max = np.inf, -np.inf
 	for name in model.samples:
 		rng = model.samples[name].get_range()
 		if None in rng:
 			continue
@@ -293,19 +292,28 @@
 		todo = model.npass
 		with tqdm(total=todo * 2) as pbar:
 			pbar.set_description("Clusters: %d/%d, Conv.: %0.3f" % (cluster_n, clu_max, c))
 			i = -1
 			while True:
 				i += 1
 				while i >= len(D_pool):
-					process_mp(worker_fnc, range(max(4, (todo - len(D_pool)) + 1)),
-					           [dates_n, t_param1, t_param2, model.uncertainties, model.uncertainty_base, model.curve,
-					            model.uniform],
-					           collect_fnc=collect_fnc, collect_args=[D_pool, pbar],
-					           max_cpus=max_cpus, max_queue_size=max_queue_size)
+					n_dists = max(4, (todo - len(D_pool)) + 1)
+					if n_dists > 50:						
+						process_mp(worker_fnc, range(n_dists),
+								   [dates_n, t_mean, t_std, model.uncertainties, model.uncertainty_base, model.curve,
+									model.uniform],
+								   collect_fnc=collect_fnc, collect_args=[D_pool, pbar],
+								   max_cpus=max_cpus, max_queue_size=max_queue_size)
+					else:
+						for j in range(n_dists):
+							D_pool.append(worker_fnc(j, dates_n, t_mean, t_std, model.uncertainties, model.uncertainty_base,
+													 model.curve, model.uniform))
+							pbar.n = len(D_pool)
+							pbar.refresh()
+				
 				D = squareform(D_pool[i])
 				sils_rnd.append(calc_silhouette(D, calc_clusters_hca(D, cluster_n)))
 				pbar.n = len(sils_rnd)
 				pbar.refresh()
 				if len(sils_rnd) >= todo:
 					sils_m = np.array(sils_rnd).mean()
 					if sils_prev is not None:
@@ -334,15 +342,15 @@
 						clusters[cluster_n][label].remove(name)
 						clusters[cluster_n][label] += joined[name]
 	
 	return clusters, means, sils, ps
 
 
 def find_opt_clusters(clusters: Dict[int, Dict[int, List[int]]], ps: Dict[int, float], sils: Dict[int, float],
-                      p_value: float = 0.05) -> int or None:
+					  p_value: float = 0.05) -> int or None:
 	"""
 	Find the optimal number of clusters based on Silhouette scores and p-values of clustering solutions.
 
 	This function takes dictionaries of clusters, p-values, and Silhouette scores, and a p-value threshold as input.
 	It returns the optimal number of clusters that have a p-value less than the threshold and the highest Silhouette score.
 
 	Parameters:
@@ -399,15 +407,15 @@
 		clusters = {model.cluster_n: clusters}
 		means = {model.cluster_n: means}
 		sils = {model.cluster_n: sil}
 		ps = {model.cluster_n: 1}
 		opt_n = model.cluster_n
 	else:
 		clusters, means, sils, ps = test_distribution_clustering(model, max_cpus=max_cpus,
-		                                                         max_queue_size=max_queue_size)
+																 max_queue_size=max_queue_size)
 		opt_n = find_opt_clusters(clusters, ps, sils, model.p_value)
 	if opt_n is None:
 		opt_n = 0
 		clusters[0] = {0: sorted(list(model.samples.keys()))}
 		means[0] = {0: 0}
 		sils[0] = 0
 		ps[0] = 1
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_data.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_data.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_load.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_load.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_mp.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import multiprocessing as mp
+import threading
 import time
 
 from typing import Union, Generator, Callable
 
 
 def _worker(worker_fnc: Callable, params_mp: mp.Queue, collect_mp: mp.Queue, max_queue_size: int, args: list) -> None:
 	while True:
 		try:
-			params = params_mp.get()
+			params = params_mp.get(timeout=10)
+		except mp.Empty:
+			return
 		except:
 			time.sleep(0.01)
 			continue
 		
 		while collect_mp.qsize() > max_queue_size:
 			time.sleep(0.01)
 			pass
 		collect_mp.put(worker_fnc(params, *args))
 
 
 def process_mp(worker_fnc: Callable, params_list: Union[list, Generator], worker_args: list = [],
-               collect_fnc: Callable = None, collect_args: list = [], progress_fnc: Callable = None,
-               progress_args: list = [], max_cpus: int = -1, max_queue_size: int = -1) -> None:
+			   collect_fnc: Callable = None, collect_args: list = [], progress_fnc: Callable = None,
+			   progress_args: list = [], max_cpus: int = -1, max_queue_size: int = -1) -> None:
 	"""
 	Process multiple tasks in parallel using multiprocessing.
 
 	This function takes a worker function and a list of parameters, and applies the worker function to each set of parameters in parallel using multiprocessing. The results are collected and processed by a collector function.
 
 	Parameters:
 	worker_fnc (Callable): The worker function to apply to each set of parameters. It should take a set of parameters and any additional arguments, and return a result.
@@ -44,14 +47,17 @@
 	def call_progress(progress_fnc, done, todo, progress_args):
 		
 		if progress_fnc == True:
 			print("\r%d/%d             " % (done, todo), end="")
 		elif callable(progress_fnc):
 			progress_fnc(done, todo, *progress_args)
 	
+	def start_process(proc):
+		proc.start()
+	
 	params_mp = mp.Queue()
 	todo = 0
 	for params in params_list:
 		params_mp.put(params)
 		todo += 1
 	done = 0
 	collect_mp = mp.Queue(todo)
@@ -59,23 +65,26 @@
 		n_cpus = min(max_cpus, mp.cpu_count() - 1, todo)
 	else:
 		n_cpus = min(mp.cpu_count() - 1, todo)
 	if max_queue_size < 0:
 		max_queue_size = n_cpus * 10
 	call_progress(progress_fnc, done, todo, progress_args)
 	procs = []
+	while len(procs) < n_cpus:
+		procs.append(
+			mp.Process(target=_worker, args=(worker_fnc, params_mp, collect_mp, max_queue_size, worker_args)))
+		threading.Thread(target=start_process, args=(procs[-1],)).start()
 	while done < todo:
-		if len(procs) < n_cpus:
-			procs.append(
-				mp.Process(target=_worker, args=(worker_fnc, params_mp, collect_mp, max_queue_size, worker_args)))
-			procs[-1].start()
 		if not collect_mp.empty():
 			data = collect_mp.get()
 			done += 1
 			call_progress(progress_fnc, done, todo, progress_args)
 			if collect_fnc is not None:
 				collect_fnc(data, *collect_args)
 		else:
 			time.sleep(0.5)
 	for proc in procs:
-		proc.terminate()
+		try:
+			proc.terminate()
+		except:
+			pass
 		proc = None
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_oxcal.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_oxcal.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_phase.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_phase.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_plot.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_plot.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_radiocarbon.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_radiocarbon.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.3/src/sitesyncro/utils/fnc_stat.py` & `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_stat.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,14 +118,65 @@
 			break
 		if mul > max_multiplier:
 			break
 	
 	return [float(v_opt[1]), float(v_opt[0])]
 
 
+def calc_range_approx(years: np.ndarray, distribution: np.ndarray, p: float = 0.9545) -> [int, int] or [None, None]:
+	"""
+	Calculate the range of the given distribution - faster but less precise.
+
+	Parameters:
+	years (np.ndarray): Array of years.
+	distribution (np.ndarray): Array of probabilities for each year.
+	p (float): The desired percentile. Default is 0.9545.
+	p_threshold (float): The threshold for the percentile difference. Default is 0.0001.
+	max_multiplier (int): The maximum multiplier for the number of values. Default is 32.
+
+	Returns:
+	[from, to]: The range of the distribution, or [None, None] if the distribution sum is zero.
+	"""
+	
+	if not distribution.sum():
+		return [None, None]
+	
+	idxs = np.where(distribution > 0.0001)[0]
+	i0, i1 = idxs.min(), idxs.max()
+	years = years[i0:i1]
+	distribution = distribution[i0:i1]
+	
+	thresholds = np.unique(distribution)
+	thresholds.sort()
+	t_prev = thresholds[0]
+	p_sum = 0
+	p_sum_prev = 0
+	mask_prev = None
+	for t in thresholds[::-1]:
+		mask = (distribution > t)
+		if mask_prev is None:
+			mask_prev = mask.copy()
+		p_sum = distribution[mask].sum()
+		if p_sum >= p:
+			break
+		t_prev = t
+		p_sum_prev = p_sum
+		mask_prev = mask.copy()
+	
+	yrs = years[mask]
+	r1, r2 = yrs.max(), yrs.min()
+	yrs = years[mask_prev]
+	rp1, rp2 = yrs.max(), yrs.min()
+	weights = np.array([abs(p - p_sum_prev), abs(p - p_sum)])
+	r1 = np.average([r1, rp1], weights = weights)
+	r2 = np.average([r2, rp2], weights = weights)
+	
+	return [r1, r2]
+
+
 def calc_percentiles(distributions: List[np.ndarray] or np.ndarray, perc_lower: float, perc_upper: float) -> np.ndarray:
 	"""
 	Calculate the lower and upper percentiles of the given distributions.
 
 	Parameters:
 	distributions (List[np.ndarray]): List of distributions.
 	perc_lower (float): The lower percentile.
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro.egg-info/PKG-INFO` & `sitesyncro-0.9.4/src/sitesyncro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9.3
+Version: 0.9.4
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sitesyncro-0.9.3/src/sitesyncro.egg-info/SOURCES.txt` & `sitesyncro-0.9.4/src/sitesyncro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

