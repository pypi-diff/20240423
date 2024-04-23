# Comparing `tmp/sa818-0.2.5.tar.gz` & `tmp/sa818-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sa818-0.2.5.tar", last modified: Mon Apr 22 20:04:23 2024, max compression
+gzip compressed data, was "sa818-0.2.6.tar", last modified: Tue Apr 23 16:00:59 2024, max compression
```

## Comparing `sa818-0.2.5.tar` & `sa818-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-22 20:04:23.260045 sa818-0.2.5/
--rw-r--r--   0 fred       (501) staff       (20)       70 2024-04-19 14:31:50.000000 sa818-0.2.5/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)     1321 2020-12-25 18:38:33.000000 sa818-0.2.5/LICENSE
--rw-r--r--   0 fred       (501) staff       (20)     1086 2024-04-22 20:04:23.259786 sa818-0.2.5/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)     4982 2024-03-15 15:47:46.000000 sa818-0.2.5/README.md
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-22 20:04:23.258123 sa818-0.2.5/docs/
--rw-r--r--   0 fred       (501) staff       (20)   316331 2020-12-25 22:25:10.000000 sa818-0.2.5/docs/IMG_0716.JPG
--rw-r--r--   0 fred       (501) staff       (20)   816814 2023-01-05 21:00:46.000000 sa818-0.2.5/docs/SA818_moduleV3.4.pdf
--rw-r--r--   0 fred       (501) staff       (20)   232499 2020-12-25 17:28:59.000000 sa818-0.2.5/docs/SA818_programming_manual.pdf
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-22 20:04:23.259609 sa818-0.2.5/sa818.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)     1086 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      300 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)       37 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/entry_points.txt
--rw-r--r--   0 fred       (501) staff       (20)        9 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/requires.txt
--rw-r--r--   0 fred       (501) staff       (20)        6 2024-04-22 20:04:23.000000 sa818-0.2.5/sa818.egg-info/top_level.txt
--rwxr-xr-x   0 fred       (501) staff       (20)    12941 2024-04-22 20:03:50.000000 sa818-0.2.5/sa818.py
--rw-r--r--   0 fred       (501) staff       (20)       38 2024-04-22 20:04:23.260078 sa818-0.2.5/setup.cfg
--rw-r--r--   0 fred       (501) staff       (20)     1564 2024-04-22 20:03:33.000000 sa818-0.2.5/setup.py
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-23 16:00:59.828189 sa818-0.2.6/
+-rw-r--r--   0 fred       (501) staff       (20)       70 2024-04-19 14:31:50.000000 sa818-0.2.6/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)     1321 2020-12-25 18:38:33.000000 sa818-0.2.6/LICENSE
+-rw-r--r--   0 fred       (501) staff       (20)     5975 2024-04-23 16:00:59.827977 sa818-0.2.6/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)     5313 2024-04-23 15:37:24.000000 sa818-0.2.6/README.md
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-23 16:00:59.826434 sa818-0.2.6/docs/
+-rw-r--r--   0 fred       (501) staff       (20)   316331 2020-12-25 22:25:10.000000 sa818-0.2.6/docs/IMG_0716.JPG
+-rw-r--r--   0 fred       (501) staff       (20)   816814 2023-01-05 21:00:46.000000 sa818-0.2.6/docs/SA818_moduleV3.4.pdf
+-rw-r--r--   0 fred       (501) staff       (20)   232499 2020-12-25 17:28:59.000000 sa818-0.2.6/docs/SA818_programming_manual.pdf
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-23 16:00:59.827815 sa818-0.2.6/sa818.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)     5975 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      300 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)       37 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/entry_points.txt
+-rw-r--r--   0 fred       (501) staff       (20)        9 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/requires.txt
+-rw-r--r--   0 fred       (501) staff       (20)        6 2024-04-23 16:00:59.000000 sa818-0.2.6/sa818.egg-info/top_level.txt
+-rwxr-xr-x   0 fred       (501) staff       (20)    13491 2024-04-23 15:45:47.000000 sa818-0.2.6/sa818.py
+-rw-r--r--   0 fred       (501) staff       (20)       38 2024-04-23 16:00:59.828222 sa818-0.2.6/setup.cfg
+-rw-r--r--   0 fred       (501) staff       (20)     1435 2024-04-23 15:55:02.000000 sa818-0.2.6/setup.py
```

### Comparing `sa818-0.2.5/LICENSE` & `sa818-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sa818-0.2.5/README.md` & `sa818-0.2.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 [root@allstar ~]# sa818 version
 SA818: INFO: Firmware version: V4.2
 
 [root@allstar ~]# sa818 radio --frequency 145.230 --offset -.6 --ctcss 100
 SA818: INFO: +DMOSETGROUP:0, BW: Wide, Frequency (RX: 145.2300 / TX: 144.6300), CTCSS (TX: 100.0 / RX: 100.0), squelch: 4, OK
 
 [root@allstar ~]# sa818 volume --level 5
