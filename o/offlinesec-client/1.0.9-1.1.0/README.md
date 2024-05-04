# Comparing `tmp/offlinesec_client-1.0.9.tar.gz` & `tmp/offlinesec_client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "offlinesec_client-1.0.9.tar", last modified: Sat Jul  8 08:52:31 2023, max compression
+gzip compressed data, was "offlinesec_client-1.1.0.tar", last modified: Fri May  3 11:33:42 2024, max compression
```

## Comparing `offlinesec_client-1.0.9.tar` & `offlinesec_client-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.432901 offlinesec_client-1.0.9/
--rw-rw-rw-   0        0        0     3418 2023-07-08 08:52:31.431899 offlinesec_client-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3173 2023-07-08 07:35:59.000000 offlinesec_client-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.424879 offlinesec_client-1.0.9/offlinesec_client/
--rw-rw-rw-   0        0        0       23 2023-07-08 07:39:01.000000 offlinesec_client-1.0.9/offlinesec_client/__init__.py
--rw-rw-rw-   0        0        0       81 2023-07-02 10:37:26.000000 offlinesec_client-1.0.9/offlinesec_client/__main__.py
--rw-rw-rw-   0        0        0     2892 2023-07-07 16:49:27.000000 offlinesec_client-1.0.9/offlinesec_client/config.py
--rw-rw-rw-   0        0        0      219 2023-06-28 20:09:51.000000 offlinesec_client-1.0.9/offlinesec_client/const.py
--rw-rw-rw-   0        0        0     1045 2023-07-07 15:40:58.000000 offlinesec_client-1.0.9/offlinesec_client/func.py
--rw-rw-rw-   0        0        0     3189 2023-07-07 15:46:18.000000 offlinesec_client-1.0.9/offlinesec_client/get_reports.py
--rw-rw-rw-   0        0        0     2414 2023-07-07 15:46:18.000000 offlinesec_client-1.0.9/offlinesec_client/req_notes_report.py
-drwxrwxrwx   0        0        0        0 2023-07-08 08:52:31.430894 offlinesec_client-1.0.9/offlinesec_client.egg-info/
--rw-rw-rw-   0        0        0     3418 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-08 08:52:31.000000 offlinesec_client-1.0.9/offlinesec_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 08:52:31.432901 offlinesec_client-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-07-02 10:22:37.000000 offlinesec_client-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.139343 offlinesec_client-1.1.0/
+-rw-rw-rw-   0        0        0     6793 2024-05-03 11:33:42.138278 offlinesec_client-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6499 2024-05-03 06:54:42.000000 offlinesec_client-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.130898 offlinesec_client-1.1.0/offlinesec_client/
+-rw-rw-rw-   0        0        0       23 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/__init__.py
+-rw-rw-rw-   0        0        0      110 2023-07-14 20:07:51.000000 offlinesec_client-1.1.0/offlinesec_client/__main__.py
+-rw-rw-rw-   0        0        0     4252 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/abap_system.py
+-rw-rw-rw-   0        0        0     4080 2023-10-03 17:05:46.000000 offlinesec_client-1.1.0/offlinesec_client/agr_1251.py
+-rw-rw-rw-   0        0        0     1255 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/bo_system.py
+-rw-rw-rw-   0        0        0     2893 2023-09-14 14:17:57.000000 offlinesec_client-1.1.0/offlinesec_client/config.py
+-rw-rw-rw-   0        0        0      577 2023-09-17 12:59:15.000000 offlinesec_client-1.1.0/offlinesec_client/const.py
+-rw-rw-rw-   0        0        0     1594 2023-10-10 16:14:36.000000 offlinesec_client-1.1.0/offlinesec_client/cwbntcust.py
+-rw-rw-rw-   0        0        0     4342 2023-12-03 15:32:46.000000 offlinesec_client-1.1.0/offlinesec_client/func.py
+-rw-rw-rw-   0        0        0     3435 2023-08-21 06:40:25.000000 offlinesec_client-1.1.0/offlinesec_client/get_reports.py
+-rw-rw-rw-   0        0        0     2235 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/offlinesec_client/java_system.py
+-rw-rw-rw-   0        0        0     1847 2024-04-07 08:20:55.000000 offlinesec_client-1.1.0/offlinesec_client/multi_systems.py
+-rw-rw-rw-   0        0        0     4118 2023-10-21 13:22:58.000000 offlinesec_client-1.1.0/offlinesec_client/req_bo_notes.py
+-rw-rw-rw-   0        0        0     4642 2023-11-17 19:46:10.000000 offlinesec_client-1.1.0/offlinesec_client/req_java_notes.py
+-rw-rw-rw-   0        0        0     4601 2023-10-14 08:09:41.000000 offlinesec_client-1.1.0/offlinesec_client/req_notes_report.py
+-rw-rw-rw-   0        0        0     4652 2023-07-15 08:41:30.000000 offlinesec_client-1.1.0/offlinesec_client/req_param_report.py
+-rw-rw-rw-   0        0        0     1926 2024-04-28 06:12:18.000000 offlinesec_client-1.1.0/offlinesec_client/req_patch_day.py
+-rw-rw-rw-   0        0        0     4060 2023-10-03 20:26:25.000000 offlinesec_client-1.1.0/offlinesec_client/req_roles_report.py
+-rw-rw-rw-   0        0        0     1885 2024-04-28 06:33:53.000000 offlinesec_client-1.1.0/offlinesec_client/req_sec_notes.py
+-rw-rw-rw-   0        0        0     2499 2023-08-21 12:55:22.000000 offlinesec_client-1.1.0/offlinesec_client/resolve_report.py
+-rw-rw-rw-   0        0        0     5092 2024-03-10 09:46:08.000000 offlinesec_client-1.1.0/offlinesec_client/rsparam.py
+-rw-rw-rw-   0        0        0     5028 2023-09-19 06:24:24.000000 offlinesec_client-1.1.0/offlinesec_client/sap_gui.py
+-rw-rw-rw-   0        0        0     2931 2023-11-19 10:07:16.000000 offlinesec_client-1.1.0/offlinesec_client/sap_system.py
+drwxrwxrwx   0        0        0        0 2024-05-03 11:33:42.137245 offlinesec_client-1.1.0/offlinesec_client.egg-info/
+-rw-rw-rw-   0        0        0     6793 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1013 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      578 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      125 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-03 11:33:41.000000 offlinesec_client-1.1.0/offlinesec_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-03 11:33:42.139343 offlinesec_client-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2024-05-03 05:48:17.000000 offlinesec_client-1.1.0/setup.py
```

### Comparing `offlinesec_client-1.0.9/offlinesec_client/config.py` & `offlinesec_client-1.1.0/offlinesec_client/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import os.path
 from pathlib import Path
