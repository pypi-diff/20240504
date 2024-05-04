# Comparing `tmp/ayjay-0.1.1.tar.gz` & `tmp/ayjay-0.1.2.tar.gz`

## Comparing `ayjay-0.1.1.tar` & `ayjay-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 ayjay-0.1.1/.python-version
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 ayjay-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ayjay-0.1.1/requirements.lock
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 ayjay-0.1.1/src/ayjay/__init__.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 ayjay-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 ayjay-0.1.1/tests/test_ayjay.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ayjay-0.1.1/.gitignore
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ayjay-0.1.1/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ayjay-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ayjay-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 ayjay-0.1.2/.python-version
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 ayjay-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ayjay-0.1.2/requirements.lock
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 ayjay-0.1.2/src/ayjay/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ayjay-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 ayjay-0.1.2/tests/test_ayjay.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 ayjay-0.1.2/.gitignore
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 ayjay-0.1.2/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ayjay-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 ayjay-0.1.2/PKG-INFO
```

### Comparing `ayjay-0.1.1/requirements-dev.lock` & `ayjay-0.1.2/requirements-dev.lock`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #   with-sources: false
 
 -e file:.
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
+colorama==0.4.6
+    # via pytest
 diskcache==5.6.3
     # via ayjay
 idna==3.6
     # via requests
 iniconfig==2.0.0
     # via pytest
 numpy==1.26.4
```

