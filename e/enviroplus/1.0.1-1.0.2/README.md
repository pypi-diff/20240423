# Comparing `tmp/enviroplus-1.0.1.tar.gz` & `tmp/enviroplus-1.0.2.tar.gz`

## Comparing `enviroplus-1.0.1.tar` & `enviroplus-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 enviroplus-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    47407 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Enviro-Plus-pHAT.jpg
--rw-r--r--   0        0        0    46494 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Enviro-mini-pHAT.jpg
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 enviroplus-1.0.1/MANIFEST.in
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 enviroplus-1.0.1/Makefile
--rw-r--r--   0        0        0     4021 2020-02-02 00:00:00.000000 enviroplus-1.0.1/README.md
--rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 enviroplus-1.0.1/check.sh
--rwxr-xr-x   0        0        0     9938 2020-02-02 00:00:00.000000 enviroplus-1.0.1/install.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enviroplus-1.0.1/requirements-dev.txt
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tox.ini
--rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 enviroplus-1.0.1/uninstall.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/__init__.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/gas.py
--rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 enviroplus-1.0.1/enviroplus/noise.py
--rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/adc.py
--rwxr-xr-x   0        0        0     4674 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one-enviro-mini.py
--rwxr-xr-x   0        0        0     5301 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one-no-pm.py
--rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/all-in-one.py
--rwxr-xr-x   0        0        0    11341 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/combined.py
--rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/compensated-temperature.py
--rwxr-xr-x   0        0        0      470 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/gas.py
--rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/lcd.py
--rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/light.py
--rwxr-xr-x   0        0        0     7789 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/mqtt-all.py
--rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/noise-amps-at-freqs.py
--rwxr-xr-x   0        0        0      899 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/noise-profile.py
--rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/particulates.py
--rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/sensorcommunity.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/sensorcommunity_combined.py
--rwxr-xr-x   0        0        0    13209 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/weather-and-light.py
--rwxr-xr-x   0        0        0      679 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/weather.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-bright.png
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-dark.png
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-dim.png
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/bulb-light.png
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity-bad.png
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity-good.png
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/humidity.png
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/temperature.png
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-change.png
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-dry.png
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-fair.png
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-rain.png
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 enviroplus-1.0.1/examples/icons/weather-storm.png
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/test_noise.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 enviroplus-1.0.1/tests/test_setup.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 enviroplus-1.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 enviroplus-1.0.1/LICENSE
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 enviroplus-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 enviroplus-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 enviroplus-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    47407 2020-02-02 00:00:00.000000 enviroplus-1.0.2/Enviro-Plus-pHAT.jpg
+-rw-r--r--   0        0        0    46494 2020-02-02 00:00:00.000000 enviroplus-1.0.2/Enviro-mini-pHAT.jpg
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 enviroplus-1.0.2/MANIFEST.in
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 enviroplus-1.0.2/Makefile
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 enviroplus-1.0.2/README.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 enviroplus-1.0.2/check.sh
+-rwxr-xr-x   0        0        0     9938 2020-02-02 00:00:00.000000 enviroplus-1.0.2/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 enviroplus-1.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 enviroplus-1.0.2/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 enviroplus-1.0.2/uninstall.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enviroplus-1.0.2/enviroplus/__init__.py
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 enviroplus-1.0.2/enviroplus/gas.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 enviroplus-1.0.2/enviroplus/noise.py
+-rwxr-xr-x   0        0        0      512 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/adc.py
+-rwxr-xr-x   0        0        0     4674 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/all-in-one-enviro-mini.py
+-rwxr-xr-x   0        0        0     5301 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/all-in-one-no-pm.py
+-rwxr-xr-x   0        0        0     6535 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/all-in-one.py
+-rwxr-xr-x   0        0        0    11341 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/combined.py
+-rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/compensated-temperature.py
+-rwxr-xr-x   0        0        0      470 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/gas.py
+-rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/lcd.py
+-rwxr-xr-x   0        0        0      689 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/light.py
+-rwxr-xr-x   0        0        0     7789 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/mqtt-all.py
+-rwxr-xr-x   0        0        0     1190 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/noise-amps-at-freqs.py
+-rwxr-xr-x   0        0        0      899 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/noise-profile.py
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/particulates.py
+-rwxr-xr-x   0        0        0     6944 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/sensorcommunity.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/sensorcommunity_combined.py
+-rwxr-xr-x   0        0        0    13209 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/weather-and-light.py
+-rwxr-xr-x   0        0        0      679 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/weather.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/bulb-bright.png
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/bulb-dark.png
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/bulb-dim.png
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/bulb-light.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/humidity-bad.png
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/humidity-good.png
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/humidity.png
+-rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/temperature.png
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/weather-change.png
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/weather-dry.png
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/weather-fair.png
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/weather-rain.png
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 enviroplus-1.0.2/examples/icons/weather-storm.png
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 enviroplus-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 enviroplus-1.0.2/tests/test_noise.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 enviroplus-1.0.2/tests/test_setup.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 enviroplus-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 enviroplus-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 enviroplus-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 enviroplus-1.0.2/PKG-INFO
```

### Comparing `enviroplus-1.0.1/Enviro-Plus-pHAT.jpg` & `enviroplus-1.0.2/Enviro-Plus-pHAT.jpg`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/Enviro-mini-pHAT.jpg` & `enviroplus-1.0.2/Enviro-mini-pHAT.jpg`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/Makefile` & `enviroplus-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/README.md` & `enviroplus-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,70 @@
 # Enviro+
 
 Designed for environmental monitoring, Enviro+ lets you measure air quality (pollutant gases and particulates), temperature, pressure, humidity, light, and noise level. Learn more - https://shop.pimoroni.com/products/enviro-plus
 
