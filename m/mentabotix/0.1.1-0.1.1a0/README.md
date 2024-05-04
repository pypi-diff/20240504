# Comparing `tmp/mentabotix-0.1.1.tar.gz` & `tmp/mentabotix-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.1.tar", last modified: Sat May  4 01:48:48 2024, max compression
+gzip compressed data, was "mentabotix-0.1.1a0.tar", last modified: Wed May  1 16:22:14 2024, max compression
```

## Comparing `mentabotix-0.1.1.tar` & `mentabotix-0.1.1a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    19747 2024-05-04 01:48:24.381681 mentabotix-0.1.1/README.md
--rw-r--r--   0        0        0      630 2024-05-04 01:48:48.749712 mentabotix-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      847 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    56590 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    19645 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     3363 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/tools/algrithm_tools.py
--rw-r--r--   0        0        0      229 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     5457 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/vision/camra.py
--rw-r--r--   0        0        0     8336 2024-05-04 01:48:24.381681 mentabotix-0.1.1/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-04 01:48:24.381681 mentabotix-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0    12243 2024-05-04 01:48:24.381681 mentabotix-0.1.1/tests/test_botix.py
--rw-r--r--   0        0        0     8042 2024-05-04 01:48:24.381681 mentabotix-0.1.1/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-04 01:48:24.381681 mentabotix-0.1.1/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-04 01:48:24.381681 mentabotix-0.1.1/tests/test_moving_transition.py
--rw-r--r--   0        0        0    20179 1970-01-01 00:00:00.000000 mentabotix-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    14350 2024-05-01 16:21:51.481188 mentabotix-0.1.1a0/README.md
+-rw-r--r--   0        0        0      701 2024-05-01 16:22:14.453434 mentabotix-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      847 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    56590 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    19645 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     3363 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/algrithm_tools.py
+-rw-r--r--   0        0        0      229 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     5457 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/camra.py
+-rw-r--r--   0        0        0     8336 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/__init__.py
+-rw-r--r--   0        0        0    12243 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_botix.py
+-rw-r--r--   0        0        0     8042 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-01 16:21:51.485188 mentabotix-0.1.1a0/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    14877 1970-01-01 00:00:00.000000 mentabotix-0.1.1a0/PKG-INFO
```

### Comparing `mentabotix-0.1.1/README.md` & `mentabotix-0.1.1a0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,51 +4,30 @@
 ---
 
 ## Installation
 
 Use `pdm` to install mentabotix
 
 ```shell
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable release
 pdm add mentabotix
-
-# for unstable release
-pdm add mentabotix --pre
-
 ```
 
 ## Usage
 
 ### Menta
 
 You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
 
 #### Step 1: Define Sampler Functions
 
 Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
 could include sequence samplers that return a series of data points, index samplers that provide data at a specific
 index, and direct response samplers that give an immediate value.
 
-|               Sampler                |                 Description                  |                    Type                    |
-|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
-| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
-| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
-| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
-
-> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
-> their respective types in the `Menta` class.
-
 ```python
-
 def temperature_sequence_sampler() -> list[float]:
     """Simulates a sequence of temperature readings."""
     return [25.5, 26.0, 25.8]
 
 
 def humidity_index_sampler(index: int) -> float:
     """Returns simulated humidity data at a given index."""
@@ -64,160 +43,80 @@
 #### Step 2: Initialize Menta Instance and Add Samplers
 
 After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
 
 ```python
 from mentabotix import Menta  # Ensure to import the correct Menta class
 
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
+menta_instance = Menta(samplers=[temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
 ```
 
 #### Step 3: Update Sampler Types
 
 Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
 
 ```python
-from mentabotix import Menta  # Ensure to import the correct Menta class
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
 menta_instance.update_sampler_types()
 ```
 
-#### Step 4: Construct Judge Function
+#### Step 4: Construct Updater Function
 
 To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
 which system updates might occur. For example:
 
 ```python
-from mentabotix import SamplerUsage, Menta
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+from mentabotix import SamplerUsage
 
-menta_instance.update_sampler_types()
+# Assuming we want to trigger an update when the temperature is above 25 and humidity is below 50%
+judging_source = "temp > 25 and humidity < 50"
 
 # Define how samplers will be used
 usages = [
-
-    # Use sequence sampler for first and third temp data
     SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-    # Use index sampler for the first humidity value
-    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
+    # Use sequence sampler for first and third temp data
+    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),  # Use index sampler for the first humidity value
+    # For direct response samplers, typically, no required_data_indexes are needed since they return a single value
 ]
 
-# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
-# s0 stands for the data at index 0 of the first sampler
-# s1 stands for the data at index 2 of the first sampler
-# s3 stands for the data at index 1 of the second sampler
-
-judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
-
-# Extra context for the judge function, here only contains the "baseline"
-extra_context = {"baseline": 47}
-
-from typing import Callable
-
-# Construct the judge function object
-updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
-                                                                               extra_context=extra_context)
-
-# Use the judge function to update the system
-updater_function()
-
+updater_function = menta_instance.construct_updater(usages)
 