### Comparing `ayjay-0.1.1/requirements.lock` & `ayjay-0.1.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `ayjay-0.1.1/tests/test_ayjay.py` & `ayjay-0.1.2/tests/test_ayjay.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import pytest
-
-
-# Functionality tests
-def test_ayjay_innit_no_error(ayjay_fixture) -> None:
-    _ = ayjay_fixture
-
-
-def test_ayjay_cached_disabled_innit_no_error(ayjay_fixture_no_cache) -> None:
-    _ = ayjay_fixture_no_cache
-
-
-def test_get_wrong_arg_type_value_error(ayjay_fixture) -> None:
-    with pytest.raises(ValueError):
-        _ = ayjay_fixture.get("http://test.com/", params="Invalid")
-
-
-def test_get_wrong_arg_name_value_error(ayjay_fixture) -> None:
-    with pytest.raises(TypeError):
-        _ = ayjay_fixture.get("http://test.com/", query="Invalid")
-
-
-# Mocked test
-def test_get_correct_response_no_cache(mocker, ayjay_fixture_no_cache) -> None:
-    mocked_endpoint = "http://fakeapi.test.com/"
-    mocked_call_api_value = [
-        {
-            "player_name": "Jordan Mabey",
-            "position": "goalkeeper",
-            "team_name": "Barcelona",
-            "goals_scored": 32,
-            "matches_played": 39,
-        }
-    ]
-
-    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value)
-    actual_mock_response = ayjay_fixture_no_cache.get(
-        mocked_endpoint, params={"fakeParamA": 1, "fakeParamB": 2, "fakeParamC": 1}
-    )
-    assert mocked_call_api_value == actual_mock_response
-
-
-def test_get_correct_response(mocker, ayjay_fixture) -> None:
-    mocked_endpoint = "http://fakeapi.test.com/"
-
-    # call 1
-    mocked_call_api_value_1 = [
-        {
-            "player_name": "Dennie Mulberry",
-            "position": "defender",
-            "team_name": "Manchester United",
-            "goals_scored": 21,
-            "matches_played": 7,
-        }
-    ]
-
-    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value_1)
-    actual_mock_response_1 = ayjay_fixture.get(
-        mocked_endpoint, params={"fakeParamD": 1}
-    )
-    # call 2
-    mocked_call_api_value_2 = [
-        {
-            "player_name": "Hale Jagiela",
-            "position": "defender",
-            "team_name": "Real Madrid",
-            "goals_scored": 11,
-            "matches_played": 10,
-        },
-        {
-            "player_name": "Barby Malham",
-            "position": "goalkeeper",
-            "team_name": "Barcelona",
-            "goals_scored": 33,
-            "matches_played": 14,
-        },
-    ]
-
-    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value_2)
-    actual_mock_response_2 = ayjay_fixture.get(
-        mocked_endpoint, params={"fakeParamD": 2}
-    )
-    assert (
-        mocked_call_api_value_1 == actual_mock_response_1
-        and mocked_call_api_value_2 == actual_mock_response_2
-        and actual_mock_response_1 != actual_mock_response_2
-    )
+import pytest
+
+
+# Functionality tests
+def test_ayjay_innit_no_error(ayjay_fixture) -> None:
+    _ = ayjay_fixture
+
+
+def test_ayjay_cached_disabled_innit_no_error(ayjay_fixture_no_cache) -> None:
+    _ = ayjay_fixture_no_cache
+
+
+def test_get_wrong_arg_type_value_error(ayjay_fixture) -> None:
+    with pytest.raises(ValueError):
+        _ = ayjay_fixture.get("http://test.com/", params="Invalid")
+
+
+def test_get_wrong_arg_name_value_error(ayjay_fixture) -> None:
+    with pytest.raises(TypeError):
+        _ = ayjay_fixture.get("http://test.com/", query="Invalid")
+
+
+# Mocked test
+def test_get_correct_response_no_cache(mocker, ayjay_fixture_no_cache) -> None:
+    mocked_endpoint = "http://fakeapi.test.com/"
+    mocked_call_api_value = [
+        {
+            "player_name": "Jordan Mabey",
+            "position": "goalkeeper",
+            "team_name": "Barcelona",
+            "goals_scored": 32,
+            "matches_played": 39,
+        }
+    ]
+
+    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value)
+    actual_mock_response = ayjay_fixture_no_cache.get(
+        mocked_endpoint, params={"fakeParamA": 1, "fakeParamB": 2, "fakeParamC": 1}
+    )
+    assert mocked_call_api_value == actual_mock_response
+
+
+def test_get_correct_response(mocker, ayjay_fixture) -> None:
+    mocked_endpoint = "http://fakeapi.test.com/"
+
+    # call 1
+    mocked_call_api_value_1 = [
+        {
+            "player_name": "Dennie Mulberry",
+            "position": "defender",
+            "team_name": "Manchester United",
+            "goals_scored": 21,
+            "matches_played": 7,
+        }
+    ]
+
+    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value_1)
+    actual_mock_response_1 = ayjay_fixture.get(
+        mocked_endpoint, params={"fakeParamD": 1}
+    )
+    # call 2
+    mocked_call_api_value_2 = [
+        {
+            "player_name": "Hale Jagiela",
+            "position": "defender",
+            "team_name": "Real Madrid",
+            "goals_scored": 11,
+            "matches_played": 10,
+        },
+        {
+            "player_name": "Barby Malham",
+            "position": "goalkeeper",
+            "team_name": "Barcelona",
+            "goals_scored": 33,
+            "matches_played": 14,
+        },
+    ]
+
+    mocker.patch("ayjay.AyJay.get", return_value=mocked_call_api_value_2)
+    actual_mock_response_2 = ayjay_fixture.get(
+        mocked_endpoint, params={"fakeParamD": 2}
+    )
+    assert (
+        mocked_call_api_value_1 == actual_mock_response_1
+        and mocked_call_api_value_2 == actual_mock_response_2
+        and actual_mock_response_1 != actual_mock_response_2
+    )
```

### Comparing `ayjay-0.1.1/pyproject.toml` & `ayjay-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayjay"
-version = "0.1.1"
+version = "0.1.2"
 description = "Small package for getting cached API requests with propper error handling."
 authors = [
     { name = "Tobias Schnack", email = "tobias.schnack@gmail.com" }
 ]
 dependencies = [
     "requests>=2.31.0",
     "diskcache>=5.6.3",
```

