# Comparing `tmp/scrapkit-2.0.tar.gz` & `tmp/scrapkit-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapkit-2.0.tar", last modified: Fri May  3 00:43:08 2024, max compression
+gzip compressed data, was "scrapkit-2.1.tar", last modified: Fri May  3 22:40:18 2024, max compression
```

## Comparing `scrapkit-2.0.tar` & `scrapkit-2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.532441 scrapkit-2.0/
--rw-rw-rw-   0        0        0     2066 2024-05-03 00:43:08.529443 scrapkit-2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.479472 scrapkit-2.0/scrapkit/
--rw-rw-rw-   0        0        0      597 2024-05-03 00:24:13.000000 scrapkit-2.0/scrapkit/__init__.py
--rw-rw-rw-   0        0        0     5819 2024-05-03 00:25:12.000000 scrapkit-2.0/scrapkit/main.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:43:08.527442 scrapkit-2.0/scrapkit.egg-info/
--rw-rw-rw-   0        0        0     2066 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-03 00:43:08.000000 scrapkit-2.0/scrapkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 00:43:08.533439 scrapkit-2.0/setup.cfg
--rw-rw-rw-   0        0        0      457 2024-05-03 00:42:49.000000 scrapkit-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:18.139806 scrapkit-2.1/
+-rw-rw-rw-   0        0        0     1522 2024-05-03 22:40:18.136808 scrapkit-2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:18.088835 scrapkit-2.1/scrapkit/
+-rw-rw-rw-   0        0        0      643 2024-05-03 22:31:17.000000 scrapkit-2.1/scrapkit/__init__.py
+-rw-rw-rw-   0        0        0     6229 2024-05-03 22:22:06.000000 scrapkit-2.1/scrapkit/main.py
+drwxrwxrwx   0        0        0        0 2024-05-03 22:40:18.132810 scrapkit-2.1/scrapkit.egg-info/
+-rw-rw-rw-   0        0        0     1522 2024-05-03 22:40:17.000000 scrapkit-2.1/scrapkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2024-05-03 22:40:17.000000 scrapkit-2.1/scrapkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 22:40:17.000000 scrapkit-2.1/scrapkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-03 22:40:17.000000 scrapkit-2.1/scrapkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-03 22:40:17.000000 scrapkit-2.1/scrapkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 22:40:18.139806 scrapkit-2.1/setup.cfg
+-rw-rw-rw-   0        0        0      475 2024-05-03 22:38:33.000000 scrapkit-2.1/setup.py
```

### Comparing `scrapkit-2.0/scrapkit/__init__.py` & `scrapkit-2.1/scrapkit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 from .main import clickButton
 
 # ScrapKit 2.0
 from .main import getMetaTags
 from .main import getTextFromElement
 from .main import getDataTables
 from .main import getJsonData
-from .main import saveJson
+from .main import saveJson
+
+# ScrapKit 2.1
+from .main import saveFile
```

### Comparing `scrapkit-2.0/scrapkit/main.py` & `scrapkit-2.1/scrapkit/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,16 +116,20 @@
         return None
 
 def getTextFromElement(url, element_tag):
     response = requests.get(url)
     if response.status_code == 200:
         soup = BeautifulSoup(response.text, 'html.parser')
         elements = soup.find_all(element_tag)
-        text_list = [element.text for element in elements]
-        return '\n'.join(text_list)
+        if elements:
+            text_list = [element.text for element in elements]
+            return '\n'.join(text_list)
+        else:
+            print(f"No elements found with tag '{element_tag}'")
+            return None
     else:
         print(f"Failed to fetch text from elements '{element_tag}'. Status code:", response.status_code)
         return None
 
 def getDataTables(url):
     response = requests.get(url)
     if response.status_code == 200:
@@ -160,8 +164,14 @@
     if json_data:
         with open(filename, "w", encoding="utf-8") as file:
             json.dump(json_data, file, indent=4)
         print(f"JSON data saved to {filename}")
     else:
         print("No JSON data to save.")
 
-
+def saveFile(content, filename):
+    try:
+        with open (filename, 'w', encoding = 'utf-8') as f:
+            f.write (content)
+            print (f'Content saved to {filename}')
+    except Exception as e:
+        print (f'Failed to save content to {filename}: {e}')
```