-from .const import CLIENT_ID, INST_DATE, CONNECTION_STR, APIKEY
+from offlinesec_client.const import CLIENT_ID, INST_DATE, CONNECTION_STR, API_KEY_VALUE, APIKEY, SUBDIR
 import json
 import sysconfig
 
 CONFIG_FILE = "config.json"
 SERVER_NAME = "offlinesec.com"
 PORT = "443"
 ID_LENGTH = 128
-API_KEY = "K3p6Ulx1CZU1x5KPY8edAbLgC2743QztWIbKfPsncQMxo8dyYEt6ug07X2gRS3RgK0AuNEQh0k9ZvpOc5HsR7v39R1XH2EEf1c23tyw5234r91qqFqooFJhfHtbw8K34"
 
 
 class ConfigFile:
     def __init__(self):
-        full_path = os.path.join(sysconfig.get_path('purelib'), 'offlinesec_client', CONFIG_FILE)
+        full_path = os.path.join(Path.home(), SUBDIR, CONFIG_FILE)
         if not Path(full_path).is_file():
             self.create_file(full_path)
 
         self.data = dict()
         self.read_file()
         self.check_params()
 
@@ -29,15 +28,15 @@
         if INST_DATE not in self.data.keys():
             self.data[INST_DATE] = ConfigFile.generate_date()
             flag = True
         if CONNECTION_STR not in self.data.keys():
             self.data[CONNECTION_STR] = ConfigFile.generate_conn_str()
             flag = True
         if APIKEY not in self.data.keys():
-            self.data[APIKEY] = API_KEY
+            self.data[APIKEY] = API_KEY_VALUE
             flag = True
         if flag:
             self.write_file()
 
     @staticmethod
     def generate_conn_str():
         return SERVER_NAME + ":" + PORT
@@ -47,27 +46,31 @@
         config_data = {
             CONNECTION_STR: ConfigFile.generate_conn_str(),
             CLIENT_ID: ConfigFile.generate_client_id(),
             INST_DATE: ConfigFile.generate_date()
         }
         json_data = json.dumps(config_data)
 