-# Below is the equivalent implementation of the judge function, but is defined manually. 
-# It acts exactly the same as the `updater_function` above.
-def manual_judge_function() -> bool:
-    """Manually construct the judge function."""
-    seq_temp = temperature_sequence_sampler()
-    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
+# Execute the updater function
+result = updater_function()
+print(result)
 ```
 
-In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
-performance since the all the calls and variables are inlined and stored in the closure.
----
+In this scenario, `construct_updater` dynamically creates and executes a function based on the specified sampler usages
+and a logical condition (`judging_source`). This function then returns a result or triggers actions according to the
+given criteria (e.g., temperature and humidity conditions).
+
+Make sure to tailor the sampler functions, the logic expression string, and the usage of samplers to fit your specific
+application needs.
 
 ## Botix
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
-schemas into executable closures using the Botix framework.
+schemas into executable closures using the Botix framework. Keep in mind that while this explanation avoids deep Python
+specifics, a basic understanding of programming concepts will be helpful.
 
 ### Understanding State-Transition Control Schema
 
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
   motor speeds or changing direction.
-- A state describe the robot's **moving behavior**, 4 motor speeds in this case
 
 #### Transitions
 
 - Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
   one state to another, possibly based on sensor inputs or internal conditions.
-- Transitions describe how the robot **moves** from one state to another
 
 ### Building Your Control Schema
 
 #### Step 1: Define States
 
 For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
 that state. For instance, creating a state for moving forward might look like this:
@@ -258,18 +157,17 @@
 #### Step 2: Define Transitions
 
 Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
 occur (using a breaker function), and the source and destination states.
 
 ```python
 from mentabotix import MovingTransition, MovingState
-from random import random
 
-sensor_reading = lambda: random()  # Example sensor reading function
-threshold = 0.6
+sensor_reading = lambda: 25.5  # Example sensor reading function
+threshold = 25.0
 
 
 def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
     return sensor_reading() < threshold
 
 
 moving_forward = MovingState(10)
@@ -317,67 +215,14 @@
 ```
 
 #### Step 3: Connect States with Transitions
 
 Create a collection of your states and transitions, ensuring each transition correctly references its source and target
 states.
 
-A legal control schema should have a start state and at least one end state.
-And each state can **ONLY** connect to **ONE** transition as its input state
-
-```python
-from mentabotix import MovingState, MovingTransition
-import random
-
-moving_left = MovingState.turn("l", 10)
-moving_right = MovingState.turn("r", 10)
-moving_dash = MovingState.straight(100)
-stopped_state = MovingState(0)
-
-start_state = MovingState(100)
-
-
-def _breaker_1() -> int:
-    return random.choice([0, 1, 2])
-
-
-def _breaker_2() -> int:
-    return random.choice([0, 1])
-
-
-transition_1 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_1,  # When to break the transition
-    from_states=stopped_state,
-    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
-)
-
-transition_2 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_2,  # When to break the transition
-    from_states=stopped_state,
-    to_states={0: moving_dash, 1: stopped_state},
-)
-
-
-```
-
-As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
-the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
-stage.
-
-Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
-
-```python
-from mentabotix import Botix
-
-# A StructuralError will be raised if the structure is not valid
-Botix.ensure_structure_validity([transition_1, transition_2])
-```
-
 ### Compiling to Closures with Botix
 
 Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
 as closures, which can directly control the robot's behavior.
 
 #### Step 4: Compile the Schema
 
@@ -420,15 +265,15 @@
 [
     "def _func():",
     "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
 ]
 
 ```
 