-SA818: INFO: +DMOSETVOLUME:0 Volume level: 5
+SA818: INFO: +DMOSETVOLUME:0 Volume level: 5, OK
 ```
 
 If you use an FTDI dongle to program the SA828 module the USB port can
 be specified with the `--port` argument
 
 ```
 [root@allstar ~]# sa818 --port /dev/ttyAMA0 volume --level 5
@@ -63,70 +63,77 @@
 
  - radio: Program the radio's frequency, tone and squelch level
  - volume: Set the volume level
  - filters: Turn on or off the [pre/de]-emphasis and as well as the high and low pass filter
  - version: display the firmware version of the SA818 module
 
 ```
-usage: sa818 [-h] [--port PORT] [--debug]
+usage: sa818 [-h] [--debug] [--port PORT]
+                [--speed {300,1200,2400,4800,9600,19200,38400,57600,115200}]
                 {radio,volume,filters,version} ...
 
 generate configuration for switch port
 
 positional arguments:
   {radio,volume,filters,version}
     radio               Program the radio (frequency/tome/squelch)
     volume              Set the volume level
-    filters             Set filters
+    filters             Enable/Disable filters
     version             Show the firmware version of the SA818
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
-  --port PORT           Serial port [default: linux console port]
   --debug
+  --port PORT           Serial port [default: linux console port]
+  --speed {300,1200,2400,4800,9600,19200,38400,57600,115200}
+                        Connection speed
 ```
 
 ### Radio
 
 ```
-usage: sa818 radio [-h] --frequency FREQUENCY [--offset OFFSET]
-                      [--squelch SQUELCH] [--ctcss CTCSS | --dcs DCS]
+usage: sa818 radio [-h] [--bw {0,1}] --frequency FREQUENCY
+                      [--offset OFFSET] [--squelch SQUELCH]
+                      [--ctcss CTCSS | --dcs DCS] [--tail TAIL]
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
+  --bw {0,1}            Bandwidth 0=NARROW (12.5KHz), 1=WIDE (25KHx) [default:
+                        WIDE]
   --frequency FREQUENCY
-                        Transmit frequency
-  --offset OFFSET       0.0 for no offset [default: 0.0]
-  --squelch SQUELCH     Squelch value (1 to 9) [default: 4]
+                        Receive frequency
+  --offset OFFSET       Offset in MHz, 0 for no offset [default: 0.0]
+  --squelch SQUELCH     Squelch value (0 to 8) [default: 4]
   --ctcss CTCSS         CTCSS (PL Tone) 0 for no CTCSS [default: None]
-  --dcs DCS             DCS code must me the number followed by [N normal] or
+  --dcs DCS             DCS code must be the number followed by [N normal] or
                         [I inverse] [default: None]
+  --tail TAIL           Close CTCSS Tail Tone (Open/Close)
 ```
 
 ### Volume
 
 ```
 usage: sa818 volume [-h] [--level LEVEL]
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   --level LEVEL  Volume value (1 to 8) [default: 4]
 ```
 
 ### Filters
 
 ```
-usage: sa818 filters [-h] [--emphasis EMPHASIS] [--highpass HIGHPASS]
-                        [--lowpass LOWPASS]
+usage: sa818 filters [-h] --emphasis EMPHASIS --highpass HIGHPASS --lowpass
+                        LOWPASS
 
-optional arguments:
+options:
   -h, --help           show this help message and exit
-  --emphasis EMPHASIS  Disable [Pr/De]-emphasis (yes/no) [default: no]
-  --highpass HIGHPASS  Disable high pass filter (yes/no) [default: no]
-  --lowpass LOWPASS    Disable low pass filters (yes/no) [default: no]
+  --emphasis EMPHASIS  [Pr/De]-emphasis (Enable/Disable)
+  --highpass HIGHPASS  High pass filter (Enable/Disable)
+  --lowpass LOWPASS    Low pass filters (Enable/Disable)
 ```
 
 ## CTCSS codes (PL Tones)
 ```
 67.0, 71.9, 74.4, 77.0, 79.7, 82.5, 85.4, 88.5, 91.5, 94.8, 97.4,
 100.0, 103.5, 107.2, 110.9, 114.8, 118.8, 123.0, 127.3, 131.8, 136.5,
 141.3, 146.2, 151.4, 156.7, 162.2, 167.9, 173.8, 179.9, 186.2, 192.8,
```

