# Comparing `tmp/rp2040home-0.1.0.tar.gz` & `tmp/rp2040home-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2040home-0.1.0.tar", last modified: Tue Apr 30 10:09:16 2024, max compression
+gzip compressed data, was "rp2040home-0.1.4.tar", last modified: Sat May  4 08:44:47 2024, max compression
```

## Comparing `rp2040home-0.1.0.tar` & `rp2040home-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.731684 rp2040home-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-01-08 07:40:07.000000 rp2040home-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      373 2024-04-30 10:09:16.727694 rp2040home-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2506 2024-03-29 08:46:49.000000 rp2040home-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.543847 rp2040home-0.1.0/RP2040Home/
--rw-rw-rw-   0        0        0     2641 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/RP2040Home.py
--rw-rw-rw-   0        0        0       58 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.645376 rp2040home-0.1.0/RP2040Home/configparsing/
--rw-rw-rw-   0        0        0      118 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/__init__.py
--rw-rw-rw-   0        0        0     1497 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/configparser.py
--rw-rw-rw-   0        0        0      195 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/homeassistantdiscoveryconfig.py
--rw-rw-rw-   0        0        0      672 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/mqttconfig.py
--rw-rw-rw-   0        0        0      379 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/output.py
--rw-rw-rw-   0        0        0      170 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/configparsing/wificonfig.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.672303 rp2040home-0.1.0/RP2040Home/homeassistant/
--rw-rw-rw-   0        0        0        0 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/homeassistant/__init__.py
--rw-rw-rw-   0        0        0     4263 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/homeassistant/discoveryPayload.py
--rw-rw-rw-   0        0        0      611 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/homeassistant/disoveryDevice.py
--rw-rw-rw-   0        0        0     3038 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/homeassistant/mqttClient.py
--rw-rw-rw-   0        0        0     2972 2024-04-30 09:46:48.000000 rp2040home-0.1.0/RP2040Home/homeassistant/payloadGenerator.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.710609 rp2040home-0.1.0/RP2040Home.egg-info/
--rw-rw-rw-   0        0        0      373 2024-04-30 10:09:16.000000 rp2040home-0.1.0/RP2040Home.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      756 2024-04-30 10:09:16.000000 rp2040home-0.1.0/RP2040Home.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 10:09:16.000000 rp2040home-0.1.0/RP2040Home.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-30 10:09:16.000000 rp2040home-0.1.0/RP2040Home.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 10:09:16.735674 rp2040home-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      418 2024-04-30 10:09:02.000000 rp2040home-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.677291 rp2040home-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2024-03-27 11:35:12.000000 rp2040home-0.1.0/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 10:09:16.698235 rp2040home-0.1.0/test/config_parsing/
--rw-rw-rw-   0        0        0     1822 2024-04-30 09:46:48.000000 rp2040home-0.1.0/test/config_parsing/ConfigParserTest.py
--rw-rw-rw-   0        0        0        0 2024-03-27 11:35:12.000000 rp2040home-0.1.0/test/config_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-04 08:44:31.000000 rp2040home-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-04 08:44:47.739096 rp2040home-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-04 08:44:31.000000 rp2040home-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.735096 rp2040home-0.1.4/RP2040Home/
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/RP2040Home.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/RP2040Home/configparsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/homeassistantdiscoveryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/mqttconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/configparsing/wificonfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/RP2040Home/homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/homeassistant/discoveryPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/homeassistant/disoveryDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/homeassistant/mqttClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-04 08:44:31.000000 rp2040home-0.1.4/RP2040Home/homeassistant/payloadGenerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/RP2040Home.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-04 08:44:47.000000 rp2040home-0.1.4/RP2040Home.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-04 08:44:47.000000 rp2040home-0.1.4/RP2040Home.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 08:44:47.000000 rp2040home-0.1.4/RP2040Home.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-04 08:44:47.000000 rp2040home-0.1.4/RP2040Home.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 08:44:47.739096 rp2040home-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-04 08:44:31.000000 rp2040home-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:31.000000 rp2040home-0.1.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:47.739096 rp2040home-0.1.4/test/config_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-04 08:44:31.000000 rp2040home-0.1.4/test/config_parsing/ConfigParserTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 08:44:31.000000 rp2040home-0.1.4/test/config_parsing/__init__.py
```

### Comparing `rp2040home-0.1.0/LICENSE` & `rp2040home-0.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 ESteanes
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 ESteanes
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `rp2040home-0.1.0/README.md` & `rp2040home-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# mqtt-home
-A simple micro-python mqtt client which enables simple plug-and-play functionality and interoperability with Home Assistant. 
-```  
-"availability_topic": "home/wateringsystem/back/status",
-"state_topic": "home/wateringsystem/back/output/solenoid3",
-"command_topic": "home/wateringsystem/back/output/solenoid3/set",
-```
-
-The overall standard of MQTT topics that will be used going forward is:
-`<area>/<entity>/<location>/<property>/<object>/<modifier>` but there's no set requirement on structure.
-
-topic_prefix is: `<area>/<entity>/<location>`
-
-This simplifies it down to:
-`<topic_prefix>/<property>/<object>/<modifier>`
-
-# Software Setup
-## From a fresh Raspberry Pi Pico
-Following the [official Raspberry Pi Docs](https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/3)
-1. Hold down the bootsel button while plugging in pi pico for the first time
-2. Open Thonny with the pico plugged in
-3. Choose the micropython language selector in the bottom right hand corner of the UI
-4. Choose the latest version of Micropython and install it onto the raspberry pi
-## From an existing Raspberry Pi Pico with micropython installed
-5. In the top bar of Thonny, under `Tools`, there should be an option to `Manage Packages`, select that option
-6. Then search for `umqtt` in the package manager, there should be one called `micropython-umqtt.simple` and install it onto the Pi Pico.
-	1. You could potentially use [mpremote](https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mpremote) `mpremote mip install micropython-umqtt.simple` (untested) in the Thonny console when the Pi Pico is connected
-8. Clone the [mqtt-home](https://github.com/ESteanes/mqtt-home) repository to a local area
-9. Create an appropriate `config.json` file based off the `test-config.json`
-10. Upload `config.json`, `main.py`, `boot.py` and `main` to the Pi Pico
-11. Manually run `boot.py` and `main.py` in Thonny to ensure that the SSID and password are correct, in addition to the Home Assistant connection.
-12. Once confirmed connected, disconnect the Pi Pico and plug it in from cold to ensure that the start up works as expected.
-13. Once the status LED is shining, that is an indication that `main.py` is running and the Pi Pico should be up and running!
-
-## Virtual Environment Setup
-* Using a virtual environment, install the python dependencies listed in `requirements.txt` by running `python -m pip install -r requirements.txt`
+# mqtt-home
+A simple micro-python mqtt client which enables simple plug-and-play functionality and interoperability with Home Assistant. 
+```  
+"availability_topic": "home/wateringsystem/back/status",
+"state_topic": "home/wateringsystem/back/output/solenoid3",
+"command_topic": "home/wateringsystem/back/output/solenoid3/set",
+```
+
+The overall standard of MQTT topics that will be used going forward is:
+`<area>/<entity>/<location>/<property>/<object>/<modifier>` but there's no set requirement on structure.
+
+topic_prefix is: `<area>/<entity>/<location>`
+
+This simplifies it down to:
+`<topic_prefix>/<property>/<object>/<modifier>`
+
+# Software Setup
+## From a fresh Raspberry Pi Pico
+Following the [official Raspberry Pi Docs](https://projects.raspberrypi.org/en/projects/getting-started-with-the-pico/3)
+1. Hold down the bootsel button while plugging in pi pico for the first time
+2. Open Thonny with the pico plugged in
+3. Choose the micropython language selector in the bottom right hand corner of the UI
+4. Choose the latest version of Micropython and install it onto the raspberry pi
+## From an existing Raspberry Pi Pico with micropython installed
+5. In the top bar of Thonny, under `Tools`, there should be an option to `Manage Packages`, select that option
+6. Then search for `umqtt` in the package manager, there should be one called `micropython-umqtt.simple` and install it onto the Pi Pico.
+	1. You could potentially use [mpremote](https://docs.micropython.org/en/latest/reference/packages.html#installing-packages-with-mpremote) `mpremote mip install micropython-umqtt.simple` (untested) in the Thonny console when the Pi Pico is connected
+8. Clone the [mqtt-home](https://github.com/ESteanes/mqtt-home) repository to a local area
+9. Create an appropriate `config.json` file based off the `test-config.json`
+10. Upload `config.json`, `main.py`, `boot.py` and `main` to the Pi Pico
+11. Manually run `boot.py` and `main.py` in Thonny to ensure that the SSID and password are correct, in addition to the Home Assistant connection.
+12. Once confirmed connected, disconnect the Pi Pico and plug it in from cold to ensure that the start up works as expected.
+13. Once the status LED is shining, that is an indication that `main.py` is running and the Pi Pico should be up and running!
+
+## Virtual Environment Setup
+* Using a virtual environment, install the python dependencies listed in `requirements.txt` by running `python -m pip install -r requirements.txt`
```