-But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
+But usaully, you want to compile the code into a closure that can be used to control the robot with higher performance
 and less human error.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 from typing import Callable
 
@@ -437,15 +282,15 @@
                                                             MotorInfo(code_sign=2, direction=-1),
                                                             MotorInfo(code_sign=4, direction=-1)], port="COM3")
 
 start_state = MovingState(-1)
 state_a = MovingState(0)
 state_b = MovingState(1)
 state_c = MovingState(2)
-# create some transitions
+# 创建一些假的MovingTransition对象用于测试
 transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
 transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
@@ -455,26 +300,29 @@
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
-```
-< function _func at 0x0000020D40EAECA0 >
+```python
+< function
+_func
+at
+0x0000020D40EAECA0 >
 ```
 
 Usage is as follows
 
 ```python
 # call the closure, which will execute the compiled code
 function_closure()
 ```
 
-Of course, you can also build a closure with branching logic in it.
+Of course, you can also build a closure with branch logic in it.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 import random
 from typing import List, Tuple, Dict, Any, Callable
 
@@ -540,28 +388,13 @@
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
 ```
 
-## Logging
-
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
-
-```python
-from mentabotix import set_log_level
-
-"""
-Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
-Logging INFO - Information message, used to inform the general program running status, with a value of 20.
-Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
-Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
-Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
-"""
-
-set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
-
-from logging import CRITICAL
+### Conclusion
 
-set_log_level(CRITICAL)  # this has the same effect as above
-```
+By following these steps, you can design a control schema for your robot using state transitions and compile it into
+executable code using Botix. Remember, practice and experimentation are key – start with simple schemas and gradually
+increase complexity as you become more comfortable with the process. Always test your schemas in a safe environment
+before deploying on actual hardware.
```

### Comparing `mentabotix-0.1.1/src/mentabotix/__init__.py` & `mentabotix-0.1.1a0/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/modules/botix.py` & `mentabotix-0.1.1a0/src/mentabotix/modules/botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/modules/logger.py` & `mentabotix-0.1.1a0/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/modules/menta.py` & `mentabotix-0.1.1a0/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/tools/algrithm_tools.py` & `mentabotix-0.1.1a0/src/mentabotix/tools/algrithm_tools.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/vision/camra.py` & `mentabotix-0.1.1a0/src/mentabotix/vision/camra.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.1a0/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/tests/test_botix.py` & `mentabotix-0.1.1a0/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/tests/test_menta.py` & `mentabotix-0.1.1a0/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/tests/test_moving_state.py` & `mentabotix-0.1.1a0/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/tests/test_moving_transition.py` & `mentabotix-0.1.1a0/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.1/PKG-INFO` & `mentabotix-0.1.1a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,51 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
+Requires-Dist: pydantic>=2.7.0
 Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: bdmc>=0.1.3
+Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: numpy>=1.26.4
+Requires-Dist: pyuptech>=0.1.4a0
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Requires-Dist: pyapriltags>=3.3.0.3
 Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.4
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
 
 ## Installation
 
 Use `pdm` to install mentabotix
 
 ```shell
-# install pdm
-python -m pip install pdm
-
-# config pdm
-pdm config pypi.url https://pypi.tuna.tsinghua.edu.cn/simple
-
-# for stable release
 pdm add mentabotix
-
-# for unstable release
-pdm add mentabotix --pre
-
 ```
 
 ## Usage
 
 ### Menta
 
 You can use `Menta` to create the judge function closure of the robot, using the sensor data as the input.
 
 #### Step 1: Define Sampler Functions
 
 Firstly, you need to define sampler functions that adhere to the specifications outlined by the `Menta` class. These
 could include sequence samplers that return a series of data points, index samplers that provide data at a specific
 index, and direct response samplers that give an immediate value.
 