### Comparing `sa818-0.2.5/docs/IMG_0716.JPG` & `sa818-0.2.6/docs/IMG_0716.JPG`

 * *Files identical despite different names*

### Comparing `sa818-0.2.5/docs/SA818_moduleV3.4.pdf` & `sa818-0.2.6/docs/SA818_moduleV3.4.pdf`

 * *Files identical despite different names*

### Comparing `sa818-0.2.5/docs/SA818_programming_manual.pdf` & `sa818-0.2.6/docs/SA818_programming_manual.pdf`

 * *Files identical despite different names*

### Comparing `sa818-0.2.5/sa818.py` & `sa818-0.2.6/sa818.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
     if not isinstance(self.serial, serial.Serial):
       raise IOError('Error openning the serial port')
 
     self.send(self.INIT)
     reply = self.readline()
     if reply != "+DMOCONNECT:0":
-      raise SystemError('Connection error')
+      raise SystemError('Connection error') from None
 
   def close(self):
     self.serial.close()
 
   def send(self, *args):
     data = ','.join(args)
     logger.debug('Sending: %s', data)
@@ -149,60 +149,62 @@
         msg = "%s, BW: %s Frequency (RX: %s / TX: %s), DCD (TX: %s / RX: %s), squelch: %s, OK"
         logger.info(msg, response, bw_label, rx_freq, tx_freq,
                     tx_tone, rx_tone, opts.squelch)
       else:
         msg = "%s, BW: %s, RX frequency: %s, TX frequency: %s, squelch: %s, OK"
         logger.info(msg, response, bw_label, rx_freq, tx_freq, opts.squelch)
 
-    if opts.close_tail is not None and opts.ctcss is not None:
-      self.close_tail(opts)
-    elif opts.close_tail is not None:
-      logger.warning('Ignoring "--close-tail" specified without ctcss')
+    if opts.tail is not None and opts.ctcss is not None:
+      self.tail(opts)
+    elif opts.tail is not None:
+      logger.warning('Ignoring "--tail" specified without ctcss')
 
   def set_filter(self, opts):
-    _yn = {True: "Yes", False: "No"}
+    for key in ("emphasis", "highpass", "lowpass"):
+      if getattr(opts, key) is None:
+        setattr(opts, key, 1)
+    _rx = {0: 'enabled', 1: 'disabled'}
     # filters are pre-emphasis, high-pass, low-pass
-    cmd = (f"{self.FILTER}={int(not opts.emphasis)},"
-           f"{int(not opts.highpass)},{int(not opts.lowpass)}")
+    cmd = (f"{self.FILTER}={opts.emphasis},{opts.highpass},{opts.lowpass}")
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETFILTER:0":
       logger.error('SA818 set filter error')
     else:
       logger.info("%s filters [Pre/De]emphasis: %s, high-pass: %s, low-pass: %s",
-                  response, _yn[opts.emphasis], _yn[opts.highpass], _yn[opts.lowpass])
+                  response, _rx[opts.emphasis], _rx[opts.highpass], _rx[opts.lowpass])
 
   def set_volume(self, opts):
     cmd = f"{self.VOLUME}={opts.level:d}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETVOLUME:0":
       logger.error('SA818 set volume error')
     else:
       logger.info("%s Volume level: %d, OK", response, opts.level)
 
-  def close_tail(self, opts):
-    _yn = {True: "Yes", False: "No"}
-    cmd = f"{self.TAIL}={int(opts.close_tail)}"
+  def tail(self, opts):
+    _oc = {True: "open", False: "close"}
+    cmd = f"{self.TAIL}={int(opts.tail)}"
     self.send(cmd)
     time.sleep(1)
     response = self.readline()
     if response != "+DMOSETTAIL:0":
       logger.error('SA818 set filter error')
     else:
-      logger.info("%s close tail: %s", response, _yn[opts.close_tail])
+      logger.info("%s tail: %s", response, _oc[opts.tail])
 
 
 def type_frequency(parg):
   try:
     frequency = float(parg)
   except ValueError:
-    raise argparse.ArgumentTypeError from None
+    raise argparse.ArgumentError from None
 
   if not 144 < frequency < 148 and not 420 < frequency < 450:
     logger.error('Frequency outside the amateur bands')
     raise argparse.ArgumentError
   return frequency
 
 
@@ -278,28 +280,30 @@
 
   if value not in range(1, 9):
     logger.error('The value must must be between 1 and 8 (inclusive)')
     raise argparse.ArgumentError
   return value
 
 
-def yesno(parg):
-  yes_strings = ["y", "yes", "true", "1", "on"]
-  no_strings = ["n", "no", "false", "0", "off"]
-  if parg.lower() in yes_strings:
-    return True
-  if parg.lower() in no_strings:
-    return False
-  raise argparse.ArgumentError
+def enabledisable(parg):
+  if parg.lower() == 'enable':
+    return 0
+  if parg.lower() == 'disable':
+    return 1
+  raise argparse.ArgumentTypeError("Possible values are [Enable/Disable]") from None
 
 
-def noneyesno(parg):
-  if parg is not None:
-    return yesno(parg)
-  return None
+def openclose(parg):
+  if parg is None:
+    return None
+  if parg.lower() in "open":
+    return True
+  if parg.lower() in "close":
+    return False
+  raise argparse.ArgumentTypeError("Possible values are [Open/Close]") from None
 
 
 def set_loglevel():
   loglevel = os.getenv('LOGLEVEL', 'INFO')
   loglevel = loglevel.upper()
   try:
     logger.root.setLevel(loglevel)
@@ -320,16 +324,15 @@
     "DCS Codes:\n"
     "DCS codes must be followed by N or I for Normal or Inverse:\n",
     f"> Example: 047I\n{chr(10).join(dcs)}"
   )
   return ''.join(codes)
 
 
-def main():
-  set_loglevel()
+def command_parser():
   parser = argparse.ArgumentParser(
     description="generate configuration for switch port",
     epilog=format_codes(),
     formatter_class=argparse.RawDescriptionHelpFormatter,
   )
   parser.add_argument("--debug", action="store_true", default=False)
   parser.add_argument("--port", type=str,
@@ -350,57 +353,73 @@
                        help="Squelch value (0 to 8) [default: %(default)s]")
   code_group = p_radio.add_mutually_exclusive_group()
   code_group.add_argument("--ctcss", default=None, type=type_ctcss,
                           help="CTCSS (PL Tone) 0 for no CTCSS [default: %(default)s]")
   code_group.add_argument("--dcs", default=None, type=type_dcs,
                           help=("DCS code must be the number followed by [N normal] or "
                                 "[I inverse]  [default: %(default)s]"))
-  p_radio.add_argument("--close-tail", default=None, type=noneyesno,
-                       help="Close CTCSS Tail Tone (yes/no)")
+  p_radio.add_argument("--tail", default=None, type=openclose,
+                       help="Close CTCSS Tail Tone (Open/Close)")
 
   p_volume = subparsers.add_parser("volume", help="Set the volume level")
   p_volume.set_defaults(func="volume")
   p_volume.add_argument("--level", type=type_level, default=4,
                         help="Volume value (1 to 8) [default: %(default)s]")
 
-  p_filter = subparsers.add_parser("filters", help="Set/Unset filters")
+  p_filter = subparsers.add_parser("filters", aliases=['filter'], help="Enable/Disable filters")
   p_filter.set_defaults(func="filters")
-  p_filter.add_argument("--emphasis", type=yesno, required=True,
-                        help="Disable [Pr/De]-emphasis (yes/no)")
-  p_filter.add_argument("--highpass", type=yesno, required=True,
-                        help="Disable high pass filter (yes/no)")
-  p_filter.add_argument("--lowpass", type=yesno, required=True,
-                        help="Disable low pass filters (yes/no)")
+  p_filter.add_argument("--emphasis", type=enabledisable,
+                        help="[Pr/De]-emphasis (Enable/Disable) [default: disable]")
+  p_filter.add_argument("--highpass", type=enabledisable,
+                        help="High pass filter (Enable/Disable) [default: disable]")
+  p_filter.add_argument("--lowpass", type=enabledisable,
+                        help="Low pass filters (Enable/Disable) [default: disable]")
 
   p_version = subparsers.add_parser("version", help="Show the firmware version of the SA818")
   p_version.set_defaults(func="version")
 
