# Comparing `tmp/nightingalejsonadapter-2.1.0.tar.gz` & `tmp/nightingalejsonadapter-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nightingalejsonadapter-2.1.0.tar", last modified: Thu May  2 15:31:34 2024, max compression
+gzip compressed data, was "nightingalejsonadapter-2.2.0.tar", last modified: Fri May  3 18:34:30 2024, max compression
```

## Comparing `nightingalejsonadapter-2.1.0.tar` & `nightingalejsonadapter-2.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/PKG-INFO
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.709797 nightingalejsonadapter-2.1.0/nightingalejsonadapter/
--rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/__init__.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/intervention_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      560 2023-04-03 16:31:02.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/patient_info_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/trigger_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/uuid_generator.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      622 2023-04-05 17:04:56.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vital_kafka_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_adapter.py
--rw-r--r--   0 nuno      (1000) nuno      (1000)     1180 2023-04-05 17:05:24.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_response.py
-drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/
--rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/PKG-INFO
--rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/SOURCES.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/dependency_links.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/requires.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-02 15:31:34.000000 nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/top_level.txt
--rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-02 15:31:34.713131 nightingalejsonadapter-2.1.0/setup.cfg
--rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-02 14:50:05.000000 nightingalejsonadapter-2.1.0/setup.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-03 18:34:30.090001 nightingalejsonadapter-2.2.0/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-03 18:34:30.090001 nightingalejsonadapter-2.2.0/PKG-INFO
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-03 18:34:30.086667 nightingalejsonadapter-2.2.0/nightingalejsonadapter/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        0 2023-04-04 16:22:01.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/__init__.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      452 2023-04-05 17:04:25.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/intervention_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      700 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/patient_info_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      434 2024-05-02 14:49:08.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/trigger_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      516 2023-03-15 15:22:55.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/uuid_generator.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      607 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/vital_kafka_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      601 2023-04-05 17:04:40.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/vitals_adapter.py
+-rw-r--r--   0 nuno      (1000) nuno      (1000)     1034 2024-05-03 18:33:03.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter/vitals_response.py
+drwxr-xr-x   0 nuno      (1000) nuno      (1000)        0 2024-05-03 18:34:30.090001 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      270 2024-05-03 18:34:30.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/PKG-INFO
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      578 2024-05-03 18:34:30.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/SOURCES.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        1 2024-05-03 18:34:30.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/dependency_links.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)        9 2024-05-03 18:34:30.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/requires.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       23 2024-05-03 18:34:30.000000 nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/top_level.txt
+-rw-r--r--   0 nuno      (1000) nuno      (1000)       38 2024-05-03 18:34:30.090001 nightingalejsonadapter-2.2.0/setup.cfg
+-rw-r--r--   0 nuno      (1000) nuno      (1000)      774 2024-05-03 18:34:25.000000 nightingalejsonadapter-2.2.0/setup.py
```

### Comparing `nightingalejsonadapter-2.1.0/nightingalejsonadapter/patient_info_adapter.py` & `nightingalejsonadapter-2.2.0/nightingalejsonadapter/vital_kafka_adapter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 from __future__ import annotations
 
 from pydantic import BaseModel
 
+from datetime import datetime
+
 
 class DateObserved(BaseModel):
     type: str
-    value: str
+    value: datetime
 
 
 class Payload(BaseModel):
-    name: str
-    surname: str
-    sex: str
-    dob: str
-    age: int
-    nationality: str
-    job: str
-    injury: str
-    transport: int
-    destination: str
-    service: str
-    vector: str
-    color: str
-    identifier: str
-    device: str
-    incident: str
-    latitude: int
-    longitude: int
+    victimid: str
+    incidentid: str
+    devicetype: str
+    respiratory_rate: float
+    systolicbloodpressure: float
+    diastolicbloodpressure: float
+    temperature: float
+    pulserate: float
+    heartratevariability: float
+    pulseoxymetry: float
+    skinmoisture: float
+    encounterdatetime: datetime
 
 
 class Model(BaseModel):
     id: str
     type: str
     dateObserved: DateObserved
     payload: Payload
```

### Comparing `nightingalejsonadapter-2.1.0/nightingalejsonadapter/uuid_generator.py` & `nightingalejsonadapter-2.2.0/nightingalejsonadapter/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_adapter.py` & `nightingalejsonadapter-2.2.0/nightingalejsonadapter/vitals_adapter.py`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.1.0/nightingalejsonadapter/vitals_response.py` & `nightingalejsonadapter-2.2.0/nightingalejsonadapter/vitals_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,40 +18,32 @@
 class VitalEarlyWarningScore(BaseModel):
     HR: int
     RR: int
     SBP: int
     DBP: int
     SPO2: int
 
-
-class ShockIndex(BaseModel):
-    Value: float
-    EarlyWarningScore: int
-
-
 class ProcedureMessage(BaseModel):
-    PredictedInterventionTimestamp: Optional[datetime.datetime] = None
-    Message: Optional[str] = None
-
-
-class ProcedureMessagesABC(BaseModel):
-    a: ProcedureMessage
-    b: ProcedureMessage
-    c: ProcedureMessage
+    procedureName: str
+    predictedInterventionTimestamp: datetime
+    message: str
 
 
 class Prediction(BaseModel):
-    Timestamp: datetime
-    VitalPredictions: VitalPredictions
-    VitalEarlyWarningScore: VitalEarlyWarningScore
-    ShockIndex: ShockIndex
-    ProcedureMessagesABC: ProcedureMessagesABC
+    timestamp: datetime
+    earlyWarningScore: int
+    vitalPredictions: VitalPredictions
+    vitalEarlyWarningScore: VitalEarlyWarningScore
+    shockIndex: float
 
 
 class Model(BaseModel):
     UUID: str
-    LastMeasurementTimestamp: datetime
-    PredictionTimestampId: str
-    PredictionTimeDeltaMinutes: int
-    PatientId: str
-    ProcedureMessageCount: int
-    Predictions: List[Prediction]
+    timestamp: datetime
+    requestId: str
+    lastMeasurementTimestamp: datetime
+    predictionTimestampId: str
+    predictionTimeDeltaMinutes: int
+    victimId: str
+    procedureMessageCount: int
+    procedureMessages: List[ProcedureMessage]
+    predictions: List[Prediction]
```

### Comparing `nightingalejsonadapter-2.1.0/nightingalejsonadapter.egg-info/SOURCES.txt` & `nightingalejsonadapter-2.2.0/nightingalejsonadapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nightingalejsonadapter-2.1.0/setup.py` & `nightingalejsonadapter-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.1.0' 
+VERSION = '2.2.0' 
 DESCRIPTION = 'JSON adapter'
 LONG_DESCRIPTION = 'JSON adapters and validators for Nightingale Communication and Integration'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="nightingalejsonadapter",
```