-|               Sampler                |                 Description                  |                    Type                    |
-|:------------------------------------:|:--------------------------------------------:|:------------------------------------------:|
-| `mentabotix.SamplerType.SEQ_SAMPLER` | The sensor data is returned in a `Sequence`. | `Callable[[], Sequence[Union[float,int]]]` |
-| `mentabotix.SamplerType.IDX_SAMPLER` |         Use a index to get the data.         |    `Callable[[int], Union[float,int]]`     |
-| `mentabotix.SamplerType.DRC_SAMPLER` |  Direct read sensor data without any args.   |      `Callable[[], Union[float,int]]`      |
-
-> Do remember to add return type annotations to your sampler functions, which will be used to classify the samplers into
-> their respective types in the `Menta` class.
-
 ```python
-
 def temperature_sequence_sampler() -> list[float]:
     """Simulates a sequence of temperature readings."""
     return [25.5, 26.0, 25.8]
 
 
 def humidity_index_sampler(index: int) -> float:
     """Returns simulated humidity data at a given index."""
@@ -79,160 +61,80 @@
 #### Step 2: Initialize Menta Instance and Add Samplers
 
 After defining the sampler functions, initialize the `Menta` instance and add these samplers to it.
 
 ```python
 from mentabotix import Menta  # Ensure to import the correct Menta class
 
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
+menta_instance = Menta(samplers=[temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
 ```
 
 #### Step 3: Update Sampler Types
 
 Invoke the `update_sampler_types` method to automatically classify the samplers into their respective types.
 
 ```python
-from mentabotix import Menta  # Ensure to import the correct Menta class
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
-
 menta_instance.update_sampler_types()
 ```
 
-#### Step 4: Construct Judge Function
+#### Step 4: Construct Updater Function
 
 To use the samplers in a meaningful way, you can construct an updater function that encapsulates a condition based on
 which system updates might occur. For example:
 
 ```python
-from mentabotix import SamplerUsage, Menta
-
-
-def temperature_sequence_sampler() -> list[float]:
-    """Simulates a sequence of temperature readings."""
-    return [25.5, 26.0, 25.8]
-
-
-def humidity_index_sampler(index: int) -> float:
-    """Returns simulated humidity data at a given index."""
-    humidity_values = [45.0, 50.0, 55.0]
-    return humidity_values[index]
-
-
-def light_direct_sampler() -> float:
-    """Provides the current light intensity reading."""
-    return 750.0
-
-
-menta_instance = Menta()
-menta_instance.samplers.extend([temperature_sequence_sampler, humidity_index_sampler, light_direct_sampler])
+from mentabotix import SamplerUsage
 
-menta_instance.update_sampler_types()
+# Assuming we want to trigger an update when the temperature is above 25 and humidity is below 50%
+judging_source = "temp > 25 and humidity < 50"
 
 # Define how samplers will be used
 usages = [
-
-    # Use sequence sampler for first and third temp data
     SamplerUsage(used_sampler_index=0, required_data_indexes=[0, 2]),
-    # Use index sampler for the first humidity value
-    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),
+    # Use sequence sampler for first and third temp data
+    SamplerUsage(used_sampler_index=1, required_data_indexes=[0]),  # Use index sampler for the first humidity value
+    # For direct response samplers, typically, no required_data_indexes are needed since they return a single value
 ]
 
-# Note: the judge source has some built-in syntaxes.Currently, sensor data indexes flattening and extra data context insertion
-# s0 stands for the data at index 0 of the first sampler
-# s1 stands for the data at index 2 of the first sampler
-# s3 stands for the data at index 1 of the second sampler
-
-judging_source = "(s0 > 25 and s1 < 50) or s3>baseline"
-
-# Extra context for the judge function, here only contains the "baseline"
-extra_context = {"baseline": 47}
-
-from typing import Callable
-
-# Construct the judge function object
-updater_function: Callable[[], bool] = menta_instance.construct_judge_function(usages, judging_source=judging_source,
-                                                                               extra_context=extra_context)
-
-# Use the judge function to update the system
-updater_function()
-
+updater_function = menta_instance.construct_updater(usages)
 
-# Below is the equivalent implementation of the judge function, but is defined manually. 
-# It acts exactly the same as the `updater_function` above.
-def manual_judge_function() -> bool:
-    """Manually construct the judge function."""
-    seq_temp = temperature_sequence_sampler()
-    return (seq_temp[0] > 25 and seq_temp[2] < 50) or humidity_index_sampler(0) > 47
+# Execute the updater function
+result = updater_function()
+print(result)
 ```
 
-In this case, a judge function closure is created using `exec()` method.Normally the built should have a better
-performance since the all the calls and variables are inlined and stored in the closure.
----
+In this scenario, `construct_updater` dynamically creates and executes a function based on the specified sampler usages
+and a logical condition (`judging_source`). This function then returns a result or triggers actions according to the
+given criteria (e.g., temperature and humidity conditions).
+
+Make sure to tailor the sampler functions, the logic expression string, and the usage of samplers to fit your specific
+application needs.
 
 ## Botix
 
 Welcome to the guide on using Botix for state-transition control schema creation and compilation. This document will
 walk you through the steps to design a control schema using state and transition concepts, and then how to compile those
-schemas into executable closures using the Botix framework.
+schemas into executable closures using the Botix framework. Keep in mind that while this explanation avoids deep Python
+specifics, a basic understanding of programming concepts will be helpful.
 
 ### Understanding State-Transition Control Schema
 
 Imagine you're designing an autonomous robot that needs to navigate different environments. Each behavior or action the
 robot can take is represented by a **state**, such as "moving forward," "turning left," or "halt." Transitions between
 these states are triggered by events or conditions, forming a **control schema**.
 
 #### States
 
 - In Botix, a state is represented by the `MovingState` class. Each state might have associated actions like setting
   motor speeds or changing direction.
-- A state describe the robot's **moving behavior**, 4 motor speeds in this case
 
 #### Transitions
 
 - Transitions between states are handled by the `MovingTransition` class. They define how and when the robot moves from
   one state to another, possibly based on sensor inputs or internal conditions.
-- Transitions describe how the robot **moves** from one state to another
 
 ### Building Your Control Schema
 
 #### Step 1: Define States
 
 For each distinct behavior, create a `MovingState` instance. Include the actions or configurations that should occur in
 that state. For instance, creating a state for moving forward might look like this:
@@ -273,18 +175,17 @@
 #### Step 2: Define Transitions
 
 Transitions are created with `MovingTransition`. Specify the duration, any conditions under which the transition should
 occur (using a breaker function), and the source and destination states.
 
 ```python
 from mentabotix import MovingTransition, MovingState
-from random import random
 
-sensor_reading = lambda: random()  # Example sensor reading function
-threshold = 0.6
+sensor_reading = lambda: 25.5  # Example sensor reading function
+threshold = 25.0
 
 
 def stop_condition() -> bool:  # the return type must be annotated, since an exception will be raised otherwise
     return sensor_reading() < threshold
 
 
 moving_forward = MovingState(10)
@@ -332,67 +233,14 @@
 ```
 
 #### Step 3: Connect States with Transitions
 
 Create a collection of your states and transitions, ensuring each transition correctly references its source and target
 states.
 
-A legal control schema should have a start state and at least one end state.
-And each state can **ONLY** connect to **ONE** transition as its input state
-
-```python
-from mentabotix import MovingState, MovingTransition
-import random
-
-moving_left = MovingState.turn("l", 10)
-moving_right = MovingState.turn("r", 10)
-moving_dash = MovingState.straight(100)
-stopped_state = MovingState(0)
-
-start_state = MovingState(100)
-
-
-def _breaker_1() -> int:
-    return random.choice([0, 1, 2])
-
-
-def _breaker_2() -> int:
-    return random.choice([0, 1])
-
-
-transition_1 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_1,  # When to break the transition
-    from_states=stopped_state,
-    to_states={1: moving_left, 2: moving_right, 0: moving_dash},
-)
-
-transition_2 = MovingTransition(
-    duration=2,  # Duration to transition
-    breaker=_breaker_2,  # When to break the transition
-    from_states=stopped_state,
-    to_states={0: moving_dash, 1: stopped_state},
-)
-
-
-```
-
-As the above example, `transition_1` and `transition_2` both have the `stopped_state` as the input state,which means
-the `stopped_state` connects more than **ONE** transition. Definition as such is illegal and will not pass the compile
-stage.
-
-Normally, you can ensure that the structure is valid by using `ensure_structure_validity`. to eliminate this problem.
-
-```python
-from mentabotix import Botix
-
-# A StructuralError will be raised if the structure is not valid
-Botix.ensure_structure_validity([transition_1, transition_2])
-```
-
 ### Compiling to Closures with Botix
 
 Once your control schema is defined, Botix can help you compile this structure into executable code, often referred to
 as closures, which can directly control the robot's behavior.
 
 #### Step 4: Compile the Schema
 
@@ -435,15 +283,15 @@
 [
     "def _func():",
     "    con.set_motors_speed((-1, -1, -1, -1)).delay(0.1).set_motors_speed((0, 0, 0, 0)).delay(1).set_motors_speed((1, 1, 1, 1)).delay(2).set_motors_speed((2, 2, 2, 2))",
 ]
 
 ```
 