-  opts = parser.parse_args()
+  try:
+    opts = parser.parse_args()
+  except argparse.ArgumentTypeError as err:
+    parser.error(str(err))
+
   if not hasattr(opts, 'func'):
     print('sa818: error: the following arguments are required: {radio,volume,filters,version}\n'
           'use --help for more informatiion',
           file=sys.stderr)
-    raise SystemExit(os.EX_USAGE) from None
+    raise SystemExit('Argument Error') from None
+
+  return opts
+
+
+def main():
+  set_loglevel()
+  opts = command_parser()
 
   if opts.debug:
     logger.setLevel(logging.DEBUG)
 
   logger.debug(opts)
 
   try:
     radio = SA818(opts.port, opts.speed)
   except (IOError, SystemError) as err:
-    logger.error(err)
-    raise SystemExit(os.EX_IOERR) from None
+    raise SystemExit(err) from None
 
   if opts.func == 'version':
     radio.version()
   elif opts.func == 'radio':
     radio.set_radio(opts)
   elif opts.func == 'filters':
+    for key in ('emphasis', 'highpass', 'lowpass'):
+      if getattr(opts, key) is not None:
+        break
+    else:
+      logger.error('filters need at least one argument')
+      raise SystemExit('Argument error') from None
     radio.set_filter(opts)
   elif opts.func == 'volume':
     radio.set_volume(opts)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `sa818-0.2.5/setup.py` & `sa818-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,63 +10,56 @@
 
 from setuptools import setup
 
 __doc__ = """
 
 ## SA818 Programming
 
-Use this software to program the frequency, ctcss, dcs and filters ont
+Use this software to program the frequency, ctcss, dcs and filters on
 the radio module SA818
 
-### Installation
-
-```
-$ pip install sa818
-```
-
-### Example
-
-```
-$ sa818 radio --frequency 145.230 --offset -.6 --ctcss 100
-SA818: INFO: +DMOSETGROUP:0, RX frequency: 145.2300, TX frequency: 144.6300, ctcss: 100.0,
-squelch: 4, OK
-
-$ sa818 volume --level 5
-SA818: INFO: +DMOSETVOLUME:0 Volume level: 5
-```
-
 """
 
 __author__ = "Fred C. (W6BSD)"
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 __license__ = 'BSD'
 
 py_version = sys.version_info[:2]
 if py_version < (3, 8):
   raise RuntimeError('SA818 requires Python 3.8 or later')
 
-setup(
-  name='sa818',
-  version=__version__,
-  description='SA818 Programming Software',
-  long_description=__doc__,
-  long_description_content_type='text/markdown',
-  url='https://github.com/0x9900/SA818/',
-  license=__license__,
-  author=__author__,
-  author_email='w6bsd@bsdworld.org',
-  py_modules=['sa818'],
-  install_requires=['pyserial'],
-  entry_points={
-    'console_scripts': ['sa818 = sa818:main'],
-  },
-  classifiers=[
-    'Development Status :: 3 - Alpha',
-    'Intended Audience :: Developers',
-    'License :: OSI Approved :: BSD License',
-    'Operating System :: OS Independent',
-    'Programming Language :: Python',
-    'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.8',
-    'Topic :: Communications :: Ham Radio',
-  ],
-)
+
+def readme():
+  return open('README.md', 'r', encoding='utf-8').read()
+
+
+def main():
+  setup(
+    name='sa818',
+    version=__version__,
+    description='SA818 Programming Software',
+    long_description=readme(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/0x9900/SA818/',
+    license=__license__,
+    author=__author__,
+    author_email='w6bsd@bsdworld.org',
+    py_modules=['sa818'],
+    install_requires=['pyserial'],
+    entry_points={
+      'console_scripts': ['sa818 = sa818:main'],
+    },
+    classifiers=[
+      'Development Status :: 3 - Alpha',
+      'Intended Audience :: Developers',
+      'License :: OSI Approved :: BSD License',
+      'Operating System :: OS Independent',
+      'Programming Language :: Python',
+      'Programming Language :: Python :: 3',
+      'Programming Language :: Python :: 3.8',
+      'Topic :: Communications :: Ham Radio',
+    ],
+  )
+
+
+if __name__ == "__main__":
+  main()
```

