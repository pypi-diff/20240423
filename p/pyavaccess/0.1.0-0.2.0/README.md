# Comparing `tmp/pyavaccess-0.1.0.tar.gz` & `tmp/pyavaccess-0.2.0.tar.gz`

## Comparing `pyavaccess-0.1.0.tar` & `pyavaccess-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/requirements.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/pyavaccess/__init__.py
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/pyavaccess/avaccess_serial.py
--rw-r--r--   0        0        0    16701 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/pyavaccess/hdmi_matrix.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/pyavaccess/config/matrix_devices.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/tests/test_4KMX42.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/LICENSE
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/README.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 pyavaccess-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/pyavaccess/__init__.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/pyavaccess/avaccess_serial.py
+-rw-r--r--   0        0        0    17229 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/pyavaccess/hdmi_matrix.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/pyavaccess/config/matrix_devices.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/tests/test_4KMX42.py
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/README.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 pyavaccess-0.2.0/PKG-INFO
```

### Comparing `pyavaccess-0.1.0/pyavaccess/avaccess_serial.py` & `pyavaccess-0.2.0/pyavaccess/avaccess_serial.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,19 @@
         self, cmdStr: str, useDeviceEOL: bool = False, lineCount: int = 1
     ) -> str:
         """
         Send a command to the device and receive its response
         @param cmdStr: Data to send
         @return: Response from the device
         """
+        _LOGGER.debug("Checking cmdStr content before sending to device")
+        # Make sure string exists
+        if not cmdStr:
+            raise ValueError("Cannot send empty line to device!")
+
         _LOGGER.debug("Clearing buffers...")
         self._port.reset_output_buffer()
         self._port.reset_input_buffer()
 
         # Process the cmd for sending
         _LOGGER.debug('Encoding "%s"...', cmdStr)
         cmdStr = cmdStr + "\r\n"
@@ -46,18 +51,21 @@
 
         _LOGGER.debug("Receiving...")
         result = bytearray()
         linesRead = 0
         while True:
             char = self._port.read(1)
 
+            # Check for end of incoming serial
             if char is None:
                 break
 
+            # If we received back nothing, but not null (ex: "")
             if not char:
+                # Usually only reached by invalid command
                 raise serial.SerialTimeoutException(
                     "Connection timed out! Last received bytes {}".format(
                         [hex(c) for c in result]
                     )
                 )
 
             result += char
```

### Comparing `pyavaccess-0.1.0/pyavaccess/hdmi_matrix.py` & `pyavaccess-0.2.0/pyavaccess/hdmi_matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,121 +9,125 @@
 
 
 class HDMIMatrixSerial(AVAccessSerial):
     """
     General class for AV Access HDMI Matrix devices
     """
 
-    def __init__(
-        self,
-        url: str,
-        device: str,
-    ) -> None:
+    def __init__(self, url: str, device: str) -> None:
         """
         Initialize the AVAccess device for connecting over serial
         """
-        # Get the device config from the yaml file
-        deviceConfig = self._getDeviceConfig(device)
-
         _LOGGER.debug("Creating HDMI Matrix %s...")
         super().__init__(url)
+
+        # Begin device setup
         self.model = device
+        self.apiVersion = self.getVer()
+
+        # Get the device config from the yaml file
+        deviceConfig = self._getDeviceConfig(device, self.apiVersion)
         self.inputs = deviceConfig["inputCount"]
         self.outputs = deviceConfig["outputCount"]
         self.audioOutputs = deviceConfig["audioOutputs"]
         self.prmEDIDCount = deviceConfig["EDIDParamCount"]
         self.maxDelay = deviceConfig["maxDelayInMin"]
         self.irModeCount = deviceConfig["irModeCount"]
         self.commandCount = deviceConfig["commandCount"]
 
-    def _getDeviceConfig(self, device: str) -> dict:
+
+    def _getDeviceConfig(self, device: str, apiVersion: str) -> dict:
         """
         @param device: Device name
+        @param apiVersion APi version string in format "VER #.#.#"
         @return: Configuration for the device
         """
-        _LOGGER.debug("Matching %s to config...", device)
+        _LOGGER.debug("Finding config for %s version %s...", device, apiVersion)
+        # Don't send anything to the device if we don't know what version we're using
+        if apiVersion not in MatrixDevices:
+            raise ValueError("Device version %s does not exist in the config!", apiVersion)
 
         # User device input case insensitive
         absDevice = device.upper()
 
         # If the device is not in the config, raise an error
-        if absDevice not in MatrixDevices:
+        if absDevice not in MatrixDevices[apiVersion]:
             raise ValueError("Device %s does not exist in the config!", device)
 
         # Only return the config for the device
