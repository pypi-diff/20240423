# Comparing `tmp/python_automationshield-0.4.0.tar.gz` & `tmp/python_automationshield-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_automationshield-0.4.0.tar", max compression
+gzip compressed data, was "python_automationshield-1.0.0.tar", max compression
```

## Comparing `python_automationshield-0.4.0.tar` & `python_automationshield-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,28 @@
--rw-r--r--   0        0        0     1079 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/LICENSE
--rw-r--r--   0        0        0     3193 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/README.md
--rw-r--r--   0        0        0       94 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/arduino_firmware/leonardo/.gitignore
--rw-r--r--   0        0        0      274 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/arduino_firmware/leonardo/.vscode/extensions.json
--rw-r--r--   0        0        0      197 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/arduino_firmware/leonardo/diagram.json
--rw-r--r--   0        0        0     1386 2024-04-05 10:56:23.676691 python_automationshield-0.4.0/arduino_firmware/leonardo/include/README
--rw-r--r--   0        0        0     6308 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/lib/AS5600/AS5600_AS.cpp
--rw-r--r--   0        0        0     4802 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/lib/AS5600/AS5600_AS.h
--rw-r--r--   0        0        0     1037 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/lib/README
--rw-r--r--   0        0        0    30282 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/lib/VL53L0X/VL53L0X.cpp
--rw-r--r--   0        0        0     6326 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/lib/VL53L0X/VL53L0X.h
--rw-r--r--   0        0        0      437 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/platformio.ini
--rw-r--r--   0        0        0     1289 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/src_aeroshield/main.cpp
--rw-r--r--   0        0        0     2049 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/src_floatshield/main.cpp
--rw-r--r--   0        0        0     1874 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/src_magnetoshield/main.cpp
--rw-r--r--   0        0        0      518 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/test/README
--rw-r--r--   0        0        0      132 2024-04-05 10:56:23.677691 python_automationshield-0.4.0/arduino_firmware/leonardo/wokwi.toml
--rw-r--r--   0        0        0      785 2024-04-05 10:56:23.678691 python_automationshield-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      262 2024-04-05 10:56:23.678691 python_automationshield-0.4.0/src/automationshield/__init__.py
--rw-r--r--   0        0        0     6408 2024-04-05 10:56:23.678691 python_automationshield-0.4.0/src/automationshield/controller.py
--rw-r--r--   0        0        0       52 2024-04-05 10:56:23.678691 python_automationshield-0.4.0/src/automationshield/exception.py
--rw-r--r--   0        0        0       67 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/plotting/__init__.py
--rw-r--r--   0        0        0     2692 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/plotting/live_plotter.py
--rw-r--r--   0        0        0     1620 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/plotting/plotter.py
--rw-r--r--   0        0        0      236 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/aeroshield.py
--rw-r--r--   0        0        0     7453 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/baseshield.py
--rw-r--r--   0        0        0      509 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/dummyshield.py
--rw-r--r--   0        0        0      582 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/floatshield.py
--rw-r--r--   0        0        0      700 2024-04-05 10:56:23.679691 python_automationshield-0.4.0/src/automationshield/shields/magnetoshield.py
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 python_automationshield-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-04-23 09:48:31.740728 python_automationshield-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4590 2024-04-23 09:48:31.740728 python_automationshield-1.0.0/README.md
+-rw-r--r--   0        0        0      752 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      776 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/src/automationshield/__init__.py
+-rw-r--r--   0        0        0     4473 2024-04-23 09:48:31.741729 python_automationshield-1.0.0/src/automationshield/arduino.py
+-rw-r--r--   0        0        0      113 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/aeroshield/aeroshield.ino
+-rw-r--r--   0        0        0      115 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/floatshield/floatshield.ino
+-rw-r--r--   0        0        0      418 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.cpp
+-rw-r--r--   0        0        0      447 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/aeroshield/aeroshield.h
+-rw-r--r--   0        0        0     2481 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.cpp
+-rw-r--r--   0        0        0      986 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/automationshield/automationshield.h
+-rw-r--r--   0        0        0      356 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.cpp
+-rw-r--r--   0        0        0      367 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/floatshield/floatshield.h
+-rw-r--r--   0        0        0      122 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.cpp
+-rw-r--r--   0        0        0      269 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/lib/magnetoshield/magnetoshield.h
+-rw-r--r--   0        0        0      119 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/arduino_firmware/magnetoshield/magnetoshield.ino
+-rw-r--r--   0        0        0     7525 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/controller.py
+-rw-r--r--   0        0        0       52 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/exception.py
+-rw-r--r--   0        0        0       67 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/live_plotter.py
+-rw-r--r--   0        0        0     1615 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/plotting/plotter.py
+-rw-r--r--   0        0        0      186 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/shields/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-23 09:48:31.742729 python_automationshield-1.0.0/src/automationshield/shields/aeroshield.py
+-rw-r--r--   0        0        0    11855 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/baseshield.py
+-rw-r--r--   0        0        0      468 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/dummyshield.py
+-rw-r--r--   0        0        0     1060 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/floatshield.py
+-rw-r--r--   0        0        0     6933 2024-04-23 09:48:31.743729 python_automationshield-1.0.0/src/automationshield/shields/magnetoshield.py
+-rw-r--r--   0        0        0     5404 1970-01-01 00:00:00.000000 python_automationshield-1.0.0/PKG-INFO
```

### Comparing `python_automationshield-0.4.0/LICENSE` & `python_automationshield-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_automationshield-0.4.0/README.md` & `python_automationshield-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 # python-automationshield
 