-But usually, you want to compile the code into a closure that can be used to control the robot with higher performance
+But usaully, you want to compile the code into a closure that can be used to control the robot with higher performance
 and less human error.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 from typing import Callable
 
@@ -452,15 +300,15 @@
                                                             MotorInfo(code_sign=2, direction=-1),
                                                             MotorInfo(code_sign=4, direction=-1)], port="COM3")
 
 start_state = MovingState(-1)
 state_a = MovingState(0)
 state_b = MovingState(1)
 state_c = MovingState(2)
-# create some transitions
+# 创建一些假的MovingTransition对象用于测试
 transition_start_a = MovingTransition(duration=0.1, from_states=start_state, to_states=state_a)
 transition_ab = MovingTransition(duration=1, from_states=state_a, to_states=state_b)
 transition_bc = MovingTransition(duration=2, from_states=state_b, to_states=state_c)
 
 botix = Botix(controller=con)
 botix.token_pool.append(transition_start_a)
 botix.token_pool.append(transition_ab)
@@ -470,26 +318,29 @@
 function_closure: Callable[[], None] = botix.compile(return_median=False)
 
 print(function_closure)
 ```
 
 By printing out the `function_closure` object, you can see the compiled code as a closure that can be called
 
-```
-< function _func at 0x0000020D40EAECA0 >
+```python
+< function
+_func
+at
+0x0000020D40EAECA0 >
 ```
 
 Usage is as follows
 
 ```python
 # call the closure, which will execute the compiled code
 function_closure()
 ```
 