+        filepath = os.path.join(Path.home(), SUBDIR)
+        if not os.path.exists(filepath):
+            os.makedirs(filepath)
+
         with open(path, "w") as json_file:
             json_file.write(json_data)
             print("The config file successfully created")
             json_file.close()
 
     def write_file(self):
-        full_path = os.path.join(sysconfig.get_path('purelib'), 'offlinesec_client', CONFIG_FILE)
+        os.makedirs(os.path.dirname(os.path.join(Path.home(), SUBDIR)), exist_ok=True)
+        full_path = os.path.join(Path.home(), SUBDIR, CONFIG_FILE)
         with open(full_path, "w") as json_file:
             json.dump(self.data, json_file)
-            json_file.close()
 
     def read_file(self):
-        full_path = os.path.join(sysconfig.get_path('purelib'), 'offlinesec_client', CONFIG_FILE)
+        full_path = os.path.join(Path.home(), SUBDIR, CONFIG_FILE)
         with open(full_path, "r") as json_file:
             try:
                 data = json.load(json_file)
             except:
                 data = dict()
             json_file.close()
         self.data = data
```

### Comparing `offlinesec_client-1.0.9/offlinesec_client/get_reports.py` & `offlinesec_client-1.1.0/offlinesec_client/get_reports.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os.path
 from pathlib import Path
-from .const import ACTION, FILENAME, ERR_MESSAGE
+from offlinesec_client.const import ACTION, FILENAME, ERR_MESSAGE
 import json
 import time
-from . import func
+import offlinesec_client.func
 import requests
+from offlinesec_client.resolve_report import read_file
 
 UPLOAD_URL = "/get-status"
 ACTION_GET_FILE_NAMES = "GET_REPORTS"
 ACTION_GET_FILE = "GET_FILE"
 ACTION_CONF = "CONFIRMATION"
 
 
 def get_status():
-    if not func.check_server():
+    if not offlinesec_client.func.check_server():
         return
     get_statuses()
 
 
 def get_file_name(filename):
     downloads_path = str(Path.home() / "Downloads")
     full_path = os.path.join(downloads_path, filename)
@@ -31,16 +32,16 @@
         for i in range(1, 100):
             full_path = os.path.join(downloads_path, base + "_" + '%03d' % i + ext)
             if not os.path.isfile(full_path):
                 return full_path
 
 
 def get_statuses():
-    url = func.get_connection_str(UPLOAD_URL)
-    data = func.get_base_json(action=ACTION_GET_FILE_NAMES)
+    url = offlinesec_client.func.get_connection_str(UPLOAD_URL)
+    data = offlinesec_client.func.get_base_json(action=ACTION_GET_FILE_NAMES)
     files = {'json': ('Check available reports to download', json.dumps(data), 'application/json')}
     r = requests.post(url, files=files)
 
     if not r.content:
         print("No answer from server. Please try later")
         return
 
@@ -63,15 +64,15 @@
         for error in response["errors"]:
             print(" * " + error)
 
     print("%s report(s) are available to download from server" % (response["files_num"],))
 
     i = 0
     for file in response["files"]:
-        new_data = func.get_base_json(action=ACTION_GET_FILE)
+        new_data = offlinesec_client.func.get_base_json(action=ACTION_GET_FILE)
         new_data[FILENAME] = file
         print("Downloading the report '%s'" % (file,))
         files = {'json': ('Get file', json.dumps(new_data), 'application/json')}
         r = requests.post(url, files=files)
         full_path = get_file_name(file)
 
         if len(r.content) < 1000:
@@ -80,19 +81,21 @@
 
         if r.content:
             open(full_path, 'wb').write(r.content)
 
         if os.path.isfile(full_path):
             i += 1
             print(" * The report '%s' successfully downloaded (%s bytes)" % (file, len(r.content),))
-            new_data = func.get_base_json(action=ACTION_CONF)
+            new_data = offlinesec_client.func.get_base_json(action=ACTION_CONF)
             new_data[FILENAME] = file
             files = {'json': ('Confirmation', json.dumps(new_data), 'application/json')}
             r = requests.post(url, files=files)
             time.sleep(1)
+            # inverse transformation
+            read_file(full_path)
 
     print("%s report(s) were downloaded. Please check 'Downloads' folder" % (i,))
 
 
 def main():
     get_status()