-`python-automationshield` is a Python package that implements a Python interface to [Automationshield](https://github.com/gergelytakacs/AutomationShield)'s devices. Automationshield creates cheap and accessible tools for control engineering education in the form of Arduino shields. Currently, this package has Python implementations for the following shields:
+`python-automationshield` is a Python package that implements a Python interface to [Automationshield](https://github.com/gergelytakacs/AutomationShield)'s devices. Automationshield creates cheap and accessible tools for control engineering education in the form of Arduino shields. Much of the Arduino code used in this package is derived from the code in the [Automationshield](https://github.com/gergelytakacs/AutomationShield) repository.
+
+Currently, this package has Python implementations for the following shields:
 
 - [Aeroshield](https://github.com/gergelytakacs/AutomationShield/wiki/AeroShield)
 - [Floatshield](https://github.com/gergelytakacs/AutomationShield/wiki/FloatShield)
 - [Magnetoshield](https://github.com/gergelytakacs/AutomationShield/wiki/MagnetoShield)
 
-This project was built to allow TU Delft students learning control engineering to use Python in their assignments, since that is what they are thought in the curriculum. This package provides a flexible controller class that lets users conveniently implement a controller and run it on the Arduino hardware.
+This project was built to allow TU Delft students learning control engineering to use Python in their assignments, since that is what they are thought in the curriculum. This package provides a flexible controller class that lets users conveniently implement a controller and test it on the hardware without having to reupload new firmware to the Arduino board.
+
+This project was developed using [Arduino Leonardo](https://docs.arduino.cc/hardware/leonardo/) boards. The code may work on other devices as well, but it will likely need a few changes. You are welcome to submit a pull request to add functionality for additional Arduino boards!
 
 ## Installation
 
 `python-automationshield` requires Python >= 3.10 and can be installed with the following command:
 
 ```bash
 $ pip install python-automationshield
 ```
 
 ## Usage
 
 <!-- - TODO: basic basic example, live plot visuals. link to examples -->
 Below is a very simple example with the AeroShield to get started. Read more in the [documentation](https://python-automationshield.readthedocs.io).
 
-Use the `AeroShield` class to interface directly with the Arduino.
+### Install the firmware on an Arduino board
+
+When first importing the module, `AutomationShield` will download the [`arduino-cli`](https://arduino.github.io/arduino-cli/) to the package directory. The `arduino-cli` is used to flash the correct firmware onto your Arduino board. The package _should_ download the correct executable for your operating system and architecture, but it has only been tested on a 64-bit Windows system.
+
+```python
+from automationshield import AeroShield
+from automationshield.arduino import UNO  # import the FQBN for the UNO from the arduino module
+
+aero_shield = AeroShield()
+aero_shield.install_firmware(device=UNO)
+
+#optionally check that the correct firmware is installed
+with aero_shield:
+    print(aero_shield.check_firmware)  # this will print the version number of the Arduino code if the firmware is correct and throw an exception otherwise.
+```
+
+### Send commands to the `AeroShield` and read its state
 
 ```python
 from automationshield import AeroShield
 
 
 with AeroShield() as aero_shield:
     for _ in range(100):
         aero_shield.write(flag=aero_shield.RUN, motor=50)
         out = aero_shield.read()
         print(f"Potentiomneter [%]: {out[0]}, Angle [°]: {out[1]}")
 ```
 
-Use the `ShieldController` class to conveniently implement a controller.
+### Use the `ShieldController` class to conveniently implement a controller
 
 ```python
 from automationshield import AeroShield, ShieldController
 
 
 class MyController(ShieldController):
     def controller(self, t: float, dt: float, ref: float, pot: float, angle: float) -> float:
@@ -47,25 +67,25 @@
 
 # create controller instance
 my_controller = MyController(AeroShield())
 # run the controller on the Arduino.
 hist = my_controller.run(freq=200, cycles=1000, ref=45)
 ```
 
-Plot the experiment data using the `plotting.Plotter` class
+### Plot the experiment data using the `plotting.Plotter` class
 
 ```python
 from automationshield.plotting import Plotter
 
 
 fig, ax = Plotter.plot(hist)
 fig.show()
 ```
 
-Below is an example of a figure plotting the result of a PID controller with a constant reference at 45°.
+Below is an example of a figure plotting the result of a PID controller on the AeroShield with a constant reference at 45°.
 
 ![Plot of PID controller output](https://gitlab.com/mrtreasurer/python-automationshield/-/raw/main/docs/images/pid_controller_output.png)
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
```

### Comparing `python_automationshield-0.4.0/pyproject.toml` & `python_automationshield-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "python-automationshield"
-version = "0.4.0"
+version = "1.0.0"
 description = "A Python interface to AutomationShield's Arduino shields"
 authors = ["Bert Van den Abbeele"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/mrtreasurer/python-automationshield"
 documentation = "https://python-automationshield.readthedocs.io"
 packages = [
     { include = "automationshield", from = "src"}
 ]
-include = ["arduino_firmware/*"]
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 matplotlib = ">=3.8.2"
 numpy = ">=1.26.3"
 pyserial = ">=3.5"
```

### Comparing `python_automationshield-0.4.0/src/automationshield/controller.py` & `python_automationshield-1.0.0/src/automationshield/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,37 @@
 from typing import Optional, Iterable
 
 from .shields.baseshield import BaseShield
 from .plotting import LivePlotter
 
 
 class ShieldController:
+    """The ShieldController class implements a controller interface for the various shield classes. This class should be subclassed to create custom controllers.\
+        In a subclass, overwrite the :py:meth:`ShieldController.controller` method to implement your controller. Optionally, overwrite the :py:meth:`ShieldController.variables` method \
+        to initialise instance variables that should persist beyond the scope of the controller method.
+
+    Example:
+
+    >>> class MyController(ShieldController):
+    ...     def controller(self, t: float, dt: float, ref: float, pot: float, sensor: float) -> float:
+    ...         return ref
+
+    :param shield: shield class instance.
+    :type shield: ~automationshield.shields.BaseShield
+    :param n_base_vars: Number of variables that is saved by default. These are the time, reference, potentiometer, sensor and actuator values.
+    :type n_base_vars: int
+    :param tracked_variables: Mapping of additional variables to track during run.
+    :type tracked_variables: dict[str, int]
+    """
     def __init__(self, shield:BaseShield) -> None:
         self.shield = shield
 
         self.n_base_vars = 5
         # store additional variables to save when running an experiment
-        self.extra_hist_vars: dict[str, int] = dict()
+        self.tracked_variables: dict[str, int] = dict()
 
         # initiate controller variables
         self.variables()
 
     def variables(self) -> None:
         """Define variables to be used by the controller or saved during the experiment."""
         pass
@@ -30,17 +47,17 @@
         :param name: Name of the variable, without 'self.'
         :type name: str
         :param size: Size of the variable, e.g. 3 for a three-dimensional position vector. Defaults to 1, i.e. single values.
         :type size: int, optional
         :return: A copy of the current map of tracked variables and their respective size.
         :rtype: dict[str, int]
         """
-        self.extra_hist_vars[name] = size
+        self.tracked_variables[name] = size
 
-        return self.extra_hist_vars.copy()
+        return self.tracked_variables.copy()
 
     def controller(self, t: float, dt: float, ref: float, pot: float, sensor: float) -> float:
         """Implement the controller here. You can subclass ShieldController and overwrite the controller.
 
         :param t: Time since start of run in seconds.
         :type t: float
         :param dt: Length of current time step in seconds.
@@ -62,26 +79,26 @@
 
         :param freq: Desired frequency of the loop.
         :type freq: int
         :param cycles: Number of cycles to run the experiment.
         :type cycles: int
         :param ref: The reference to follow. It should have a lenght equal to freq * time or be a single value for a constant reference. Defaults to None, in which case the reference is set to 0.
         :type ref: Optional[float  |  int  |  Iterable[float | int]], optional
-        :param live_plotter: Optional LivePlotter instance to use for displaying a live plot, defaults to None
-        :type live_plotter: Optional[LivePlotter], optional
+        :param live_plotter: Optional :py:class:`~automationshield.plotting.LivePlotter` instance to use for displaying a live plot, defaults to None.
+        :type live_plotter: ~automationshield.plotting.LivePlotter, optional
         :return: Experiment data. The columns of the array are time, reference, potentiometer, sensor, actuator, and any additional variables in the order they were added.
-        :rtype: npt.NDArray[np.float_]
+        :rtype: npt.NDArray[np.float\_]
         """
 
         cntr = 0
         maxcntr = cycles
         period = 1/freq
 
         # calculate number of additional columns needed
-        extra_hist_size = sum(self.extra_hist_vars.values())
+        extra_hist_size = sum(self.tracked_variables.values())
         # t1 - tstart, ref, pot, sensor, actuator, any additional variables
         hist = np.zeros((maxcntr, self.n_base_vars + extra_hist_size))
 
         # create a zero array if no ref is given
         if ref is None:
             ref = np.zeros(maxcntr)
 
@@ -137,26 +154,26 @@
 
         return hist
 
     def _update_hist(self, hist: npt.NDArray[np.float_], cntr: int, t: float, ref: float, pot:float, sensor: float, actuator: float):
         """Update hist array with variables of the current iteration (cntr). If variables were added to `extra_hist_vars`, add them to the hist as well.
 
         :param hist: array to update.
-        :type hist: npt.NDArray[np.float_]
+        :type hist: npt.NDArray[np.float\_]
         :param cntr: Iteration counter. Provides the first index to hist.
         :type cntr: int
         :param t: Time.
         :type t: float
         :param ref: Current reference value.
         :type ref: float
         :param sensor: Current pendulum angle
         :type sensor: float
         :param actuator: Current Motor value.
         :type actuator: float
         """
         hist[cntr, 0:self.n_base_vars] = t, ref, pot, sensor, actuator
         total_vars = self.n_base_vars
 
-        for name, size in self.extra_hist_vars.items():
+        for name, size in self.tracked_variables.items():
             hist[cntr, total_vars:total_vars+size] = getattr(self, name)
 
             total_vars += size
```

### Comparing `python_automationshield-0.4.0/src/automationshield/plotting/live_plotter.py` & `python_automationshield-1.0.0/src/automationshield/plotting/live_plotter.py`

 * *Files identical despite different names*

### Comparing `python_automationshield-0.4.0/src/automationshield/plotting/plotter.py` & `python_automationshield-1.0.0/src/automationshield/plotting/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     def plot(self, hist):
         self.ref_line.set_data(hist[:, 0], hist[:, 1])
         self.angle_line.set_data(hist[:, 0], hist[:, 3])
         self.ax[0].relim()
         self.ax[0].autoscale_view()
 
-        self.motor_line.set_data(hist[:, 0], hist[:, 4]/2.55)
+        self.motor_line.set_data(hist[:, 0], hist[:, 4])
         self.pot_line.set_data(hist[:, 0], hist[:, 2])
         self.ax[1].relim()
         self.ax[1].autoscale_view()
 
         self.dt_line.set_data(hist[:, 0], 1000*np.gradient(hist[:, 0]))
         self.ax[2].relim()
         self.ax[2].autoscale_view()
```

### Comparing `python_automationshield-0.4.0/src/automationshield/shields/baseshield.py` & `python_automationshield-1.0.0/src/automationshield/shields/baseshield.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,121 @@
 import serial
 import serial.tools.list_ports
 import time
 
-from random import randint
 from typing import Optional
 
+from .. import arduino
 from ..exception import AutomationShieldException
 
 
 class BaseShield:
+    """Base class for shield devices. Handles communication with Arduino, sensor calibration and unit conversions. The class can also install the proper firmware on an Arduino.
+
+    Interface:
+        * Actuator input should be provided in percent by default.
+        * Potentiometer is provided in percent by default.
+        * Sensor values are converted to relevant physical units in the child classes.
+
+    :param TEST: Flag to write to Arduino. This flag is used to check if the correct firmware is installed. The response from the Arduino should be the C++ software version and the id of the shield.
+    :type TEST: int
+    :param RUN: Falg to write to Arduino. This flag is used for normal running of the shield device. The actuator value is applied and the Arduino responds with the potentiometer and sensor values.
+    :type RUN: int
+    :param STOP: Flag to write to Arduino. This flag is used to stop the actuator. The Arduino will stop the actuator to ensure the shield is safely stopped.
+    :type STOP: int
+    :param TIMEOUT: Time to wait after opening the serial connection before writing to the Arduino.
+    :type TIMEOUT: int
+    :param script: name of the script directory in which the ``.ino`` file for the specific shield is located.
+    :type script: str
+    :param shield_id: ID assigned to shield. This is used to check whether the correct firmware is installed on the Arduino.
+    :type shield_id: str
+    :param actuator_bits: Number of bits used for actuator.
+    :type actuator_bits: int
+    :param potentiometer_bits: Number of bits used for potentiometer.
+    :type potentiometer_bits: int
+    :param sensor_bits: Number of bits used for sensor.
+    :type sensor_bits: int
+    :param port: Port of the Arduino.
+    :type port: str
+    :param conn: Serial connection to the Arduino.
+    :type conn: serial.Serial
+    :param zero_reference: Zero reference of the sensor for calibration.
+    :type zero_reference: float
+    """
     TEST = 0
     RUN = 1
     STOP = 2
 
     # Wait time after opening connection
     TIMEOUT = 3
 
-    def __init__(self, baudrate:Optional[int]=115200, port:Optional[str]=None) -> None:
+    script = ""
+    shield_id = ""
+
+    actuator_bits = 8
+    potentiometer_bits = 10  # resolution of system ad converter
+    sensor_bits = 12
+
+    def __init__(self, port:Optional[str]=None) -> None:
+        """Constructor method. Create a serial connection object (without opening the connection). Will try to find the Arduino device is no port is provided.
+
+        :param port: Port on which the Arduino is connected, defaults to None.
+        :type port: str
+        """
         if port is None:
             port = self.find_arduino()
+        self.port = port
 
-        self.conn = serial.Serial(port, baudrate=baudrate)
+        self.conn = serial.Serial(baudrate=115200)
+        self.conn.port = self.port
         self.conn.timeout = 1
 
-        self.actuator_bits = 8
-        self.potentiometer_bits = 10  # resolution of system ad converter
-        self.sensor_bits = 12
-
         self.zero_reference = 0
 
     def find_arduino(self) -> str:
         """Get the name of the port that is connected to Arduino. Raises exception if no port was found.
 
-        :raises AutomationShieldException: Raised if no Arduino was found.
+        :raises automationshield.AutomationShieldException: Raised if no Arduino was found.
         :return: COM port of the Arduino.
         :rtype: str
         """
         ports = serial.tools.list_ports.comports()
         for p in ports:
             if p.manufacturer is not None and "Arduino" in p.manufacturer:
                 return p.device
 
         raise AutomationShieldException("No Arduino Found")
 
-    def firmware_installed(self) -> bool:
-        """Check that the correct firmware is installed on the Arduino. This is done by sending flag `BaseShield.TEST` to the Arduino, \
-            followed by a random integer. If the Arduino responds with the double and quadruple of the random integer, \
-            the firmware is assumed to be correct.
-
-        :return: True if the firmware is assumed correct, False otherwise.
-        :rtype: bool.
-        """
-        with self as shield:
-            # set the upper limit of the range to the lower of the potentiometer bits divided by 2 and the sensor bits divided by 4, to guarantee the response fits in the bits.
-            v = randint(0, min(2**(self.potentiometer_bits-1), 2**(self.sensor_bits-2)) - 1)
-            shield.write(self.TEST, v)
-            r1, r2 = shield.read()
-
-        return (r1 == 2*v) and (r2 == 4*v)
-
-    def check_firmware(self):
-        if not self.firmware_installed():
-            # run install thing here
-            raise AutomationShieldException("Wrong firmware installed on the Arduino")
+    def check_firmware(self) -> int:
+        """Check that the correct firmware is installed on the Arduino. When the arduino reads the :py:attr:`BaseShield.TEST` flag, it should respond with the code version and two bytes which, when converted to ASCII, should match the shield id.
+
+        :raises automationshield.AutomationShieldException: If the arduino didn't respond correctly.
+        :return: version number of Arduino firmware.
+        :rtype: int
+        """
+
+        # set the upper limit of the range to the lower of the potentiometer bits divided by 2 and the sensor bits divided by 4, to guarantee the response fits in the bits.
+        self.write(self.TEST, 0)
+        bts = self.conn.read(size=3)
+        id = f"{chr(bts[1])}{chr(bts[2])}"
+
+        if id == self.shield_id:
+            return bts[0]
+
+        else:
+            raise AutomationShieldException("Incorrect firmware installed on Arduino")
+
+    def install_firmware(self, device:str) -> None:
+        """Compile firmware for the current shield and upload to the Arduino.
 
+        :param device: FQBN of Arduino. FQBNs for common devices are provided in :py:mod:`automationshield.arduino`, e.g. :py:const:`automationshield.arduino.LEONARDO`: ``arduino:avr:leonardo``.
+        :type device: str
+        """
+        arduino.compile_script(device, self.script)
+        arduino.upload_script(device, self.script, self.port)
 
     def convert_potentiometer_reading(self, raw: int) -> float:
         """Convert n-bit potentiometer reading to percentage value.
 
         :param raw: n-bit potentiometer value.
         :type raw: int
         :return: Potentiometer value as percentage [0, 100].
@@ -93,30 +141,33 @@
         :type sensor: int
         :return: Sensor value converted to physical units
         :rtype: int
         """
         return sensor
 
     def calibrate_sensor_reading(self, sensor: int) -> int:
-        """Calibrate the sensor reading with the zero reference. Should be implemented on subclass.
+        """Calibrate the sensor reading with the zero reference. Should be implemented on subclass. The default implementation is
+
+        .. math::
+            sensor_{calibrated} = sensor_{raw} - ref
 
         :param sensor: Raw sensor value.
         :type sensor: int
         :return: Calibrated sensor value.
         :rtype: int
         """
         return sensor - self.zero_reference
 
     def read(self, raw: bool=False) -> tuple[float]:
-        """Read data from Arduino. If `raw == False`, the potentiometer value is rescaled to percentages; and the sensor is calibrated with the zero reference and converted to relevant units. This is the default. \
-            If `raw == True`, none of that happens and the potentiometer and sensor are returned as n-bit values. No calibration is performed either.
+        """Read data from Arduino. If ``raw == False``, the potentiometer value is rescaled to percentages; and the sensor is calibrated with the zero reference and converted to relevant units. This is the default. \
+            If ``raw == True``, none of that happens and the potentiometer and sensor are returned as n-bit values. No calibration is performed either.
 
         :param raw: If True, returns raw n-bit readings from potentiometer and sensor. Defaults to False, in which case the potentiometer is converted to percent and the sensor to approppriate units.
         :type raw: bool
-        :raises AutomationShieldException: Raised if no data was received. This can happen if there was no `write` command preceding a call to `read`.
+        :raises automationshield.AutomationShieldException: Raised if no data was received. This can happen if there was no :py:meth:`BaseShield.write` command invoked preceding a call to :py:meth:`BaseShield.read`.
         :return: Converted and calibrated potentiometer and sensor readings, in that order.
         :rtype: tuple[float]
         """
         try:
             data = self.conn.read(size=3)
 
             pot = data[0] // 16 * 256 + data[1]
@@ -128,76 +179,113 @@
             else:
                 return self.convert_potentiometer_reading(pot), self.convert_sensor_reading(self.calibrate_sensor_reading(sensor))
 
         except IndexError:
             raise AutomationShieldException("No data received from Arduino")
 
     @staticmethod
-    def saturate(value: float, bits: int) -> int:
-        """Saturate value between `0` and `2**bits - 1`.
+    def saturate_bits(value: float, bits: int) -> int:
+        """Saturate value between :math:`0` and :math:`2^{bits - 1}` inclusive.
 
         :param value: Raw value.
         :type value: float
         :param bits: Number of bits.
         :type bits: int
         :return: Saturated value.
         :rtype: int
         """
-        return int(min(max((value), 0), 2**bits - 1))
+        return int(min(max(value, 0), 2**bits - 1))
+
+    @staticmethod
+    def saturate_percent(value: float) -> float:
+        """Saturate value between :math:`0` and :math:`100` inclusive.
+
+        :param value: Raw value in percent.
+        :type value: float
+        :return: Saturated value in percent.
+        :rtype: float
+        """
+        return min(max(value, 0), 100)
 
     def write(self, flag: int, actuator: float, raw: bool=False) -> int:
         """Write run/stop flag and actuator value to Arduino. Convert and saturate the actuator value before sending.
 
-        :param flag: `BaseShield.RUN` or `BaseShield.STOP`. The former signals normal running mode, the latter tells the Arduino to stop the motor.
+        the flag must be one of :py:attr:`BaseShield.TEST`, :py:attr:`BaseShield.RUN` or :py:attr:`BaseShield.STOP`.
+
+        * :py:attr:`BaseShield.TEST` returns the version number of the Arduino code and a shield id, which should match :py:attr:`BaseShield.shield_id`. The actuator input is irrelevant for this command.
+        * :py:attr:`BaseShield.RUN` means normal running mode. Set the actuator value.
+        * :py:attr:`BaseShield.STOP` tells the arduino to stop the actuator. The supplied actuator value is ignored by the Arduino.
+
+        :param flag: :py:attr:`BaseShield.TEST`, :py:attr:`BaseShield.RUN` or :py:attr:`BaseShield.STOP`.
         :type flag: int
         :param actuator: actuator value.
         :type actuator: float
-        :param raw: If False, expects actuator as percentage [0, 100]. Value is converted before being sent. If True, expects actuator in range of [0, 2^actuator_bits). Defaults to False.
+        :param raw: If False, expects actuator as percentage [0, 100]. Value is converted before being sent. If True, expects actuator in range of [0, 2^actuator_bits - 1]. Defaults to False.
         :type raw: bool, optional
         :return: Saturated n-bit motor value.
         :rtype: int
         """
 
         if not raw:
-            actuator = self.convert_actuator_input(actuator)
+            saturated_actuator = self.saturate_percent(actuator)
+            actuator = self.convert_actuator_input(saturated_actuator)
+            output = self.saturate_bits(actuator, self.actuator_bits)
 
-        actuator = self.saturate(actuator, self.actuator_bits)
+        else:
+            saturated_actuator = self.saturate_bits(actuator, self.actuator_bits)
+            output = saturated_actuator
 
         if self.actuator_bits > 8:
-            bts = [flag, actuator//256, actuator%256]
+            bts = [flag, output//256, output%256]
         else:
-            bts = [flag, actuator]
+            bts = [flag, output]
 
         self.conn.write(bytes(bts))
-        return actuator
+
+        return saturated_actuator
 
     def calibrate(self):
-        """Read out a zero reference. System should be at rest when calling this method."""
+        """Read out a zero reference. System should be at rest when calling this method. The zero reference is assigned to :py:attr:`BaseShield.zero_reference`."""
         self.write(self.RUN, 0)
         _, self.zero_reference = self.read(raw=True)
 
     def stop(self):
-        """Send stop signal to Arduino."""
+        """Send :py:attr:`BaseShield.STOP` signal to Arduino."""
         self.write(self.STOP, 0)
 
     def open(self):
-        """Reset buffers and open connection to Arduino if it is not open already. Wait for `AeroShield.TIMEOUT` seconds to make sure connection is established."""
+        """Reset buffers and open connection to Arduino if it is not open already. Wait for :py:attr:`BaseShield.TIMEOUT` seconds to make sure connection is established."""
         if not self.conn.is_open:
             self.conn.open()
 
         self.conn.reset_input_buffer()
         self.conn.reset_output_buffer()
 
         time.sleep(self.TIMEOUT)
 
     def close(self, *args):
         """Close connection to Arduino."""
         self.conn.close()
 
     def __enter__(self):
+        """Implements the ``with`` context manager. This method calls
+
+        * :py:meth:`BaseShield.open`,
+        * :py:meth:`BaseShield.check_firmware`,
+        * :py:meth:`BaseShield.calibrate`.
+
+        :return: Shield instance.
+        :rtype: BaseShield
+        """
         self.open()
+        self.check_firmware()
         self.calibrate()
         return self
 
     def __exit__(self, *args):
+        """Closes the context manager. This method calls
+
+        * :py:meth:`BaseShield.stop`,
+        * :py:meth:`BaseShield.close`.
+        """
         self.stop()
         self.close(*args)
```

### Comparing `python_automationshield-0.4.0/src/automationshield/shields/magnetoshield.py` & `python_automationshield-1.0.0/src/automationshield/shields/floatshield.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from .baseshield import BaseShield
 
 
-class MagnetoShield(BaseShield):
-    def __init__(self, baudrate: int | None = 115200, port: str | None = None) -> None:
-        super().__init__(baudrate, port)
-
-        self.actuator_bits = 12
-        self.sensor_bits = 10
-
-    def convert_sensor_reading(self, sensor: int) -> float:
-        """Converts the n-bit sensor reading of the Hall effect sensor to Gauss. \
-            The constants in this method are for release 4 of the MagnetoShield.
+class FloatShield(BaseShield):
+    """Class for Floatshield device. Inherits from BaseShield.
+
+    The Floatshield features a ball in a vertical tube. A fan (the actuator) is installed at the bottom, which can blow the ball up in the tube. \
+        The position of the ball in the tube is measured by a distance sensor at the top of the tube, using infrared laser.
+
+    Interface:
+        * Actuator input should be provided in percent by default.
+        * Potentiometer is provided in percent by default.
+        * Sensor values are provided in millimeters from the bottom of the tube.
+    """
+    script = "floatshield"
+    shield_id = "FL"
+
+    actuator_bits = 12
+
+    def calibrate_sensor_reading(self, sensor: int) -> int:
+        """Calibrate sensor reading. 0 is taken as the ball being at the bottome of the tube.
 
         :param sensor: Raw sensor value.
         :type sensor: int
-        :return: Sensor value in Gauss.
+        :return: Calibrate sensor value.
         :rtype: int
         """
-        return (2.5 - sensor*(3.3/(2**self.potentiometer_bits - 1)))*800
+        return - super().calibrate_sensor_reading(sensor)
```

### Comparing `python_automationshield-0.4.0/PKG-INFO` & `python_automationshield-1.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-automationshield
-Version: 0.4.0
+Version: 1.0.0
 Summary: A Python interface to AutomationShield's Arduino shields
 Home-page: https://gitlab.com/mrtreasurer/python-automationshield
 License: MIT
 Author: Bert Van den Abbeele
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,49 +16,69 @@
 Requires-Dist: pyserial (>=3.5)
 Project-URL: Documentation, https://python-automationshield.readthedocs.io
 Project-URL: Repository, https://gitlab.com/mrtreasurer/python-automationshield
 Description-Content-Type: text/markdown
 
 # python-automationshield
 
-`python-automationshield` is a Python package that implements a Python interface to [Automationshield](https://github.com/gergelytakacs/AutomationShield)'s devices. Automationshield creates cheap and accessible tools for control engineering education in the form of Arduino shields. Currently, this package has Python implementations for the following shields:
+`python-automationshield` is a Python package that implements a Python interface to [Automationshield](https://github.com/gergelytakacs/AutomationShield)'s devices. Automationshield creates cheap and accessible tools for control engineering education in the form of Arduino shields. Much of the Arduino code used in this package is derived from the code in the [Automationshield](https://github.com/gergelytakacs/AutomationShield) repository.
+
+Currently, this package has Python implementations for the following shields:
 
 - [Aeroshield](https://github.com/gergelytakacs/AutomationShield/wiki/AeroShield)
 - [Floatshield](https://github.com/gergelytakacs/AutomationShield/wiki/FloatShield)
 - [Magnetoshield](https://github.com/gergelytakacs/AutomationShield/wiki/MagnetoShield)
 
-This project was built to allow TU Delft students learning control engineering to use Python in their assignments, since that is what they are thought in the curriculum. This package provides a flexible controller class that lets users conveniently implement a controller and run it on the Arduino hardware.
+This project was built to allow TU Delft students learning control engineering to use Python in their assignments, since that is what they are thought in the curriculum. This package provides a flexible controller class that lets users conveniently implement a controller and test it on the hardware without having to reupload new firmware to the Arduino board.
+
+This project was developed using [Arduino Leonardo](https://docs.arduino.cc/hardware/leonardo/) boards. The code may work on other devices as well, but it will likely need a few changes. You are welcome to submit a pull request to add functionality for additional Arduino boards!
 
 ## Installation
 
 `python-automationshield` requires Python >= 3.10 and can be installed with the following command:
 
 ```bash
 $ pip install python-automationshield
 ```
 
 ## Usage
 
 <!-- - TODO: basic basic example, live plot visuals. link to examples -->
 Below is a very simple example with the AeroShield to get started. Read more in the [documentation](https://python-automationshield.readthedocs.io).
 
-Use the `AeroShield` class to interface directly with the Arduino.
+### Install the firmware on an Arduino board
+
+When first importing the module, `AutomationShield` will download the [`arduino-cli`](https://arduino.github.io/arduino-cli/) to the package directory. The `arduino-cli` is used to flash the correct firmware onto your Arduino board. The package _should_ download the correct executable for your operating system and architecture, but it has only been tested on a 64-bit Windows system.
+
+```python
+from automationshield import AeroShield
+from automationshield.arduino import UNO  # import the FQBN for the UNO from the arduino module
+
+aero_shield = AeroShield()
+aero_shield.install_firmware(device=UNO)
+
+#optionally check that the correct firmware is installed
+with aero_shield:
+    print(aero_shield.check_firmware)  # this will print the version number of the Arduino code if the firmware is correct and throw an exception otherwise.
+```
+
+### Send commands to the `AeroShield` and read its state
 
 ```python
 from automationshield import AeroShield
 
 
 with AeroShield() as aero_shield:
     for _ in range(100):
         aero_shield.write(flag=aero_shield.RUN, motor=50)
         out = aero_shield.read()
         print(f"Potentiomneter [%]: {out[0]}, Angle [°]: {out[1]}")
 ```
 
-Use the `ShieldController` class to conveniently implement a controller.
+### Use the `ShieldController` class to conveniently implement a controller
 
 ```python
 from automationshield import AeroShield, ShieldController
 
 
 class MyController(ShieldController):
     def controller(self, t: float, dt: float, ref: float, pot: float, angle: float) -> float:
@@ -67,25 +87,25 @@
 
 # create controller instance
 my_controller = MyController(AeroShield())
 # run the controller on the Arduino.
 hist = my_controller.run(freq=200, cycles=1000, ref=45)
 ```
 
-Plot the experiment data using the `plotting.Plotter` class
+### Plot the experiment data using the `plotting.Plotter` class
 
 ```python
 from automationshield.plotting import Plotter
 
 
 fig, ax = Plotter.plot(hist)
 fig.show()
 ```
 
-Below is an example of a figure plotting the result of a PID controller with a constant reference at 45°.
+Below is an example of a figure plotting the result of a PID controller on the AeroShield with a constant reference at 45°.
 
 ![Plot of PID controller output](https://gitlab.com/mrtreasurer/python-automationshield/-/raw/main/docs/images/pid_controller_output.png)
 
 ## Contributing
 
 Interested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.
```