-Of course, you can also build a closure with branching logic in it.
+Of course, you can also build a closure with branch logic in it.
 
 ```python
 from mentabotix import MovingState, MovingTransition, Botix
 from bdmc import CloseLoopController, MotorInfo
 import random
 from typing import List, Tuple, Dict, Any, Callable
 
@@ -555,28 +406,13 @@
 
 # call the closure, which will execute the compiled code
 compiled_closure()
 
 
 ```
 
-## Logging
-
-use `set_log_level` to silent the console to improve the performance in high pressure conditions
-
-```python
-from mentabotix import set_log_level
-
-"""
-Logging DEBUG - Debugging information, used for detailed development phase logs, typically with a value of 10.
-Logging INFO - Information message, used to inform the general program running status, with a value of 20.
-Logging WARN - A warning message indicating that there may be a problem but the program is still running, with a value of 30.
-Logging Error - Error message indicating an issue preventing the program from executing properly, with a value of 40.
-Logging CRITICAL - Fatal error message indicating a serious system failure with a value of 50.
-"""
-
-set_log_level(50)  # set the log-level to 50, which makes logger only print the msg important than the CRITICAL logging
-
-from logging import CRITICAL
+### Conclusion
 
-set_log_level(CRITICAL)  # this has the same effect as above
-```
+By following these steps, you can design a control schema for your robot using state transitions and compile it into
+executable code using Botix. Remember, practice and experimentation are key – start with simple schemas and gradually
+increase complexity as you become more comfortable with the process. Always test your schemas in a safe environment
+before deploying on actual hardware.
```