### Comparing `rp2040home-0.1.0/RP2040Home/configparsing/configparser.py` & `rp2040home-0.1.4/RP2040Home/configparsing/configparser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from .mqttconfig import MqttConfig
-from .output import Output
-from .wificonfig import WifiConfig
-import json
-
-class ConfigParser:
-    wifi_config: list[WifiConfig]
-    mqtt_config: MqttConfig
-    output_config: list[Output]
-    allowed_pins = [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,26,27,28]
-    def load(self, path_to_file):
-        with open(path_to_file, "r") as stream:
-            config = json.loads(stream.read())
-            self.wifi_config = [WifiConfig(wifiConfig["ssid"], wifiConfig["password"]) for wifiConfig in config['pi']]
-            self.mqtt_config = MqttConfig(**config['mqtt'])
-            if config['digital_outputs']:
-                self.output_config = [
-                    Output(
-                        x["output_type"],
-                        x['name'],
-                        x['pin'],
-                        x['on_payload'],
-                        x['off_payload']
-                    ) for x in config['digital_outputs'] if x['pin'] in self.allowed_pins]
-                
-            if len(self.output_config) == 0 and len(config['digital_outputs']) == 0:
-                print("No digital outputs")
-            if len(self.output_config) == 0 and len(config['digital_outputs']) != 0:
-                print("No valid digital outputs - choose a valid GPIO pin")
-            try:
-                print(config)
-            except json.JSONDecodeError as exc:
-                print(exc)
-        return self
+from .mqttconfig import MqttConfig
+from .output import Output
+from .wificonfig import WifiConfig
+import json
+
+class ConfigParser:
+    wifi_config: list[WifiConfig]
+    mqtt_config: MqttConfig
+    output_config: list[Output]
+    allowed_pins = [0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,26,27,28]
+    def load(self, path_to_file):
+        with open(path_to_file, "r") as stream:
+            config = json.loads(stream.read())
+            self.wifi_config = [WifiConfig(wifiConfig["ssid"], wifiConfig["password"]) for wifiConfig in config['pi']]
+            self.mqtt_config = MqttConfig(**config['mqtt'])
+            if config['digital_outputs']:
+                self.output_config = [
+                    Output(
+                        x["output_type"],
+                        x['name'],
+                        x['pin'],
+                        x['on_payload'],
+                        x['off_payload']
+                    ) for x in config['digital_outputs'] if x['pin'] in self.allowed_pins]
+                
+            if len(self.output_config) == 0 and len(config['digital_outputs']) == 0:
+                print("No digital outputs")
+            if len(self.output_config) == 0 and len(config['digital_outputs']) != 0:
+                print("No valid digital outputs - choose a valid GPIO pin")
+            try:
+                print(config)
+            except json.JSONDecodeError as exc:
+                print(exc)
+        return self
```

### Comparing `rp2040home-0.1.0/RP2040Home/homeassistant/discoveryPayload.py` & `rp2040home-0.1.4/RP2040Home/homeassistant/discoveryPayload.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from .disoveryDevice import DiscoveryDevice
-        
-class DiscoveryPayload:
-    name: str
-    availability_topic: str
-    payload_available = "running"
-    payload_not_available = "dead"
-    device: DiscoveryDevice
-    unique_id: str
-    state_topic: str
-    command_topic: str
-    payload_on: str
-    payload_off: str
-    
-    def __init__(self, name:str, availability_topic:str, payload_available: str, payload_not_available: str, device: any, unique_id: str, state_topic: str, command_topic: str, payload_on: str, payload_off: str):
-        self.name = name
-        self.availability_topic = availability_topic
-        self.payload_available = payload_available
-        self.payload_not_available = payload_not_available
-        self.device = device
-        self.unique_id = unique_id
-        self.state_topic = state_topic
-        self.command_topic = command_topic
-        self.payload_on = payload_on
-        self.payload_off = payload_off
-    
-    '''
-    Should return something along the lines of:
-    {
-            "name": "output_name",
-            "availability_topic": "availability_topic",
-            "payload_available": "running",
-            "payload_not_available": "dead",
-            "device": {
-                "manufacturer": "manufacturer_name",
-                "model": "v0",
-                "identifiers": [
-                    "identifier_1"
-                ],
-                "name": "device_name"
-            },
-            "unique_id": "uuid",
-            "state_topic": "state_topic",
-            "command_topic": "command_topic",
-            "payload_on": "ON",
-            "payload_off": "OFF"
-        }
-    '''
-    def return_map(self):
-        return {  # Thoughts: this should be its own class and then the class has a method to return all of the key values as a json
-            "name": self.name,
-            "availability_topic": self.availability_topic,
-            "payload_available": self.payload_available,
-            "payload_not_available": self.payload_not_available,
-            "device": self.device.jsonPayload(),
-            "unique_id": self.unique_id,
-            "state_topic": self.state_topic,
-            "command_topic": self.command_topic,
-            "payload_on": self.payload_on,
-            "payload_off": self.payload_off
-        }
-
-
-class HomeAssistantDiscoveryBuilder:
-    def __init__(self):
-        self.name = ""
-        self.availability_topic = ""
-        self.payload_available = "running"
-        self.payload_not_available = "dead"
-        self.device = ""
-        self.unique_id = ""
-        self.state_topic = ""
-        self.command_topic = ""
-        self.payload_on = ""
-        self.payload_off = ""
-
-    def set_name(self, name):
-        self.name = name
-        return self
-
-    def set_availability_topic(self, availability_topic):
-        self.availability_topic = availability_topic
-        return self
-
-    def set_payload_available(self, payload_available):
-        self.payload_available = payload_available
-        return self
-
-    def set_payload_not_available(self, payload_not_available):
-        self.payload_not_available = payload_not_available
-        return self
-
-    def set_device(self, device):
-        self.device = device
-        return self
-
-    def set_unique_id(self, unique_id):
-        self.unique_id = unique_id
-        return self
-
-    def set_state_topic(self, state_topic):
-        self.state_topic = state_topic
-        return self
-
-    def set_command_topic(self, command_topic):
-        self.command_topic = command_topic
-        return self
-
-    def set_payload_on(self, payload_on):
-        self.payload_on = payload_on
-        return self
-
-    def set_payload_off(self, payload_off):
-        self.payload_off = payload_off
-        return self
-
-    def build(self):
-        return DiscoveryPayload(
-            self.name,
-            self.availability_topic,
-            self.payload_available,
-            self.payload_not_available,
-            self.device,
-            self.unique_id,
-            self.state_topic,
-            self.command_topic,
-            self.payload_on,
-            self.payload_off
+from .disoveryDevice import DiscoveryDevice
+        
+class DiscoveryPayload:
+    name: str
+    availability_topic: str
+    payload_available = "running"
+    payload_not_available = "dead"
+    device: DiscoveryDevice
+    unique_id: str
+    state_topic: str
+    command_topic: str
+    payload_on: str
+    payload_off: str
+    
+    def __init__(self, name:str, availability_topic:str, payload_available: str, payload_not_available: str, device: any, unique_id: str, state_topic: str, command_topic: str, payload_on: str, payload_off: str):
+        self.name = name
+        self.availability_topic = availability_topic
+        self.payload_available = payload_available
+        self.payload_not_available = payload_not_available
+        self.device = device
+        self.unique_id = unique_id
+        self.state_topic = state_topic
+        self.command_topic = command_topic
+        self.payload_on = payload_on
+        self.payload_off = payload_off
+    
+    '''
+    Should return something along the lines of:
+    {
+            "name": "output_name",
+            "availability_topic": "availability_topic",
+            "payload_available": "running",
+            "payload_not_available": "dead",
+            "device": {
+                "manufacturer": "manufacturer_name",
+                "model": "v0",
+                "identifiers": [
+                    "identifier_1"
+                ],
+                "name": "device_name"
+            },
+            "unique_id": "uuid",
+            "state_topic": "state_topic",
+            "command_topic": "command_topic",
+            "payload_on": "ON",
+            "payload_off": "OFF"
+        }
+    '''
+    def return_map(self):
+        return {  # Thoughts: this should be its own class and then the class has a method to return all of the key values as a json
+            "name": self.name,
+            "availability_topic": self.availability_topic,
+            "payload_available": self.payload_available,
+            "payload_not_available": self.payload_not_available,
+            "device": self.device.jsonPayload(),
+            "unique_id": self.unique_id,
+            "state_topic": self.state_topic,
+            "command_topic": self.command_topic,
+            "payload_on": self.payload_on,
+            "payload_off": self.payload_off
+        }
+
+
+class HomeAssistantDiscoveryBuilder:
+    def __init__(self):
+        self.name = ""
+        self.availability_topic = ""
+        self.payload_available = "running"
+        self.payload_not_available = "dead"
+        self.device = ""
+        self.unique_id = ""
+        self.state_topic = ""
+        self.command_topic = ""
+        self.payload_on = ""
+        self.payload_off = ""
+
+    def set_name(self, name):
+        self.name = name
+        return self
+
+    def set_availability_topic(self, availability_topic):
+        self.availability_topic = availability_topic
+        return self
+
+    def set_payload_available(self, payload_available):
+        self.payload_available = payload_available
+        return self
+
+    def set_payload_not_available(self, payload_not_available):
+        self.payload_not_available = payload_not_available
+        return self
+
+    def set_device(self, device):
+        self.device = device
+        return self
+
+    def set_unique_id(self, unique_id):
+        self.unique_id = unique_id
+        return self
+
+    def set_state_topic(self, state_topic):
+        self.state_topic = state_topic
+        return self
+
+    def set_command_topic(self, command_topic):
+        self.command_topic = command_topic
+        return self
+
+    def set_payload_on(self, payload_on):
+        self.payload_on = payload_on
+        return self
+
+    def set_payload_off(self, payload_off):
+        self.payload_off = payload_off
+        return self
+
+    def build(self):
+        return DiscoveryPayload(
+            self.name,
+            self.availability_topic,
+            self.payload_available,
+            self.payload_not_available,
+            self.device,
+            self.unique_id,
+            self.state_topic,
+            self.command_topic,
+            self.payload_on,
+            self.payload_off
         )
```

### Comparing `rp2040home-0.1.0/RP2040Home/homeassistant/mqttClient.py` & `rp2040home-0.1.4/RP2040Home/homeassistant/mqttClient.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import json, machine
-from umqtt.simple import MQTTClient
-from RP2040Home.configparsing.output import Output
-
-
-class MqttClient:
-    def __init__(self, outputs: list[Output], haDiscoveryPayloads: list[map], haDiscoveryTopics: list[str], setTopicMap:map[map], mqttClient: MQTTClient, ioInteractor: machine) -> None:
-        self.outputs = outputs
-        self.haDiscoveryPayloads = haDiscoveryPayloads
-        self.haDiscoveryTopics = haDiscoveryTopics
-        self.setTopicMap = setTopicMap
-        self.ioInteractor = ioInteractor
-        self.mqttClient = mqttClient
-            
-    def defaultOutputsToOff(self) -> None:
-        for output in self.outputs:
-            self.ioInteractor.Pin(output.pin, self.ioInteractor.Pin.OUT).off()
-        for payload in self.haDiscoveryPayloads:
-            self.publish(payload["state_topic"], payload["payload_off"])
-    
-    def mqttStatus(self, isAvailable) -> None:
-        for haDiscovery in self.haDiscoveryPayloads:
-            if isAvailable:
-                self.publish(
-                    haDiscovery["availability_topic"], haDiscovery["payload_available"])
-                continue
-            self.publish(haDiscovery["availability_topic"], haDiscovery["payload_not_available"])
-
-    def mqttHADiscoveryPost(self) -> None:
-        for discoveryPayload, haDiscoveryTopic in zip(self.haDiscoveryPayloads, self.haDiscoveryTopics):
-            disoveryPayloadString = json.dumps(discoveryPayload)
-            self.publish(haDiscoveryTopic, disoveryPayloadString)
-            print("publishing to:" + haDiscoveryTopic)
-            print("discovery payload:" + disoveryPayloadString)
-            self.mqttClient.subscribe(discoveryPayload["command_topic"])
-            print("subscribing to:" + discoveryPayload["command_topic"])
-
-    def action(self, topic, msg) -> None:
-        topicString = topic.decode()
-        msgString = msg.decode()
-        print("Topic: " + topicString + "; Message: " + msgString)
-        if self.setTopicMap.get(topicString) is None:
-            return
-        topicOutput = self.setTopicMap.get(topicString).get("output")
-        topicStateTopic = self.setTopicMap.get(topicString).get("state_topic")
-        self.publish(topicStateTopic, msgString)
-        if msgString == topicOutput.on_payload:
-            self.ioInteractor.Pin(topicOutput.pin, self.ioInteractor.Pin.OUT).on()
-            return
-        if msgString == topicOutput.off_payload:
-            self.ioInteractor.Pin(topicOutput.pin, self.ioInteractor.Pin.OUT).off()
-            return
-        print("did not match either on or off payload - error")
-            
-
-    def mqttInitialise(self, isAvailable) -> None:
-        self.mqttClient.set_callback(self.action)
-        self.mqttClient.connect()
-        self.mqttHADiscoveryPost()
-        self.defaultOutputsToOff()
-        self.mqttStatus(isAvailable)
-        
-    
-    def publish(self, topic: str, payload: any) -> None:
-        self.mqttClient.publish(topic, payload)
+import json, machine
+from umqtt.simple import MQTTClient
+from RP2040Home.configparsing.output import Output
+
+
+class MqttClient:
+    def __init__(self, outputs: list[Output], haDiscoveryPayloads: list[map], haDiscoveryTopics: list[str], setTopicMap:map[map], mqttClient: MQTTClient, ioInteractor: machine) -> None:
+        self.outputs = outputs
+        self.haDiscoveryPayloads = haDiscoveryPayloads
+        self.haDiscoveryTopics = haDiscoveryTopics
+        self.setTopicMap = setTopicMap
+        self.ioInteractor = ioInteractor
+        self.mqttClient = mqttClient
+            
+    def defaultOutputsToOff(self) -> None:
+        for output in self.outputs:
+            self.ioInteractor.Pin(output.pin, self.ioInteractor.Pin.OUT).off()
+        for payload in self.haDiscoveryPayloads:
+            self.publish(payload["state_topic"], payload["payload_off"])
+    
+    def mqttStatus(self, isAvailable) -> None:
+        for haDiscovery in self.haDiscoveryPayloads:
+            if isAvailable:
+                self.publish(
+                    haDiscovery["availability_topic"], haDiscovery["payload_available"])
+                continue
+            self.publish(haDiscovery["availability_topic"], haDiscovery["payload_not_available"])
+
+    def mqttHADiscoveryPost(self) -> None:
+        for discoveryPayload, haDiscoveryTopic in zip(self.haDiscoveryPayloads, self.haDiscoveryTopics):
+            disoveryPayloadString = json.dumps(discoveryPayload)
+            self.publish(haDiscoveryTopic, disoveryPayloadString)
+            print("publishing to:" + haDiscoveryTopic)
+            print("discovery payload:" + disoveryPayloadString)
+            self.mqttClient.subscribe(discoveryPayload["command_topic"])
+            print("subscribing to:" + discoveryPayload["command_topic"])
+
+    def action(self, topic, msg) -> None:
+        topicString = topic.decode()
+        msgString = msg.decode()
+        print("Topic: " + topicString + "; Message: " + msgString)
+        if self.setTopicMap.get(topicString) is None:
+            return
+        topicOutput = self.setTopicMap.get(topicString).get("output")
+        topicStateTopic = self.setTopicMap.get(topicString).get("state_topic")
+        self.publish(topicStateTopic, msgString)
+        if msgString == topicOutput.on_payload:
+            self.ioInteractor.Pin(topicOutput.pin, self.ioInteractor.Pin.OUT).on()
+            return
+        if msgString == topicOutput.off_payload:
+            self.ioInteractor.Pin(topicOutput.pin, self.ioInteractor.Pin.OUT).off()
+            return
+        print("did not match either on or off payload - error")
+            
+
+    def mqttInitialise(self, isAvailable) -> None:
+        self.mqttClient.set_callback(self.action)
+        self.mqttClient.connect()
+        self.mqttHADiscoveryPost()
+        self.defaultOutputsToOff()
+        self.mqttStatus(isAvailable)
+        
+    
+    def publish(self, topic: str, payload: any) -> None:
+        self.mqttClient.publish(topic, payload)
```

### Comparing `rp2040home-0.1.0/RP2040Home/homeassistant/payloadGenerator.py` & `rp2040home-0.1.4/RP2040Home/homeassistant/payloadGenerator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from umqtt.simple import MQTTClient
-from .discoveryPayload import HomeAssistantDiscoveryBuilder
-from .disoveryDevice import DiscoveryDevice
-from RP2040Home.configparsing.output import Output
-from RP2040Home.configparsing.configparser import ConfigParser
-from RP2040Home.configparsing.homeassistantdiscoveryconfig import HomeAssistantDiscoveryConfig
-import json, machine, ubinascii, network
-
-class PayloadGenerator:
-    topic_prefix: str
-    outputs: list[Output]
-    ha_discovery: HomeAssistantDiscoveryConfig
-    location: str
-    UUID: str
-    haDiscoveryTopics: list[str]
-    
-    def __init__(self, parsedConfig: ConfigParser):
-        # UUID cannot contain colons from mac address https://www.home-assistant.io/integrations/mqtt/#discovery-topic
-        self.UUID = "RPi2040Home-" + ubinascii.hexlify(network.WLAN().config('mac')).decode() 
-        self.topic_prefix = parsedConfig.mqtt_config.topic_prefix
-        self.outputs = parsedConfig.output_config
-        self.ha_discovery = parsedConfig.mqtt_config.ha_discovery
-        self.location = parsedConfig.mqtt_config.location
-        self.haDiscoveryPayloads = []
-        self.haDiscoveryTopics = []
-        self.setTopicMap = {}
-        if self.ha_discovery.enabled != None:
-            self.createDiscoveryPayloads()
-
-    def createDiscoveryPayloads(self) -> None:
-        for output in self.outputs:
-            state_topic = self.location+"/output/"+output.name
-            command_topic = self.location+"/output/"+output.name+"/set"
-            outputDiscoveryPayload =  HomeAssistantDiscoveryBuilder()\
-            .set_name(output.name)\
-            .set_availability_topic(self.topic_prefix + "/status")\
-            .set_device(
-                DiscoveryDevice(
-                    "Home Assistant MQTT Client",
-                    "v0",
-                    ["Home Assistant MQTT Client", "Home Assistant MQTT Client-"+self.UUID],
-                    "Home Assistant MQTT Client")
-                )\
-            .set_unique_id(self.UUID + "-" + output.name)\
-            .set_state_topic(state_topic)\
-            .set_command_topic(command_topic)\
-            .set_payload_on(output.on_payload)\
-            .set_payload_off(output.off_payload)\
-            .build().return_map()
-            self.haDiscoveryPayloads.append(outputDiscoveryPayload)
-            self.setTopicMap[command_topic] = {"state_topic": state_topic, "output": output}
-            self.haDiscoveryTopics.append("homeassistant/" + output.output_type + "/" + self.ha_discovery.node_id + "-" + self.UUID + "/"+output.name+"/config")
-           
-    def getUUID(self) -> str:
-        return self.UUID
-    
-    def getDiscoveryPayloads(self) -> list[map]:
-        return self.haDiscoveryPayloads
-    
-    def getDiscoveryTopics(self) -> list[str]:
-        return self.haDiscoveryTopics
-    
-    def getSetTopicMap(self) -> map[map]:
-        return self.setTopicMap
-    
+from umqtt.simple import MQTTClient
+from .discoveryPayload import HomeAssistantDiscoveryBuilder
+from .disoveryDevice import DiscoveryDevice
+from RP2040Home.configparsing.output import Output
+from RP2040Home.configparsing.configparser import ConfigParser
+from RP2040Home.configparsing.homeassistantdiscoveryconfig import HomeAssistantDiscoveryConfig
+import json, machine, ubinascii, network
+
+class PayloadGenerator:
+    topic_prefix: str
+    outputs: list[Output]
+    ha_discovery: HomeAssistantDiscoveryConfig
+    location: str
+    UUID: str
+    haDiscoveryTopics: list[str]
+    
+    def __init__(self, parsedConfig: ConfigParser):
+        # UUID cannot contain colons from mac address https://www.home-assistant.io/integrations/mqtt/#discovery-topic
+        self.UUID = "RPi2040Home-" + ubinascii.hexlify(network.WLAN().config('mac')).decode() 
+        self.topic_prefix = parsedConfig.mqtt_config.topic_prefix
+        self.outputs = parsedConfig.output_config
+        self.ha_discovery = parsedConfig.mqtt_config.ha_discovery
+        self.location = parsedConfig.mqtt_config.location
+        self.haDiscoveryPayloads = []
+        self.haDiscoveryTopics = []
+        self.setTopicMap = {}
+        if self.ha_discovery.enabled != None:
+            self.createDiscoveryPayloads()
+
+    def createDiscoveryPayloads(self) -> None:
+        for output in self.outputs:
+            state_topic = self.location+"/output/"+output.name
+            command_topic = self.location+"/output/"+output.name+"/set"
+            outputDiscoveryPayload =  HomeAssistantDiscoveryBuilder()\
+            .set_name(output.name)\
+            .set_availability_topic(self.topic_prefix + "/status")\
+            .set_device(
+                DiscoveryDevice(
+                    "Home Assistant MQTT Client",
+                    "v0",
+                    ["Home Assistant MQTT Client", "Home Assistant MQTT Client-"+self.UUID],
+                    "Home Assistant MQTT Client")
+                )\
+            .set_unique_id(self.UUID + "-" + output.name)\
+            .set_state_topic(state_topic)\
+            .set_command_topic(command_topic)\
+            .set_payload_on(output.on_payload)\
+            .set_payload_off(output.off_payload)\
+            .build().return_map()
+            self.haDiscoveryPayloads.append(outputDiscoveryPayload)
+            self.setTopicMap[command_topic] = {"state_topic": state_topic, "output": output}
+            self.haDiscoveryTopics.append("homeassistant/" + output.output_type + "/" + self.ha_discovery.node_id + "-" + self.UUID + "/"+output.name+"/config")
+           
+    def getUUID(self) -> str:
+        return self.UUID
+    
+    def getDiscoveryPayloads(self) -> list[map]:
+        return self.haDiscoveryPayloads
+    
+    def getDiscoveryTopics(self) -> list[str]:
+        return self.haDiscoveryTopics
+    
+    def getSetTopicMap(self) -> map[map]:
+        return self.setTopicMap
+
```

### Comparing `rp2040home-0.1.0/RP2040Home.egg-info/SOURCES.txt` & `rp2040home-0.1.4/RP2040Home.egg-info/SOURCES.txt`

 * *Files identical despite different names*

