# Comparing `tmp/pySatlantic-0.4.1.tar.gz` & `tmp/pysatlantic-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nils/PycharmProjects/pySatlantic/dist/.tmp-kjp5qnl8/pySatlantic-0.4.1.tar", last modified: Wed Dec  7 17:57:05 2022, max compression
+gzip compressed data, was "pysatlantic-0.4.2.tar", last modified: Mon Apr 22 22:44:57 2024, max compression
```

## Comparing `pySatlantic-0.4.1.tar` & `pysatlantic-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nils       (501) staff       (20)        0 2022-12-07 17:57:05.806528 pySatlantic-0.4.1/
--rw-r--r--   0 nils       (501) staff       (20)     1070 2020-05-17 22:47:30.000000 pySatlantic-0.4.1/LICENSE
--rw-r--r--   0 nils       (501) staff       (20)     3659 2022-12-07 17:57:05.806127 pySatlantic-0.4.1/PKG-INFO
--rw-r--r--   0 nils       (501) staff       (20)     3045 2021-02-14 22:29:39.000000 pySatlantic-0.4.1/README.md
-drwxr-xr-x   0 nils       (501) staff       (20)        0 2022-12-07 17:57:05.802670 pySatlantic-0.4.1/pySatlantic/
--rw-r--r--   0 nils       (501) staff       (20)       48 2021-09-07 15:05:11.000000 pySatlantic-0.4.1/pySatlantic/__init__.py
--rw-r--r--   0 nils       (501) staff       (20)     1032 2019-12-28 23:13:19.000000 pySatlantic-0.4.1/pySatlantic/__main__.py
--rw-r--r--   0 nils       (501) staff       (20)     1972 2020-10-13 14:03:11.000000 pySatlantic-0.4.1/pySatlantic/dev.py
--rw-r--r--   0 nils       (501) staff       (20)    56206 2022-06-27 23:25:44.000000 pySatlantic-0.4.1/pySatlantic/instrument.py
--rw-r--r--   0 nils       (501) staff       (20)    19387 2021-09-07 15:18:43.000000 pySatlantic-0.4.1/pySatlantic/test.py
-drwxr-xr-x   0 nils       (501) staff       (20)        0 2022-12-07 17:57:05.805659 pySatlantic-0.4.1/pySatlantic.egg-info/
--rw-r--r--   0 nils       (501) staff       (20)     3659 2022-12-07 17:57:05.000000 pySatlantic-0.4.1/pySatlantic.egg-info/PKG-INFO
--rw-r--r--   0 nils       (501) staff       (20)      313 2022-12-07 17:57:05.000000 pySatlantic-0.4.1/pySatlantic.egg-info/SOURCES.txt
--rw-r--r--   0 nils       (501) staff       (20)        1 2022-12-07 17:57:05.000000 pySatlantic-0.4.1/pySatlantic.egg-info/dependency_links.txt
--rw-r--r--   0 nils       (501) staff       (20)        6 2022-12-07 17:57:05.000000 pySatlantic-0.4.1/pySatlantic.egg-info/requires.txt
--rw-r--r--   0 nils       (501) staff       (20)       12 2022-12-07 17:57:05.000000 pySatlantic-0.4.1/pySatlantic.egg-info/top_level.txt
--rw-r--r--   0 nils       (501) staff       (20)       38 2022-12-07 17:57:05.806640 pySatlantic-0.4.1/setup.cfg
--rw-r--r--   0 nils       (501) staff       (20)      902 2020-05-17 23:28:23.000000 pySatlantic-0.4.1/setup.py
+drwxr-xr-x   0 nils       (501) staff       (20)        0 2024-04-22 22:44:57.804030 pysatlantic-0.4.2/
+-rw-r--r--   0 nils       (501) staff       (20)     1070 2020-05-17 22:47:30.000000 pysatlantic-0.4.2/LICENSE
+-rw-r--r--   0 nils       (501) staff       (20)     3680 2024-04-22 22:44:57.803572 pysatlantic-0.4.2/PKG-INFO
+-rw-r--r--   0 nils       (501) staff       (20)     3045 2023-03-13 18:41:01.000000 pysatlantic-0.4.2/README.md
+drwxr-xr-x   0 nils       (501) staff       (20)        0 2024-04-22 22:44:57.799638 pysatlantic-0.4.2/pySatlantic/
+-rw-r--r--   0 nils       (501) staff       (20)       48 2024-04-22 20:50:15.000000 pysatlantic-0.4.2/pySatlantic/__init__.py
+-rw-r--r--   0 nils       (501) staff       (20)     1032 2019-12-28 23:13:19.000000 pysatlantic-0.4.2/pySatlantic/__main__.py
+-rw-r--r--   0 nils       (501) staff       (20)     1972 2020-10-13 14:03:11.000000 pysatlantic-0.4.2/pySatlantic/dev.py
+-rw-r--r--   0 nils       (501) staff       (20)    56468 2024-04-22 22:07:31.000000 pysatlantic-0.4.2/pySatlantic/instrument.py
+-rw-r--r--   0 nils       (501) staff       (20)    19387 2023-03-13 18:41:01.000000 pysatlantic-0.4.2/pySatlantic/test.py
+drwxr-xr-x   0 nils       (501) staff       (20)        0 2024-04-22 22:44:57.803039 pysatlantic-0.4.2/pySatlantic.egg-info/
+-rw-r--r--   0 nils       (501) staff       (20)     3680 2024-04-22 22:44:57.000000 pysatlantic-0.4.2/pySatlantic.egg-info/PKG-INFO
+-rw-r--r--   0 nils       (501) staff       (20)      313 2024-04-22 22:44:57.000000 pysatlantic-0.4.2/pySatlantic.egg-info/SOURCES.txt
+-rw-r--r--   0 nils       (501) staff       (20)        1 2024-04-22 22:44:57.000000 pysatlantic-0.4.2/pySatlantic.egg-info/dependency_links.txt
+-rw-r--r--   0 nils       (501) staff       (20)        6 2024-04-22 22:44:57.000000 pysatlantic-0.4.2/pySatlantic.egg-info/requires.txt
+-rw-r--r--   0 nils       (501) staff       (20)       12 2024-04-22 22:44:57.000000 pysatlantic-0.4.2/pySatlantic.egg-info/top_level.txt
+-rw-r--r--   0 nils       (501) staff       (20)       38 2024-04-22 22:44:57.804120 pysatlantic-0.4.2/setup.cfg
+-rw-r--r--   0 nils       (501) staff       (20)      902 2020-05-17 23:28:23.000000 pysatlantic-0.4.2/setup.py
```

### Comparing `pySatlantic-0.4.1/LICENSE` & `pysatlantic-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pySatlantic-0.4.1/PKG-INFO` & `pysatlantic-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pySatlantic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Unpack binary messages from Satlantic instruments.
 Home-page: https://github.com/OceanOptics/pySatlantic/
 Author: Nils Haentjens
 Author-email: nils.haentjens@maine.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 pySatlantic
 ===========
 [![Python 3](https://img.shields.io/badge/Python-3-blue.svg)](https://www.python.org/downloads/)
 [![license MIT](https://img.shields.io/badge/license-MIT-green)](https://github.com/OceanOptics/pySatlantic/blob/master/LICENSE)
 
 _Python package to unpack binary messages from Satlantic instruments._
```

### Comparing `pySatlantic-0.4.1/README.md` & `pysatlantic-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pySatlantic-0.4.1/pySatlantic/__main__.py` & `pysatlantic-0.4.2/pySatlantic/__main__.py`

 * *Files identical despite different names*

### Comparing `pySatlantic-0.4.1/pySatlantic/dev.py` & `pysatlantic-0.4.2/pySatlantic/dev.py`

 * *Files identical despite different names*

### Comparing `pySatlantic-0.4.1/pySatlantic/instrument.py` & `pysatlantic-0.4.2/pySatlantic/instrument.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,18 +58,18 @@
 FrameContainer = namedtuple('FrameContainer', ['header', 'data', 'timestamp', 'valid'])
 
 
 def sat_dtype_to_np_dtype(sat_data_type, sat_field_length):
     if sat_data_type == 'AS':
         # ASCII string (text)
         if sat_field_length:
-            return f'<{sat_field_length}U'
+            return '<{}U'.format(sat_field_length)
         else:
             # Assume maximum size of 12 characters
-            return f'<12U'
+            return '<12U'
     elif sat_data_type == 'AI':
         # ASCII integer number
         return np.int32
     elif sat_data_type == 'AF':
         # ASCII floating point number
         return np.float32
     elif sat_data_type == 'BS' and sat_field_length == 1:
@@ -93,15 +93,15 @@
     elif sat_data_type == 'BF' and sat_field_length == 4:
         # float
         return np.float32
     elif sat_data_type == 'BD' and sat_field_length == 8:
         # double float
         return np.float64
     else:
-        raise ParserTypeError(f'Unknown format decoder {sat_data_type}{sat_field_length}')
+        raise ParserTypeError('Unknown format decoder {}{}'.format(sat_data_type, sat_field_length))
 
 
 class Parser:
     """
     The Parser class builds a parser from Satlantic Calibration or Telemetry Definition Files (cal or tdf).
         Parser contains information to unpack binary data or split ascii data into meaningful fields.
         The Parser also contains information to calibrate fields from engineering units to calibration units
@@ -355,67 +355,67 @@
                     self.frame_length += self.field_length[i]
                     self.frame_fmt += self._sat_dtype_to_struct(self.data_type[i], self.field_length[i])
 
             # Check for variable frame length data type
             if self.variable_frame_length:
                 for t in self.data_type:
                     if t not in ['AS', 'AI', 'AF']:
-                        raise ParserTypeError(f"Invalid data type {t} for variable frame length.")
+                        raise ParserTypeError("Invalid data type {} for variable frame length.".format(t))
 
             # Special case of NMEA_CHECKSUM (not documented in SAT-DN-00134)
             #       data-type should be AI but it's an hexadecimal int instead of int.
             if 'NMEA_CHECKSUM' in self.key:
                 i = self.key.index('NMEA_CHECKSUM')
                 self.type[i] = 'CHECK'
                 self.id[i] = 'SUM'
-                self.key[i] = f'{self.type}_{self.id}'
+                self.key[i] = '{}_{}'.format(self.type, self.id)
                 self.data_type[i] = 'AI16'
 
             # Specify end of check sum computation
             if not self.variable_frame_length and 'CHECK_SUM' in self.key:
                 self.check_sum_index = -self.field_length[self.key.index('CHECK_SUM')]
                 if 'TERMINATOR' in self.id:
                     self.check_sum_index -= self.field_length[self.id.index('TERMINATOR')]
                 elif 'TERMINATOR' in self.type:
                     self.check_sum_index -= self.field_length[self.type.index('TERMINATOR')]
 
             # Group Variables
             self.core_variables = [i for i, (x, y) in enumerate(zip(self.type, self.fit_type))
                                    if x.upper() in self.CORE_VARIABLE_TYPES and y != 'NONE']
             if self.core_variables:
-                self.core_groupname = f'{self.type[self.core_variables[0]]}'
+                self.core_groupname = str(self.type[self.core_variables[0]])
             self.unusable_variables = [i for i, (x, y) in enumerate(zip(self.type, self.fit_type))
                                        if x.upper() in self.CORE_VARIABLE_TYPES and y == 'NONE']
             if self.unusable_variables:
-                self.unusable_groupname = f'{self.type[self.core_variables[0]]}_RAW'
+                self.unusable_groupname = '{}_RAW'.format(self.type[self.core_variables[0]])
             self.auxiliary_variables = [i for i, (x, y) in enumerate(zip(self.type, self.fit_type)) if
                                         x.upper() not in self.CORE_VARIABLE_TYPES]
 
             # Convert calibration coefficients to numpy array for fast computation
             if self.core_variables:
                 self.core_cal_coefs = np.array(itemgetter(*self.core_variables)(self.cal_coefs)).transpose()
             if self.unusable_variables:
                 self.unusable_cal_coefs = np.array(itemgetter(*self.unusable_variables)(self.cal_coefs)).transpose()
 
             # Check if data_type is valid for fit type
             for data, fit in zip(self.data_type, self.fit_type):
                 if fit in ['OPTIC1', 'DDMMYY']:
                     if data not in ['BU', 'BS', 'AI']:
-                        raise ParserTypeError(f"Valid data types for OPTIC1 are BU, BS, and AI.")
+                        raise ParserTypeError("Valid data types for OPTIC1 are BU, BS, and AI.")
                 elif fit in ['GPSTIME', 'GPSPOS', 'DDMM', 'HHMMSS']:
                     if data not in ['BF', 'BD', 'AF']:
-                        raise ParserTypeError(f"Valid data types for {fit} are BF, BD, and AF.")
+                        raise ParserTypeError("Valid data types for {} are BF, BD, and AF.".format(fit))
                 elif fit in ['OPTIC2', 'OPTIC3', 'THERM1', 'POW10', 'POLYU', 'POLYF', 'TIME2']:
                     if data == 'AS':
-                        raise ParserTypeError(f"All data types are valid with {fit}, except AS.")
+                        raise ParserTypeError("All data types are valid with {}, except AS.".format(fit))
                 elif fit in ['GPSHEMI', 'GPSMODE', 'GPSSTATUS']:
                     if data != 'AS':
-                        raise ParserTypeError(f"The only valid data type for {fit} is AS.")
+                        raise ParserTypeError("The only valid data type for {} is AS.".format(fit))
                 elif fit not in ['COUNT', 'NONE', 'DELIMITER']:
-                    raise ParserFitError(f"Fit type {fit} not supported.")
+                    raise ParserFitError("Fit type {} not supported.".format(fit))
 
     @staticmethod
     def _sat_dtype_to_struct(sat_data_type, sat_field_length):
         if sat_field_length is None:
             raise CalibrationFileError('Field length must be an integer for fixed length frames.')
         if sat_data_type == 'AS':
             # ASCII string (text)
@@ -447,30 +447,30 @@
         elif sat_data_type == 'BF' and sat_field_length == 4:
             # float
             return 'f'
         elif sat_data_type == 'BD' and sat_field_length == 8:
             # double float
             return 'd'
         else:
-            raise ParserTypeError(f'Unknown byte decoder combination {sat_data_type} {sat_field_length}')
+            raise ParserTypeError('Unknown byte decoder combination {} {}'.format(sat_data_type, sat_field_length))
 
     def __str__(self):
-        return f'{self.frame_header}\n' + \
-               f'\tInstrument: {self.instrument}\n' + \
-               f'\tSerial number: {self.sn}\n' + \
-               f'\tNumber of fields: {self.frame_nfields}\n' + \
-               f'\tVariable frame length: {self.variable_frame_length}\n' + \
-               f'\tFrame length (in bytes): {self.frame_length}\n' + \
-               f'\tVariables type: {self.type}\n' + \
-               f'\tVariables id: {self.id}\n' + \
-               f'\tVariables units: {self.units}\n' + \
-               f'\tVariables fit type:{self.fit_type}\n' + \
-               f'\tVariables field length: {self.field_length}\n' + \
-               f'\tVariables data type: {self.data_type}\n' + \
-               f'\tVariables frame format: {self.frame_fmt}\n'
+        return '{}\n'.format(self.frame_header) + \
+               '\tInstrument: {}\n'.format(self.instrument) + \
+               '\tSerial number: {}\n'.format(self.sn) + \
+               '\tNumber of fields: {}\n'.format(self.frame_nfields) + \
+               '\tVariable frame length: {}\n'.format(self.variable_frame_length) + \
+               '\tFrame length (in bytes): {}\n'.format(self.frame_length) + \
+               '\tVariables type: {}\n'.format(self.type) + \
+               '\tVariables id: {}\n'.format(self.id) + \
+               '\tVariables units: {}\n'.format(self.units) + \
+               '\tVariables fit type:{}\n'.format(self.fit_type) + \
+               '\tVariables field length: {}\n'.format(self.field_length) + \
+               '\tVariables data type: {}\n'.format(self.data_type) + \
+               '\tVariables frame format: {}\n'.format(self.frame_fmt)
 
 
 class Instrument:
     """
     Instrument class parse raw data from Satlantic instruments (HyperSAS, HyperNAV) if calibration files are passed
     """
 
@@ -502,26 +502,26 @@
             elif os.path.isfile(f):
                 ext = os.path.splitext(f)[1]
                 if ext in self.VALID_SIP_EXTENSIONS:
                     self.read_sip_file(f, immersed)
                 elif ext in self.VALID_CAL_EXTENSIONS:
                     self.read_calibration_file(f, immersed)
                 else:
-                    raise CalibrationFileExtensionError(f'File extension incorrect: {f}')
+                    raise CalibrationFileExtensionError('File extension incorrect: {}'.format(f))
             else:
-                raise FileNotFoundError(f'No such file or directory: {f}')
+                raise FileNotFoundError('No such file or directory: {}'.format(f))
 
     def read_calibration_file(self, filename, immersed=False):
         ext = os.path.splitext(filename)[1]
         if ext in self.VALID_CAL_EXTENSIONS:
             foo = Parser(filename, immersed)
             self.cal[foo.frame_header] = foo
             self.max_frame_header_length = max(self.max_frame_header_length, len(foo.frame_header))
         else:
-            raise CalibrationFileExtensionError(f'File extension incorrect: {f}')
+            raise CalibrationFileExtensionError('File extension incorrect: {}'.format(f))
 
     def read_calibration_dir(self, dirname, immersed=False):
         empty_dir = True
         for fn in os.listdir(dirname):
             if os.path.isfile(os.path.join(dirname, fn)) and \
                     os.path.splitext(fn)[1] in self.VALID_CAL_EXTENSIONS and os.path.basename(fn)[0] != '.':
                 # File exist, valide extension, and not hidden file
@@ -915,15 +915,15 @@
             # GPS system status.
             return True if value == 'A' else False
         elif fit_type == 'DDMM':
             # GPS global position in degrees, minutes, and seconds.
             d = int(value / 100)
             m = int(value - d * 100)
             s = int(((value - d * 100) - m) * 60)
-            return f'{d} {m}\' {s}\'\''
+            return '{} {}\' {}\'\''.format(d, m, s)
         elif fit_type == 'HHMMSS':
             # Universal Coordinated Time of GPS data in hours, minutes, and seconds.
             # DIVERGE FROM SATLANTIC SPECIFICATIONS CONVERT TO PYTHON timedelta
             hh = int(value / 10000)
             mm = int((value - hh * 10000) / 100)
             ss = value - hh * 10000 - mm * 100
             return timedelta(hours=hh, minutes=mm, seconds=ss)
@@ -942,15 +942,15 @@
             # Raw or un-calibrated information.
             return value
         elif fit_type == 'NONE':
             # Unusable data. (Used if frame data is to be ignored)
             # warnings('Fit type processing should not be applied to a NONE sensor.')
             return None
         else:
-            raise ParserFitError(f"Fit type {fit_type} not supported.")
+            raise ParserFitError("Fit type {} not supported.".format(fit_type))
 
     @staticmethod
     def compute_check_sum(frame, check_sum_index=-3):
         # Last byte of the sum of all bytes substracted from 0
         #   from frame header (included) to checksum (excluded)
         return np.uint8(0 - sum(frame[0:check_sum_index]))
 
@@ -1003,15 +1003,15 @@
                         if len(buffer) >= 7:
                             # Get SatView timestamp
                             ts = buffer[:7]
                             buffer = buffer[7:]
                             # Parse timestamp
                             ts = unpack('!ii', b'\x00' + ts)
                             try:
-                                timestamp = datetime.strptime(f'{ts[0]}{ts[1]:09d}000', '%Y%j%H%M%S%f')
+                                timestamp = datetime.strptime('{}{:09d}000', '%Y%j%H%M%S%f'.format(ts[0], ts[1]))
                             except ValueError as e:
                                 warnings.warn('Time Impossible, frame likely corrupted.')
                                 timestamp = 'NaN'
                                 invalid_timestamps += 1
                             # Calibrate frame
                             parsed_frame, valid = self.parse_frame(frame, frame_header, **kwargs)
                             if valid == True or valid is None:
@@ -1186,38 +1186,38 @@
             if not frame_header:
                 frame_header = frame[0:10].decode(self.instrument.ENCODING, self.instrument.UNICODE_HANDLING)
             [parsed_frame, valid_frame] = self.instrument.parse_frame(frame, frame_header,
                                                                       flag_get_auxiliary_variables=True)
         except FrameHeaderNotFoundError:
             if frame_header not in self.missing_frame_header:
                 self.missing_frame_header.append(frame_header)
-                warnings.warn(f'Missing calibration file for: {frame_header}')
+                warnings.warn('Missing calibration file for: {}'.format(frame_header))
             return
         except FrameLengthError as e:
             print(e)
             return
         if valid_frame:
             self.frame_parsed += 1
         # Write data
         if self.instrument.cal[frame_header].core_variables:
             data = next(iter(parsed_frame.values())).tolist()
-            data = ["%.10f" % v for v in data]
+            data = ['%.10f' % v for v in data]
             for k in [k for i, k in enumerate(self.instrument.cal[frame_header].key) if
                       i in self.instrument.cal[frame_header].auxiliary_variables]:
                 if k in parsed_frame.keys():
                     if isinstance(parsed_frame[k], float):
-                        data.append('%.4f' % parsed_frame[k])
+                        data.append(':.4f'.format(parsed_frame[k]))
                     else:
                         data.append(str(parsed_frame[k]))
         else:
             data = []
             for k in self.instrument.cal[frame_header].key:
                 if k in parsed_frame.keys():
                     if isinstance(parsed_frame[k], float):
-                        data.append('%.4f' % parsed_frame[k])
+                        data.append(':.4f'.format(parsed_frame[k]))
                     else:
                         data.append(str(parsed_frame[k]))
         self.w[frame_header].write([timestamp] + data)
 
     def __del__(self):
         if hasattr(self, 'w'):
             for k in self.w.keys():
```

### Comparing `pySatlantic-0.4.1/pySatlantic/test.py` & `pysatlantic-0.4.2/pySatlantic/test.py`

 * *Files identical despite different names*

### Comparing `pySatlantic-0.4.1/pySatlantic.egg-info/PKG-INFO` & `pysatlantic-0.4.2/pySatlantic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pySatlantic
-Version: 0.4.1
+Version: 0.4.2
 Summary: Unpack binary messages from Satlantic instruments.
 Home-page: https://github.com/OceanOptics/pySatlantic/
 Author: Nils Haentjens
 Author-email: nils.haentjens@maine.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
 pySatlantic
 ===========
 [![Python 3](https://img.shields.io/badge/Python-3-blue.svg)](https://www.python.org/downloads/)
 [![license MIT](https://img.shields.io/badge/license-MIT-green)](https://github.com/OceanOptics/pySatlantic/blob/master/LICENSE)
 
 _Python package to unpack binary messages from Satlantic instruments._
```

### Comparing `pySatlantic-0.4.1/setup.py` & `pysatlantic-0.4.2/setup.py`

 * *Files identical despite different names*

