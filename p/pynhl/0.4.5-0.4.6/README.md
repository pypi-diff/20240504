# Comparing `tmp/pynhl-0.4.5.tar.gz` & `tmp/pynhl-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynhl-0.4.5.tar", last modified: Sun Mar 10 18:01:22 2024, max compression
+gzip compressed data, was "pynhl-0.4.6.tar", last modified: Fri May  3 22:08:26 2024, max compression
```

## Comparing `pynhl-0.4.5.tar` & `pynhl-0.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 18:01:22.005529 pynhl-0.4.5/
--rw-rw-rw-   0        0        0    35149 2019-09-29 22:19:47.000000 pynhl-0.4.5/LICENSE
--rw-rw-rw-   0        0        0      555 2024-03-10 18:01:22.004022 pynhl-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0       64 2019-09-30 00:29:12.000000 pynhl-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 18:01:21.988618 pynhl-0.4.5/pynhl/
--rw-rw-rw-   0        0        0       29 2023-10-18 17:00:04.000000 pynhl-0.4.5/pynhl/__init__.py
--rw-rw-rw-   0        0        0    13580 2024-03-10 17:54:17.000000 pynhl-0.4.5/pynhl/classes.py
-drwxrwxrwx   0        0        0        0 2024-03-10 18:01:22.004022 pynhl-0.4.5/pynhl.egg-info/
--rw-rw-rw-   0        0        0      555 2024-03-10 18:01:21.000000 pynhl-0.4.5/pynhl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-03-10 18:01:21.000000 pynhl-0.4.5/pynhl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 18:01:21.000000 pynhl-0.4.5/pynhl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-10 18:01:21.000000 pynhl-0.4.5/pynhl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-10 18:01:22.008671 pynhl-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      715 2024-03-10 17:56:43.000000 pynhl-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:08:26.099232 pynhl-0.4.6/
+-rw-rw-rw-   0        0        0    35149 2019-09-29 22:19:47.000000 pynhl-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0      555 2024-05-03 22:08:26.098235 pynhl-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0       64 2019-09-30 00:29:12.000000 pynhl-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 22:08:26.087265 pynhl-0.4.6/pynhl/
+-rw-rw-rw-   0        0        0       29 2023-10-18 17:00:04.000000 pynhl-0.4.6/pynhl/__init__.py
+-rw-rw-rw-   0        0        0    13716 2024-05-03 22:05:37.000000 pynhl-0.4.6/pynhl/classes.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:08:26.097237 pynhl-0.4.6/pynhl.egg-info/
+-rw-rw-rw-   0        0        0      555 2024-05-03 22:08:26.000000 pynhl-0.4.6/pynhl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-05-03 22:08:26.000000 pynhl-0.4.6/pynhl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:08:26.000000 pynhl-0.4.6/pynhl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-03 22:08:26.000000 pynhl-0.4.6/pynhl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-03 22:08:26.100443 pynhl-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      715 2024-05-03 21:49:11.000000 pynhl-0.4.6/setup.py
```

### Comparing `pynhl-0.4.5/LICENSE` & `pynhl-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynhl-0.4.5/PKG-INFO` & `pynhl-0.4.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynhl
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for NHL API used in Home Assistant
 Home-page: https://github.com/JayBlackedOut/pynhl
 Author: Jay Lowenthal
 Author-email: jasonlowenthal@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pynhl-0.4.5/pynhl/classes.py` & `pynhl-0.4.6/pynhl/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 for i in range(0, date_count-1):
                     try_date = dt.strptime(data["gamesByDate"][i]["games"][0]["startTimeUTC"],
                                            "%Y-%m-%dT%H:%M:%SZ")
                     if (try_date - dt.utcnow()).days >= -1:
                         output = i
                         break
             except KeyError:
-                pass
+                output = -1
             return output
 
     def game_info(self) -> dict:
         """Parses the json data and returns a dict of game info"""
         response = self.response
         data = self.data
         if response.ok:
@@ -319,14 +319,19 @@
                             "goal_event_id": goal_event_id,
                             "goal_team_name": goal_team_name,
                             "goal_team_abbrev": goal_team_abbrev,
                             "away_score": away_score,
                             "home_score": home_score,
                         }
                         return output
+                    else:
+                        output = {
+                            "away_score": away_score,
+                            "home_score": home_score,
+                        }
                 else:
                     output = {
                         "away_score": away_score,
                         "home_score": home_score,
                     }
                     return output
 
@@ -343,11 +348,9 @@
                 output = {
                     "time_remaining": time_remaining,
                     "current_period": current_period,
                     "away_sog": away_sog,
                     "home_sog": home_sog,
                 }
             except KeyError:
-                output = {
-                    "time_remaining": time_remaining,
-                }
+                output = None
             return output
```

### Comparing `pynhl-0.4.5/pynhl.egg-info/PKG-INFO` & `pynhl-0.4.6/pynhl.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynhl
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python wrapper for NHL API used in Home Assistant
 Home-page: https://github.com/JayBlackedOut/pynhl
 Author: Jay Lowenthal
 Author-email: jasonlowenthal@live.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

