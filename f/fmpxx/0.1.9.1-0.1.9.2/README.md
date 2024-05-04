# Comparing `tmp/fmpxx-0.1.9.1.tar.gz` & `tmp/fmpxx-0.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpxx-0.1.9.1.tar", max compression
+gzip compressed data, was "fmpxx-0.1.9.2.tar", max compression
```

## Comparing `fmpxx-0.1.9.1.tar` & `fmpxx-0.1.9.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      144 2024-03-16 13:29:00.412234 fmpxx-0.1.9.1/README.md
--rw-r--r--   0        0        0       30 2024-03-15 15:06:44.031902 fmpxx-0.1.9.1/fmpxx/__init__.py
--rw-r--r--   0        0        0    15251 2024-03-15 15:50:43.806290 fmpxx-0.1.9.1/fmpxx/client.py
--rw-r--r--   0        0        0      536 2024-03-16 13:16:42.359305 fmpxx-0.1.9.1/fmpxx/company_info.py
--rw-r--r--   0        0        0      520 2024-03-16 13:23:26.547059 fmpxx-0.1.9.1/fmpxx/quote.py
--rw-r--r--   0        0        0      338 2024-03-17 04:11:52.855036 fmpxx-0.1.9.1/pyproject.toml
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 fmpxx-0.1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      203 2024-04-25 14:51:46.390420 fmpxx-0.1.9.2/README.md
+-rw-r--r--   0        0        0       30 2024-03-15 15:06:44.031902 fmpxx-0.1.9.2/fmpxx/__init__.py
+-rw-r--r--   0        0        0    15316 2024-04-19 09:20:48.660639 fmpxx-0.1.9.2/fmpxx/client.py
+-rw-r--r--   0        0        0      536 2024-03-16 13:16:42.359305 fmpxx-0.1.9.2/fmpxx/company_info.py
+-rw-r--r--   0        0        0     4337 2024-04-25 14:46:28.027451 fmpxx-0.1.9.2/fmpxx/financials.py
+-rw-r--r--   0        0        0      866 2024-04-19 09:27:57.003976 fmpxx-0.1.9.2/fmpxx/quote.py
+-rw-r--r--   0        0        0      338 2024-04-25 14:51:12.257842 fmpxx-0.1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 fmpxx-0.1.9.2/PKG-INFO
```

### Comparing `fmpxx-0.1.9.1/fmpxx/client.py` & `fmpxx-0.1.9.2/fmpxx/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         endpoint = f"{self.url}/{endpoint}/{symbol}"
         res = self._handle_response(endpoint, query_params)
         # print(res)
         return res[0]["price"]
 
     def get_quote(self, symbol, endpoint="v3/quote", **query_params):
         """
+        最新版的 api 用这个获取实时包括历史数据
         获取实时报价df
         timestamp请求的是当时的时间戳，如果是盘后请求就会有问题，在real his里去重
         """
         endpoint = f"{self.url}/{endpoint}/{symbol}"
         res = self._handle_response(endpoint, query_params)
         # print(res)
         df = pd.DataFrame.from_records(res)
```

### Comparing `fmpxx-0.1.9.1/fmpxx/company_info.py` & `fmpxx-0.1.9.2/fmpxx/company_info.py`

 * *Files identical despite different names*