```

### Comparing `offlinesec_client-1.0.9/offlinesec_client/req_notes_report.py` & `offlinesec_client-1.1.0/offlinesec_client/req_sec_notes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,63 @@
-import requests
 import argparse
+import yaml
+import sys
+import time
 import os
-from . import func
-from .const import ERR_MESSAGE
-import json
-from .const import FILE, SYSTEM_NAME
-
-ALLOWED_EXTENSIONS = ['txt']
-ALLOWED_WITHOUT_EXTENSION = False
-MAX_FILE_SIZE = 200000
-
-UPLOAD_URL = "/file-upload"
-
-
-def check_system_name(s):
-    if len(s) <= 20:
-        return s
-    raise argparse.ArgumentTypeError("The System Name must have length less than 20")
+import offlinesec_client.func
+from offlinesec_client.const import FILE
+from offlinesec_client.multi_systems import process_yaml_file
 
 
-def check_file_arg(s):
-    if not os.path.isfile(s):
-        raise argparse.ArgumentTypeError("File not found")
-
-    ext = s.split('.')[-1].lower()
-    if ext not in ALLOWED_EXTENSIONS:
-        raise argparse.ArgumentTypeError("File extension not supported. Only permitted: %s" %
-                                         (", ".join(ALLOWED_EXTENSIONS)))
+# SUPPORTED_SYSTEMS = ["ABAP", "JAVA", "BO", "HANA"]
+UPLOAD_URL = "/sec-notes"
 
-    if os.path.getsize(s) > MAX_FILE_SIZE:
-        raise argparse.ArgumentTypeError("File too big. Please upload text files")
 
-    return s
+def check_file_arg(s):
+    res = offlinesec_client.func.check_file_arg(s, ['yaml'], 200000)
+    with open(s, 'r') as file:
+        yaml_content = yaml.safe_load(file)
+        if "sap_systems" not in yaml_content:
+            raise argparse.ArgumentTypeError("Wrong the YAML file (%s) structure. The 'sap_systems' key not found" % (s,))
+    return res
 
 
 def init_args():
     parser = argparse.ArgumentParser()
-    parser.add_argument("-f", "--%s" % (FILE,), action="store", type=check_file_arg,
-                        help="File Name (Software Components)", required=True)
-    parser.add_argument("-s", "--%s" % (SYSTEM_NAME,), action="store", type=check_system_name,
-                        help="SAP System Name (max 20 characters)", required=False)
+    parser.add_argument("-f", "--file", action="store", type=check_file_arg,
+                        help="File Name (SAP systems (ABAP, JAVA, BO, ...) and their software components in YAML format)", required=True)
+    parser.add_argument('--wait', action='store_true', help="Wait 5 minutes and download the report")
     parser.parse_args()
     return vars(parser.parse_args())
 
 
-def send_file(file, system_name=""):
-    url = func.get_connection_str(UPLOAD_URL)
-    data = func.get_base_json(system_name=system_name)
-
-    files = {
-        'json': ('description', json.dumps(data), 'application/json'),
-        'file': (os.path.basename(file), open(file, 'rb'), 'application/octet-stream')
-    }
-    print("Uploading file %s" % (os.path.basename(file)))
-    r = requests.post(url, files=files)
-
-    if r.content:
-        try:
-            response = json.loads(r.content)
-            if ERR_MESSAGE in response:
-                print(" * " + response[ERR_MESSAGE])
-                return
-        except:
-            pass
-
-    print("No response from server. Please try later")
-
-
-def send_it(file, system_name=""):
-    if not func.check_server():
-        return
-
-    send_file(file, system_name)
+def print_errors(errors):
+    for error in errors:
+        print(error)
+
+
+def process_it(args):
+    systems = process_yaml_file(args)
+    additional_keys = dict()
+    offlinesec_client.func.send_to_server(systems, UPLOAD_URL, additional_keys)
+
+    wait = args["wait"]
+    if wait:
+        for remaining in range(310, 0, -1):
+            sys.stdout.write("\r")
+            sys.stdout.write("{:2d} seconds remaining.".format(remaining))
+            sys.stdout.flush()
+            time.sleep(1)
+        os.system("offlinesec_get_reports")
 
 
 def main():
     args = init_args()
-    if FILE in args:
-        send_it(args[FILE], args[SYSTEM_NAME])
+    if FILE in args and args[FILE]:
+        process_it(args)
+    else:
+        print("Please choose the configuration YAML file (-f option)")
 
 
 if __name__ == '__main__':
     main()
+
```