-        return MatrixDevices[absDevice]
+        return MatrixDevices[apiVersion][absDevice]
 
     """ Function Helper Methods """
 
     def isOutNumInBounds(self, outNum: int) -> bool:
         """
         Check if the output number is in bounds
         @param outNum: output number
         @return: True if in bounds, False if not
         """
+        _LOGGER.debug("Checking if output number %s is in bounds...", outNum)
         if outNum < 1 or outNum > self.outputs:
-            _LOGGER.error("Output number %s is out of bounds!", outNum)
-            return False
+            raise ValueError("Output number %s is out of bounds!", outNum)
         return True
 
     def isInputNumInBounds(self, inNum: int) -> bool:
         """
         Check if the input number is in bounds
         @param inNum: input number
         @return: True if in bounds, False if not
         """
+        _LOGGER.debug("Checking if input number %s is in bounds...", inNum)
         if inNum < 1 or inNum > self.inputs:
-            _LOGGER.error("Input number %s is out of bounds!", inNum)
-            return False
+            raise ValueError("Input number %s is out of bounds!", inNum)
         return True
 
     def isAudioOutStringOnDevice(self, outString: str) -> bool:
         """
         Check if the audio output string exists on the device
         @param outString: string of the audio output device
         @return: True if on device, False if not
         """
+        _LOGGER.debug("Checking if audio out string %s exists on device...", outString)
         if outString not in self.audioOutputs:
-            _LOGGER.error(
+            raise ValueError(
                 "Audio output string %s does not exist on the device!", outString
             )
-            return False
         return True
 
     def isEDIDPrmNumInBounds(self, prmNum: int) -> bool:
         """
         Check if the EDID param number is in bounds
         @param prmNum: EDID param number
         @return: True if in bounds, False if not
         """
+        _LOGGER.debug("Checking if EDID param number %s is in bounds...", prmNum)
         if prmNum < 1 or prmNum > self.prmEDIDCount:
-            _LOGGER.error("EDID param number %s is out of bounds!", prmNum)
-            return False
+            raise ValueError("EDID param number %s is out of bounds!", prmNum)
         return True
 
     def isDelayInBounds(self, delay: int) -> bool:
         """
         Check if the delay is in bounds
         @param delay: delay in minutes
         @return: True if in bounds, False if not
         """
+        _LOGGER.debug("Checking if delay %s is in bounds...", delay)
         if delay < 1 or delay > self.maxDelay:
-            _LOGGER.error("Delay %s is out of bounds!", delay)
-            return False
+            raise ValueError("Delay %s is out of bounds!", delay)
         return True
 
     def isIRInBounds(self, mode: int) -> bool:
         """
         Check if the IR mode is in bounds
         @param mode: IR mode
         @return: True if in bounds, False if not
         """
+        _LOGGER.debug("Checking if IR mode %s is in bounds...", mode)
         if mode < 1 or mode > self.irModeCount:
-            _LOGGER.error("IR mode %s is out of bounds!", mode)
-            return False
+            raise ValueError("IR mode %s is out of bounds!", mode)
         return True
 
     """ Output Formatting Methods """
 
     def mapWithPattern(self, mapping: str, pattern: Pattern[str]) -> dict:
         """
         Create a dictionary for all values
@@ -210,27 +214,29 @@
         _LOGGER.debug("Getting available commands...")
         deviceOutput = self._SendData(cmdStr, lineCount=self.commandCount)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     """ Status Methods """
 
-    def getMapping(self, outNum: int) -> dict:
+    def getMapping(self, outNum: int) -> int:
         """
         @param outNum: output number
-        @return: Dict w/ input number mapped to the output {out: in}
+        @return: The input number mapped to the specified output
         """
-        if not self.isOutNumInBounds(outNum):
-            return
+        self.isOutNumInBounds(outNum)
 
         cmdStr = "GET MP out{}".format(outNum)
         _LOGGER.debug("Getting mapping for output %s...", outNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
-        return self.mapWithPattern(deviceOutput, PATTERN_OUT)
+        # Get dict w/ input number mapped to the output {out: in}
+        outputMap = self.mapWithPattern(deviceOutput, PATTERN_OUT)
+        # Only return the input number
+        return outputMap[outNum]
 
     def getMappings(self) -> dict:
         """
         @return: Dictionary of current input mapping to all outputs {out: in, out: in, ...}
         """
         cmdStr = "GET MP all"
         _LOGGER.debug("Getting mappings for all outputs...")
@@ -239,44 +245,41 @@
         return self.mapWithPattern(deviceOutput, PATTERN_OUT)
 
     def getAutoCECStatus(self, outNum: int) -> str:
         """
         @param outNum: output number
         @return: Current "CEC AUTO POWER ON/OFF Status" of the output
         """
-        if not self.isOutNumInBounds(outNum):
-            return
+        self.isOutNumInBounds(outNum)
 
         cmdStr = "GET AUTOCEC_FN out{}".format(outNum)
         _LOGGER.debug("Getting Auto CEC status for output %s...", outNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     def getCECDelay(self, outNum: int) -> str:
         """
         @param outNum: output number
         @return: Current "CEC POWER Delay Time Status" of the output
         """
-        if not self.isOutNumInBounds(outNum):
-            return
+        self.isOutNumInBounds(outNum)
 
         cmdStr = "GET AUTOCEC_D out{}".format(outNum)
         _LOGGER.debug("Getting CEC Delay for output %s...", outNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     def getInputEDIDStatus(self, inNum: int) -> str:
         """
         @param inNum: input number
         @return: Current EDID Status of the input
         """
-        if not self.isInputNumInBounds(inNum):
-            return
+        self.isInputNumInBounds(inNum)
 
         cmdStr = "GET EDID in{}".format(inNum)
         _LOGGER.debug("Getting EDID status for output %s...", inNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
@@ -292,16 +295,15 @@
         return deviceOutput
 
     def getMuteStatus(self, outString: str) -> str:
         """
         @param outString: string of the audio output device
         @return: Mute status of the output
         """
-        if not self.isAudioOutStringOnDevice(outString):
-            return
+        self.isAudioOutStringOnDevice(outString)
 
         cmdStr = "GET MUTE {}".format(outString)
         _LOGGER.debug("Getting mute status for %s...", outString)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
@@ -323,47 +325,45 @@
     def mapOutput(self, outNum: int, inNum: int) -> dict:
         """
         Map an input to an output
         @param outNum: output number
         @param inNum: input number
         @return: Dict of current input mapped to the output {out: in}
         """
-        if not self.isOutNumInBounds(outNum) or not self.isInputNumInBounds(inNum):
-            return
+        self.isOutNumInBounds(outNum)
+        self.isInputNumInBounds(inNum)
 
         cmdStr = "SET SW in{} out{}".format(inNum, outNum)
         _LOGGER.debug("Mapping input %s to output %s...", inNum, outNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return self.mapWithPattern(deviceOutput, PATTERN_OUT)
 
     def mapAllOutputs(self, inNum: int) -> dict:
         """
         Map an inputs to all outputs
         @param inNum: input number
         @return: Current mapping to all outputs
         """
-        if not self.isInputNumInBounds(inNum):
-            return
+        self.isInputNumInBounds(inNum)
 
         cmdStr = "SET SW in{} all".format(inNum)
         _LOGGER.debug("Mapping input %s to all outputs...", inNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return self.mapWithPattern(deviceOutput, PATTERN_ALL)
 
     def setCECPower(self, outNum: int, state: bool) -> str:
         """
         Set the CEC power state of the output
         @param outNum: output number
         @param state: True = On, False = Off
         @return: Current power state of the output
         """
-        if not self.isOutNumInBounds(outNum):
-            return
+        self.isOutNumInBounds(outNum)
 
         # Get the text to use for the command based on state
         stateText = "on" if state else "off"
 
         cmdStr = "SET CEC_PWR out{} {}".format(outNum, stateText)
         _LOGGER.debug(
             "Setting CEC power state for output %s to %s...", outNum, stateText
@@ -375,16 +375,15 @@
     def setAutoCEC(self, outNum: int, state: bool) -> str:
         """
         Set the CEC auto power state of the output
         @param outNum: output number
         @param state: True = On, False = Off
         @return: Current auto power state of the output
         """
-        if not self.isOutNumInBounds(outNum):
-            return
+        self.isOutNumInBounds(outNum)
 
         # Get the text to use for the command based on state
         stateText = "on" if state else "off"
 
         cmdStr = "SET AUTOCEC_FN out{} {}".format(outNum, stateText)
         _LOGGER.debug(
             "Setting CEC auto power state for output %s to %s...", outNum, stateText
@@ -396,63 +395,61 @@
     def setCECDelay(self, outNum: int, delay: int) -> str:
         """
         Set the CEC power delay time for the output
         @param outNum: output number
         @param delay: Delay in minutes
         @return: Current delay time of the output in minutes
         """
-        if not self.isOutNumInBounds(outNum) or not self.isDelayInBounds(delay):
-            return
+        self.isOutNumInBounds(outNum)
+        self.isDelayInBounds(delay)
 
         cmdStr = "SET AUTOCEC_D out{} {}".format(outNum, delay)
         _LOGGER.debug("Setting CEC delay for output %s to %s...", outNum, delay)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     def setInputEDIDStatus(self, inNum: int, prmNum: int) -> str:
         """
         Set the EDID of the input
         @param inNum: input number
         @param prmNum: EDID param number (see API)
         @return: Current EDID status of the input
         """
-        if not self.isInputNumInBounds(inNum) or not self.isEDIDPrmNumInBounds(prmNum):
-            return
+        self.isInputNumInBounds(inNum)
+        self.isEDIDPrmNumInBounds(prmNum)
 
         cmdStr = "SET EDID in{} {}".format(inNum, prmNum)
         _LOGGER.debug("Setting EDID for input %s to %s...", inNum, prmNum)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     def setIR_SC(self, mode: int) -> str:
         """
         Set the IR system code
         @param mode: IR system code (see API)
         @return: Current IR system code
         """
-        if not self.isIRInBounds(mode):
-            return
+        self.isIRInBounds(mode)
 
         cmdStr = "SET IR_SC mode{}".format(mode)
         _LOGGER.debug("Setting IR system code to mode %s...", mode)
         deviceOutput = self._SendData(cmdStr)
         _LOGGER.debug("Device output: %s", deviceOutput)
         return deviceOutput
 
     def setMuteStatus(self, outString: str, state: bool) -> str:
         """
         Set the mute status of the output
         @param outString: string of the audio output device
         @param state: True = On, False = Off
         @return: Current mute status of the output
         """
-        if not self.isAudioOutStringOnDevice(outString):
-            return
+        self.isAudioOutStringOnDevice(outString)
 
         # Get the text to use for the command based on state
         stateText = "on" if state else "off"
 
         cmdStr = "SET MUTE {} {}".format(outString, stateText)
         _LOGGER.debug("Setting mute status for %s to %s...", outString, stateText)
         deviceOutput = self._SendData(cmdStr)
```

### Comparing `pyavaccess-0.1.0/pyavaccess/config/matrix_devices.py` & `pyavaccess-0.2.0/pyavaccess/config/matrix_devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 # Define regular expressions for common response patterns
 PATTERN_ALL = re.compile(r".* in(\d+) all")
 PATTERN_OUT = re.compile(r".* in(\d+) out(\d+)")
 
 # Define configuration for matrix devices
 MatrixDevices = {
-    "4KMX42-H2A": {
-        "inputCount": 4,
-        "outputCount": 2,
-        "audioOutputs": [
-            "hdmiaudioout1",
-            "hdmiaudioout2",
-            "audioout1",
-            "spdifaudioout2",
-        ],
-        "EDIDParamCount": 11,
-        "maxDelayInMin": 30,
-        "irModeCount": 2,
-        "commandCount": 24,
+    # Pick device config by version
+    "VER 1.0.2": {
+        "4KMX42-H2A": {
+            "inputCount": 4,
+            "outputCount": 2,
+            "audioOutputs": [
+                "hdmiaudioout1",
+                "hdmiaudioout2",
+                "audioout1",
+                "spdifaudioout2",
+            ],
+            "EDIDParamCount": 11,
+            "maxDelayInMin": 30,
+            "irModeCount": 2,
+            "commandCount": 24,
+        }
     }
 }
```

### Comparing `pyavaccess-0.1.0/.gitignore` & `pyavaccess-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyavaccess-0.1.0/LICENSE` & `pyavaccess-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyavaccess-0.1.0/README.md` & `pyavaccess-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,9 +32,17 @@
 for output, input in outputMap.items():
     print("Output {} is mapped to input {}".format(output, input))
 
 # Set the input for output 1 to input 4
 av.mapOutput(1, 4)
 
 # Check that the mapping was successful
-assert av.getMapping(1)[1] == 4
+assert av.getMapping(1) == 4
+```
+
+## Testing
+
+The tests for this library are driven by pytest and require connection to an AV Access device.
+
+```bash
+pytest
 ```
```

### Comparing `pyavaccess-0.1.0/pyproject.toml` & `pyavaccess-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyavaccess"
-version = "0.1.0"
+version = "0.2.0"
 description = "Automation library for AV Access devices"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

### Comparing `pyavaccess-0.1.0/PKG-INFO` & `pyavaccess-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyavaccess
-Version: 0.1.0
+Version: 0.2.0
 Summary: Automation library for AV Access devices
 Project-URL: Source Code, https://github.com/latelylk/pyavaccess
 Project-URL: Bug Reports, https://github.com/latelylk/pyavaccess/issues
 License: GPLv3+
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -48,9 +48,17 @@
 for output, input in outputMap.items():
     print("Output {} is mapped to input {}".format(output, input))
 
 # Set the input for output 1 to input 4
 av.mapOutput(1, 4)
 
 # Check that the mapping was successful
-assert av.getMapping(1)[1] == 4
+assert av.getMapping(1) == 4
+```
+
+## Testing
+
+The tests for this library are driven by pytest and require connection to an AV Access device.
+
+```bash
+pytest
 ```
```