-[![Build Status](https://travis-ci.com/pimoroni/enviroplus-python.svg?branch=master)](https://travis-ci.com/pimoroni/enviroplus-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/enviroplus-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/enviroplus-python?branch=master)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/enviroplus-python/test.yml?branch=main)](https://github.com/pimoroni/enviroplus-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/enviroplus-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/enviroplus-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/enviroplus.svg)](https://pypi.python.org/pypi/enviroplus)
 [![Python Versions](https://img.shields.io/pypi/pyversions/enviroplus.svg)](https://pypi.python.org/pypi/enviroplus)
 
 # Installing
 
 You are best using the "One-line" install method if you want all of the UART serial configuration for the PMS5003 particulate matter sensor to run automatically.
 
 **Note** The code in this repository supports both the Enviro+ and Enviro Mini boards. _The Enviro Mini board does not have the Gas sensor or the breakout for the PM sensor._
 
 ![Enviro Plus pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-Plus-pHAT.jpg)
 ![Enviro Mini pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-mini-pHAT.jpg)
 
 :warning: This library now supports Python 3 only, Python 2 is EOL - https://www.python.org/doc/sunset-python-2/
 
-## One-line (Installs from GitHub)
-
-```bash
-curl -sSL https://get.pimoroni.com/enviroplus | bash
-```
-
-**Note** report issues with one-line installer here: https://github.com/pimoroni/get
-
-## Or... Install and configure dependencies from GitHub:
+## Install and configure dependencies from GitHub:
 
 * `git clone https://github.com/pimoroni/enviroplus-python`
 * `cd enviroplus-python`
-* `sudo ./install.sh`
+* `./install.sh`
+
+**Note** Libraries will be installed in the "pimoroni" virtual environment, you will need to activate it to run examples:
+
+```
+source ~/.virtualenvs/pimoroni/bin/activate
+```
 
 **Note** Raspbian/Raspberry Pi OS Lite users may first need to install git: `sudo apt install git`
 
 ## Or... Install from PyPi and configure manually:
 
-* Run `sudo python3 -m pip install enviroplus`
+* `python3 -m venv --system-site-packages $HOME/.virtualenvs/pimoroni`
+* Run `python3 -m pip install enviroplus`
+
+And install additional dependencies:
+
+```bash
+sudo apt install python3-numpy python3-smbus python3-pil python3-setuptools
+```
 
 **Note** this will not perform any of the required configuration changes on your Pi, you may additionally need to:
 
 * Enable i2c: `raspi-config nonint do_i2c 0`
 * Enable SPI: `raspi-config nonint do_spi 0`
 
 And if you're using a PMS5003 sensor you will need to:
 
-* Enable serial: `raspi-config nonint set_config_var enable_uart 1 /boot/config.txt`
-* Disable serial terminal: `sudo raspi-config nonint do_serial 1`
+### Bookworm
+
+* Enable serial: `raspi-config nonint do_serial_hw 0`
+* Disable serial terminal: `raspi-config nonint do_serial_cons 1`
 * Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
 
-And install additional dependencies:
+### Bullseye
 
-```bash
-sudo apt install python3-numpy python3-smbus python3-pil python3-setuptools
-```
+* Enable serial: `raspi-config nonint set_config_var enable_uart 1 /boot/config.txt`
+* Disable serial terminal: `sudo raspi-config nonint do_serial 1`
+* Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
 
 ## Alternate Software & User Projects
 
 * Enviro Plus Dashboard - https://gitlab.com/dedSyn4ps3/enviroplus-dashboard - A React-based web dashboard for viewing sensor data
 * Enviro+ Example Projects - https://gitlab.com/dedSyn4ps3/enviroplus-python-projects - Includes original examples plus code to stream to Adafruit IO (more projects coming soon)
 * enviro monitor - https://github.com/roscoe81/enviro-monitor
 * mqtt-all - https://github.com/robmarkcole/rpi-enviro-mqtt - now upstream: [see examples/mqtt-all.py](examples/mqtt-all.py)
```

### Comparing `enviroplus-1.0.1/check.sh` & `enviroplus-1.0.2/check.sh`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/install.sh` & `enviroplus-1.0.2/install.sh`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/uninstall.sh` & `enviroplus-1.0.2/uninstall.sh`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/enviroplus/gas.py` & `enviroplus-1.0.2/enviroplus/gas.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     adc.set_mode("single")
     adc.set_programmable_gain(MICS6814_GAIN)
     if adc_type == "ADS1115":
         adc.set_sample_rate(128)
     else:
         adc.set_sample_rate(1600)
 
-    _heater = gpiodevice.get_pin("GPIO24")
+    _heater = gpiodevice.get_pin("GPIO24", "EnviroPlus", OUTH)
 
     atexit.register(cleanup)
 
 
 def available():
     setup()
     return _is_available
```

### Comparing `enviroplus-1.0.1/enviroplus/noise.py` & `enviroplus-1.0.2/enviroplus/noise.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/adc.py` & `enviroplus-1.0.2/examples/adc.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/all-in-one-enviro-mini.py` & `enviroplus-1.0.2/examples/all-in-one-enviro-mini.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/all-in-one-no-pm.py` & `enviroplus-1.0.2/examples/all-in-one-no-pm.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/all-in-one.py` & `enviroplus-1.0.2/examples/all-in-one.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/combined.py` & `enviroplus-1.0.2/examples/combined.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/compensated-temperature.py` & `enviroplus-1.0.2/examples/compensated-temperature.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/lcd.py` & `enviroplus-1.0.2/examples/lcd.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/light.py` & `enviroplus-1.0.2/examples/light.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/mqtt-all.py` & `enviroplus-1.0.2/examples/mqtt-all.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/noise-amps-at-freqs.py` & `enviroplus-1.0.2/examples/noise-amps-at-freqs.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/noise-profile.py` & `enviroplus-1.0.2/examples/noise-profile.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/particulates.py` & `enviroplus-1.0.2/examples/particulates.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/sensorcommunity.py` & `enviroplus-1.0.2/examples/sensorcommunity.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/sensorcommunity_combined.py` & `enviroplus-1.0.2/examples/sensorcommunity_combined.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/weather-and-light.py` & `enviroplus-1.0.2/examples/weather-and-light.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/weather.py` & `enviroplus-1.0.2/examples/weather.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/bulb-bright.png` & `enviroplus-1.0.2/examples/icons/bulb-bright.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/bulb-dark.png` & `enviroplus-1.0.2/examples/icons/bulb-dark.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/bulb-dim.png` & `enviroplus-1.0.2/examples/icons/bulb-dim.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/bulb-light.png` & `enviroplus-1.0.2/examples/icons/bulb-light.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/humidity-bad.png` & `enviroplus-1.0.2/examples/icons/humidity-bad.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/humidity-good.png` & `enviroplus-1.0.2/examples/icons/humidity-good.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/humidity.png` & `enviroplus-1.0.2/examples/icons/humidity.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/temperature.png` & `enviroplus-1.0.2/examples/icons/temperature.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/weather-change.png` & `enviroplus-1.0.2/examples/icons/weather-change.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/weather-dry.png` & `enviroplus-1.0.2/examples/icons/weather-dry.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/weather-fair.png` & `enviroplus-1.0.2/examples/icons/weather-fair.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/weather-rain.png` & `enviroplus-1.0.2/examples/icons/weather-rain.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/examples/icons/weather-storm.png` & `enviroplus-1.0.2/examples/icons/weather-storm.png`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/tests/conftest.py` & `enviroplus-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/tests/test_noise.py` & `enviroplus-1.0.2/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/tests/test_setup.py` & `enviroplus-1.0.2/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/LICENSE` & `enviroplus-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enviroplus-1.0.1/pyproject.toml` & `enviroplus-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -137,9 +137,9 @@
 ]
 commands = [
 	"printf \"Setting up i2c and SPI..\\n\"",
 	"sudo raspi-config nonint do_spi 0",
 	"sudo raspi-config nonint do_i2c 0",
 	"printf \"Setting up serial for PMS5003..\\n\"",
 	"sudo raspi-config nonint do_serial_cons 1",
-	"sudo raspi-config nonint do_serial_hw 1"
+	"sudo raspi-config nonint do_serial_hw 0"
 ]
```

### Comparing `enviroplus-1.0.1/PKG-INFO` & `enviroplus-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: enviroplus
-Version: 1.0.1
+Version: 1.0.2
 Summary: Enviro pHAT Plus environmental monitoring add-on for Raspberry Pi
 Project-URL: GitHub, https://www.github.com/pimoroni/enviroplus-python
 Project-URL: Homepage, https://www.pimoroni.com
 Author-email: Philip Howard <phil@pimoroni.com>
 Maintainer-email: Philip Howard <phil@pimoroni.com>
 License: MIT License
         
@@ -59,66 +59,73 @@
 Requires-Dist: st7735>=1.0.0
 Description-Content-Type: text/markdown
 
 # Enviro+
 
 Designed for environmental monitoring, Enviro+ lets you measure air quality (pollutant gases and particulates), temperature, pressure, humidity, light, and noise level. Learn more - https://shop.pimoroni.com/products/enviro-plus
 
-[![Build Status](https://travis-ci.com/pimoroni/enviroplus-python.svg?branch=master)](https://travis-ci.com/pimoroni/enviroplus-python)
-[![Coverage Status](https://coveralls.io/repos/github/pimoroni/enviroplus-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/enviroplus-python?branch=master)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/enviroplus-python/test.yml?branch=main)](https://github.com/pimoroni/enviroplus-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/enviroplus-python/badge.svg?branch=main)](https://coveralls.io/github/pimoroni/enviroplus-python?branch=main)
 [![PyPi Package](https://img.shields.io/pypi/v/enviroplus.svg)](https://pypi.python.org/pypi/enviroplus)
 [![Python Versions](https://img.shields.io/pypi/pyversions/enviroplus.svg)](https://pypi.python.org/pypi/enviroplus)
 
 # Installing
 
 You are best using the "One-line" install method if you want all of the UART serial configuration for the PMS5003 particulate matter sensor to run automatically.
 
 **Note** The code in this repository supports both the Enviro+ and Enviro Mini boards. _The Enviro Mini board does not have the Gas sensor or the breakout for the PM sensor._
 
 ![Enviro Plus pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-Plus-pHAT.jpg)
 ![Enviro Mini pHAT](https://raw.githubusercontent.com/pimoroni/enviroplus-python/main/Enviro-mini-pHAT.jpg)
 
 :warning: This library now supports Python 3 only, Python 2 is EOL - https://www.python.org/doc/sunset-python-2/
 
-## One-line (Installs from GitHub)
-
-```bash
-curl -sSL https://get.pimoroni.com/enviroplus | bash
-```
-
-**Note** report issues with one-line installer here: https://github.com/pimoroni/get
-
-## Or... Install and configure dependencies from GitHub:
+## Install and configure dependencies from GitHub:
 
 * `git clone https://github.com/pimoroni/enviroplus-python`
 * `cd enviroplus-python`
-* `sudo ./install.sh`
+* `./install.sh`
+
+**Note** Libraries will be installed in the "pimoroni" virtual environment, you will need to activate it to run examples:
+
+```
+source ~/.virtualenvs/pimoroni/bin/activate
+```
 
 **Note** Raspbian/Raspberry Pi OS Lite users may first need to install git: `sudo apt install git`
 
 ## Or... Install from PyPi and configure manually:
 
-* Run `sudo python3 -m pip install enviroplus`
+* `python3 -m venv --system-site-packages $HOME/.virtualenvs/pimoroni`
+* Run `python3 -m pip install enviroplus`
+
+And install additional dependencies:
+
+```bash
+sudo apt install python3-numpy python3-smbus python3-pil python3-setuptools
+```
 
 **Note** this will not perform any of the required configuration changes on your Pi, you may additionally need to:
 
 * Enable i2c: `raspi-config nonint do_i2c 0`
 * Enable SPI: `raspi-config nonint do_spi 0`
 
 And if you're using a PMS5003 sensor you will need to:
 
-* Enable serial: `raspi-config nonint set_config_var enable_uart 1 /boot/config.txt`
-* Disable serial terminal: `sudo raspi-config nonint do_serial 1`
+### Bookworm
+
+* Enable serial: `raspi-config nonint do_serial_hw 0`
+* Disable serial terminal: `raspi-config nonint do_serial_cons 1`
 * Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
 
-And install additional dependencies:
+### Bullseye
 
-```bash
-sudo apt install python3-numpy python3-smbus python3-pil python3-setuptools
-```
+* Enable serial: `raspi-config nonint set_config_var enable_uart 1 /boot/config.txt`
+* Disable serial terminal: `sudo raspi-config nonint do_serial 1`
+* Add `dtoverlay=pi3-miniuart-bt` to your `/boot/config.txt`
 
 ## Alternate Software & User Projects
 
 * Enviro Plus Dashboard - https://gitlab.com/dedSyn4ps3/enviroplus-dashboard - A React-based web dashboard for viewing sensor data
 * Enviro+ Example Projects - https://gitlab.com/dedSyn4ps3/enviroplus-python-projects - Includes original examples plus code to stream to Adafruit IO (more projects coming soon)
 * enviro monitor - https://github.com/roscoe81/enviro-monitor
 * mqtt-all - https://github.com/robmarkcole/rpi-enviro-mqtt - now upstream: [see examples/mqtt-all.py](examples/mqtt-all.py)
@@ -130,16 +137,23 @@
 
 ## Help & Support
 
 * GPIO Pinout - https://pinout.xyz/pinout/enviro_plus
 * Support forums - https://forums.pimoroni.com/c/support
 * Discord - https://discord.gg/hr93ByC
 
+1.0.2
+-----
+
+* README.md: Update install instructions
+* Fix installer to enable serial
+* Fix gas sensor heater pin
+
 1.0.1
------------
+-----
 
 * README.md: Fix images
 
 1.0.0
 -----
 
 * BREAKING: Port to gpiod/gpiodevice for Pi 5/Bookworm.
```

