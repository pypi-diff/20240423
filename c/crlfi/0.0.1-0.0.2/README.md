# Comparing `tmp/crlfi-0.0.1.tar.gz` & `tmp/crlfi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crlfi-0.0.1.tar", last modified: Tue Apr 23 06:04:33 2024, max compression
+gzip compressed data, was "crlfi-0.0.2.tar", last modified: Tue Apr 23 09:21:43 2024, max compression
```

## Comparing `crlfi-0.0.1.tar` & `crlfi-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 06:04:33.179744 crlfi-0.0.1/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-23 05:50:39.000000 crlfi-0.0.1/LICENSE
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4992 2024-04-23 06:04:33.179512 crlfi-0.0.1/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4539 2024-04-23 05:50:50.000000 crlfi-0.0.1/README.md
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 06:04:33.175716 crlfi-0.0.1/crlfi.egg-info/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4992 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)      454 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/SOURCES.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/dependency_links.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       40 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/entry_points.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/requires.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        4 2024-04-23 06:04:33.000000 crlfi-0.0.1/crlfi.egg-info/top_level.txt
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 06:04:33.176079 crlfi-0.0.1/cve/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-23 05:42:44.000000 crlfi-0.0.1/cve/__init__.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 06:04:33.177564 crlfi-0.0.1/cve/includes/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:26:47.000000 crlfi-0.0.1/cve/includes/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      629 2024-04-23 06:03:03.000000 crlfi-0.0.1/cve/includes/bot.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      456 2024-04-23 06:03:12.000000 crlfi-0.0.1/cve/includes/filereader.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2248 2024-04-23 06:03:29.000000 crlfi-0.0.1/cve/includes/scan.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-21 11:46:48.000000 crlfi-0.0.1/cve/includes/writefile.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1724 2024-04-23 06:02:23.000000 crlfi-0.0.1/cve/main.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 06:04:33.179001 crlfi-0.0.1/cve/utils/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:25:36.000000 crlfi-0.0.1/cve/utils/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1946 2024-04-23 06:02:44.000000 crlfi-0.0.1/cve/utils/configure.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      662 2024-04-21 12:31:26.000000 crlfi-0.0.1/cve/utils/const.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-21 12:43:27.000000 crlfi-0.0.1/cve/utils/helpers.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-02-12 08:19:58.000000 crlfi-0.0.1/cve/utils/status.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-23 06:04:33.179825 crlfi-0.0.1/setup.cfg
--rw-r--r--   0 karthikeyan   (501) staff       (20)      978 2024-04-23 05:49:45.000000 crlfi-0.0.1/setup.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.391711 crlfi-0.0.2/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-23 05:50:39.000000 crlfi-0.0.2/LICENSE
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4947 2024-04-23 09:21:43.391546 crlfi-0.0.2/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4494 2024-04-23 07:31:35.000000 crlfi-0.0.2/README.md
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.387386 crlfi-0.0.2/crlfi.egg-info/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4947 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      454 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       40 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/entry_points.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/requires.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        4 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/top_level.txt
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.387888 crlfi-0.0.2/cve/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-23 05:42:44.000000 crlfi-0.0.2/cve/__init__.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.389745 crlfi-0.0.2/cve/includes/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:26:47.000000 crlfi-0.0.2/cve/includes/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      629 2024-04-23 06:03:03.000000 crlfi-0.0.2/cve/includes/bot.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      456 2024-04-23 06:03:12.000000 crlfi-0.0.2/cve/includes/filereader.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     2248 2024-04-23 06:03:29.000000 crlfi-0.0.2/cve/includes/scan.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-21 11:46:48.000000 crlfi-0.0.2/cve/includes/writefile.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1724 2024-04-23 06:02:23.000000 crlfi-0.0.2/cve/main.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.391121 crlfi-0.0.2/cve/utils/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:25:36.000000 crlfi-0.0.2/cve/utils/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1946 2024-04-23 06:02:44.000000 crlfi-0.0.2/cve/utils/configure.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      796 2024-04-23 08:50:24.000000 crlfi-0.0.2/cve/utils/const.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-21 12:43:27.000000 crlfi-0.0.2/cve/utils/helpers.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-02-12 08:19:58.000000 crlfi-0.0.2/cve/utils/status.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-23 09:21:43.391834 crlfi-0.0.2/setup.cfg
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      978 2024-04-23 09:21:40.000000 crlfi-0.0.2/setup.py
```

### Comparing `crlfi-0.0.1/LICENSE` & `crlfi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/PKG-INFO` & `crlfi-0.0.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: crlfi
-Version: 0.0.1
-Author: @cappriciosec
-Author-email: <contact@cappriciosec.com>
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Cappricio-Securities/CVE-2023-29489/main/images/CVE-2023-29489.png" alt="logo">
 </div>
 
 
 ## Badges
 
 
 
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
-![PyPI - Version](https://img.shields.io/pypi/v/CVE-2023-29489)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/CVE-2023-29489)
-![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-<a href="https://github.com/Cappricio-Securities/CVE-2023-29489/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/CVE-2023-29489"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+![PyPI - Version](https://img.shields.io/pypi/v/crlfi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/crlfi)
+![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/crlfi/total)
+<a href="https://github.com/Cappricio-Securities/crlfi/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/crlfi"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
 <p align="center">
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,25 +1,17 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.1 Author: @cappriciosec Author-
-email:
-cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
-MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
 ## Badges [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)]
 (https://choosealicense.com/licenses/mit/) ![PyPI - Version](https://
-img.shields.io/pypi/v/CVE-2023-29489) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/CVE-2023-29489) ![GitHub all releases](https://
-img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_C_V_E_-_2_0_2_3_-_2_9_4_8_9_]!
-[Profile_view](https://komarev.com/ghpvc/?username=Cappricio-
-Securities&label=Profile%20views&color=0e75b6&style=flat) [![Follow Twitter]
-(https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://
-twitter.com/cappricio_sec)
+img.shields.io/pypi/v/crlfi) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/crlfi) ![GitHub all releases](https://img.shields.io/github/downloads/
+Cappricio-Securities/crlfi/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
+_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_r_l_f_i_]![Profile_view](https://komarev.com/ghpvc/
+?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+[![Follow Twitter](https://img.shields.io/twitter/follow/
+cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
 via pip - ```bash pip install CVE-2023-29489 ``` - Run bellow command to check
 - `CVE-2023-29489 -h` ## Configurations 2. We integrated with the Telegram API
    to receive instant notifications for vulnerability detection. - Telegram
   Notification - ```bash CVE-2023-29489 --chatid ``` - Open your telegram and
```

### Comparing `crlfi-0.0.1/README.md` & `crlfi-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,36 @@
+Metadata-Version: 2.1
+Name: crlfi
+Version: 0.0.2
+Author: @cappriciosec
+Author-email: <contact@cappriciosec.com>
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 <div align="center">
   <img src="https://raw.githubusercontent.com/Cappricio-Securities/CVE-2023-29489/main/images/CVE-2023-29489.png" alt="logo">
 </div>
 
 
 ## Badges
 
 
 
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
-![PyPI - Version](https://img.shields.io/pypi/v/CVE-2023-29489)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/CVE-2023-29489)
-![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-<a href="https://github.com/Cappricio-Securities/CVE-2023-29489/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/CVE-2023-29489"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+![PyPI - Version](https://img.shields.io/pypi/v/crlfi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/crlfi)
+![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/crlfi/total)
+<a href="https://github.com/Cappricio-Securities/crlfi/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/crlfi"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
 <p align="center">
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,18 +1,24 @@
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.2 Author: @cappriciosec Author-
+email:
+cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
+MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
+Content-Type: text/markdown License-File: LICENSE
                                     [logo]
 ## Badges [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)]
 (https://choosealicense.com/licenses/mit/) ![PyPI - Version](https://
-img.shields.io/pypi/v/CVE-2023-29489) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/CVE-2023-29489) ![GitHub all releases](https://
-img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_C_V_E_-_2_0_2_3_-_2_9_4_8_9_]!
-[Profile_view](https://komarev.com/ghpvc/?username=Cappricio-
-Securities&label=Profile%20views&color=0e75b6&style=flat) [![Follow Twitter]
-(https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://
-twitter.com/cappricio_sec)
+img.shields.io/pypi/v/crlfi) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/crlfi) ![GitHub all releases](https://img.shields.io/github/downloads/
+Cappricio-Securities/crlfi/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
+_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_r_l_f_i_]![Profile_view](https://komarev.com/ghpvc/
+?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+[![Follow Twitter](https://img.shields.io/twitter/follow/
+cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
 via pip - ```bash pip install CVE-2023-29489 ``` - Run bellow command to check
 - `CVE-2023-29489 -h` ## Configurations 2. We integrated with the Telegram API
    to receive instant notifications for vulnerability detection. - Telegram
   Notification - ```bash CVE-2023-29489 --chatid ``` - Open your telegram and
```

### Comparing `crlfi-0.0.1/crlfi.egg-info/PKG-INFO` & `crlfi-0.0.2/crlfi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.1
+Version: 0.0.2
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
@@ -19,18 +19,18 @@
 
 
 ## Badges
 
 
 
 [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
-![PyPI - Version](https://img.shields.io/pypi/v/CVE-2023-29489)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/CVE-2023-29489)
-![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-<a href="https://github.com/Cappricio-Securities/CVE-2023-29489/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/CVE-2023-29489"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+![PyPI - Version](https://img.shields.io/pypi/v/crlfi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/crlfi)
+![GitHub all releases](https://img.shields.io/github/downloads/Cappricio-Securities/crlfi/total)
+<a href="https://github.com/Cappricio-Securities/crlfi/releases/"><img src="https://img.shields.io/github/release/Cappricio-Securities/crlfi"></a>![Profile_view](https://komarev.com/ghpvc/?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
 <p align="center">
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.1 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.2 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
 ## Badges [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)]
 (https://choosealicense.com/licenses/mit/) ![PyPI - Version](https://
-img.shields.io/pypi/v/CVE-2023-29489) ![PyPI - Downloads](https://
-img.shields.io/pypi/dm/CVE-2023-29489) ![GitHub all releases](https://
-img.shields.io/github/downloads/Cappricio-Securities/CVE-2023-29489/total)
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_C_V_E_-_2_0_2_3_-_2_9_4_8_9_]!
-[Profile_view](https://komarev.com/ghpvc/?username=Cappricio-
-Securities&label=Profile%20views&color=0e75b6&style=flat) [![Follow Twitter]
-(https://img.shields.io/twitter/follow/cappricio_sec?style=social)](https://
-twitter.com/cappricio_sec)
+img.shields.io/pypi/v/crlfi) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/crlfi) ![GitHub all releases](https://img.shields.io/github/downloads/
+Cappricio-Securities/crlfi/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
+_C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_r_l_f_i_]![Profile_view](https://komarev.com/ghpvc/
+?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
+[![Follow Twitter](https://img.shields.io/twitter/follow/
+cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
 via pip - ```bash pip install CVE-2023-29489 ``` - Run bellow command to check
 - `CVE-2023-29489 -h` ## Configurations 2. We integrated with the Telegram API
    to receive instant notifications for vulnerability detection. - Telegram
   Notification - ```bash CVE-2023-29489 --chatid ``` - Open your telegram and
```

### Comparing `crlfi-0.0.1/cve/includes/bot.py` & `crlfi-0.0.2/cve/includes/bot.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/cve/includes/scan.py` & `crlfi-0.0.2/cve/includes/scan.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/cve/main.py` & `crlfi-0.0.2/cve/main.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/cve/utils/configure.py` & `crlfi-0.0.2/cve/utils/configure.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/cve/utils/const.py` & `crlfi-0.0.2/cve/utils/const.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  */
 
 
 """
 
 
 class Data:
-    blog = 'https://blogs.cappriciosec.com/blog/137/crlfi'
+    blog = 'https://blogs.cappriciosec.com/blog/138/Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty'
     api = 'https://api.cappriciosec.com/Telegram/cappriciosecbot.php'
     config_path = '~/.config/cappriciosec-tools/cappriciosec.yaml'
     payloadurl = 'https://raw.githubusercontent.com/Cappricio-Securities/PayloadAllTheThings/main/crlfi.txt'
     bugname = 'CRLF Injection'
 
 
 class Colors:
```

### Comparing `crlfi-0.0.1/cve/utils/helpers.py` & `crlfi-0.0.2/cve/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.1/setup.py` & `crlfi-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A Tool to find an Easy Bounty - crlfi'
 LONG_DESCRIPTION = 'This is a tool used by several security researchers to find Carriage Return Line Feed Injection Bug'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

