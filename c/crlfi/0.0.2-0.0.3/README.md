# Comparing `tmp/crlfi-0.0.2.tar.gz` & `tmp/crlfi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crlfi-0.0.2.tar", last modified: Tue Apr 23 09:21:43 2024, max compression
+gzip compressed data, was "crlfi-0.0.3.tar", last modified: Tue Apr 23 09:27:57 2024, max compression
```

## Comparing `crlfi-0.0.2.tar` & `crlfi-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.391711 crlfi-0.0.2/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-23 05:50:39.000000 crlfi-0.0.2/LICENSE
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4947 2024-04-23 09:21:43.391546 crlfi-0.0.2/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4494 2024-04-23 07:31:35.000000 crlfi-0.0.2/README.md
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.387386 crlfi-0.0.2/crlfi.egg-info/
--rw-r--r--   0 karthikeyan   (501) staff       (20)     4947 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/PKG-INFO
--rw-r--r--   0 karthikeyan   (501) staff       (20)      454 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/SOURCES.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/dependency_links.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       40 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/entry_points.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/requires.txt
--rw-r--r--   0 karthikeyan   (501) staff       (20)        4 2024-04-23 09:21:43.000000 crlfi-0.0.2/crlfi.egg-info/top_level.txt
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.387888 crlfi-0.0.2/cve/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-23 05:42:44.000000 crlfi-0.0.2/cve/__init__.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.389745 crlfi-0.0.2/cve/includes/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:26:47.000000 crlfi-0.0.2/cve/includes/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      629 2024-04-23 06:03:03.000000 crlfi-0.0.2/cve/includes/bot.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      456 2024-04-23 06:03:12.000000 crlfi-0.0.2/cve/includes/filereader.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     2248 2024-04-23 06:03:29.000000 crlfi-0.0.2/cve/includes/scan.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-21 11:46:48.000000 crlfi-0.0.2/cve/includes/writefile.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1724 2024-04-23 06:02:23.000000 crlfi-0.0.2/cve/main.py
-drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:21:43.391121 crlfi-0.0.2/cve/utils/
--rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:25:36.000000 crlfi-0.0.2/cve/utils/__init__.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1946 2024-04-23 06:02:44.000000 crlfi-0.0.2/cve/utils/configure.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      796 2024-04-23 08:50:24.000000 crlfi-0.0.2/cve/utils/const.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-21 12:43:27.000000 crlfi-0.0.2/cve/utils/helpers.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-02-12 08:19:58.000000 crlfi-0.0.2/cve/utils/status.py
--rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-23 09:21:43.391834 crlfi-0.0.2/setup.cfg
--rw-r--r--   0 karthikeyan   (501) staff       (20)      978 2024-04-23 09:21:40.000000 crlfi-0.0.2/setup.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:27:57.945562 crlfi-0.0.3/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1074 2024-04-23 05:50:39.000000 crlfi-0.0.3/LICENSE
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4773 2024-04-23 09:27:57.945331 crlfi-0.0.3/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4320 2024-04-23 09:24:32.000000 crlfi-0.0.3/README.md
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:27:57.941058 crlfi-0.0.3/crlfi.egg-info/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     4773 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/PKG-INFO
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      454 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/SOURCES.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        1 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/dependency_links.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       40 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/entry_points.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       23 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/requires.txt
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        4 2024-04-23 09:27:57.000000 crlfi-0.0.3/crlfi.egg-info/top_level.txt
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:27:57.941410 crlfi-0.0.3/cve/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-04-23 05:42:44.000000 crlfi-0.0.3/cve/__init__.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:27:57.943200 crlfi-0.0.3/cve/includes/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:26:47.000000 crlfi-0.0.3/cve/includes/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      629 2024-04-23 06:03:03.000000 crlfi-0.0.3/cve/includes/bot.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      456 2024-04-23 06:03:12.000000 crlfi-0.0.3/cve/includes/filereader.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     2248 2024-04-23 06:03:29.000000 crlfi-0.0.3/cve/includes/scan.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      267 2024-04-21 11:46:48.000000 crlfi-0.0.3/cve/includes/writefile.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1724 2024-04-23 06:02:23.000000 crlfi-0.0.3/cve/main.py
+drwxr-xr-x   0 karthikeyan   (501) staff       (20)        0 2024-04-23 09:27:57.944795 crlfi-0.0.3/cve/utils/
+-rw-r--r--   0 karthikeyan   (501) staff       (20)        0 2024-01-04 13:25:36.000000 crlfi-0.0.3/cve/utils/__init__.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1946 2024-04-23 06:02:44.000000 crlfi-0.0.3/cve/utils/configure.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      796 2024-04-23 08:50:24.000000 crlfi-0.0.3/cve/utils/const.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)     1697 2024-04-21 12:43:27.000000 crlfi-0.0.3/cve/utils/helpers.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      227 2024-02-12 08:19:58.000000 crlfi-0.0.3/cve/utils/status.py
+-rw-r--r--   0 karthikeyan   (501) staff       (20)       38 2024-04-23 09:27:57.945632 crlfi-0.0.3/setup.cfg
+-rw-r--r--   0 karthikeyan   (501) staff       (20)      978 2024-04-23 09:27:53.000000 crlfi-0.0.3/setup.py
```

### Comparing `crlfi-0.0.2/LICENSE` & `crlfi-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/PKG-INFO` & `crlfi-0.0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: crlfi
-Version: 0.0.2
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
-  <img src="https://raw.githubusercontent.com/Cappricio-Securities/CVE-2023-29489/main/images/CVE-2023-29489.png" alt="logo">
+  <img src="https://raw.githubusercontent.com/Cappricio-Securities/crlfi/main/image/CRLFI.png" alt="logo">
 </div>
 
 
 ## Badges
 
 
 
@@ -46,107 +32,108 @@
 
 ## Installation 
 
 1. Install Python3 and pip [Instructions Here](https://www.python.org/downloads/) (If you can't figure this out, you shouldn't really be using this)
 
    - Install via pip
      - ```bash
-          pip install CVE-2023-29489 
+          pip install crlfi
         ```
    - Run bellow command to check
-     - `CVE-2023-29489 -h`
+     - `crlfi -h`
 
 ## Configurations 
 2. We integrated with the Telegram API to receive instant notifications for vulnerability detection.
    
    - Telegram Notification
      - ```bash
-          CVE-2023-29489 --chatid <YourTelegramChatID>
+          crlfi --chatid <YourTelegramChatID>
         ```
    - Open your telegram and search for [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/#@CappricioSecuritiesTools_bot) and click start
 
 ## Usages 
 3. This tool has multiple use cases.
    
    - To Check Single URL
      - ```bash
-          CVE-2023-29489 -u http://example.com 
+          crlfi -u http://example.com 
         ```
    - To Check List of URL 
       - ```bash
-          CVE-2023-29489 -i urls.txt 
+          crlfi -i urls.txt 
         ```
    - Save output into TXT file
       - ```bash
-          CVE-2023-29489 -i urls.txt -o out.txt
+          crlfi -i urls.txt -o out.txt
         ```
-   - Want to Learn about [`CVE-2023-29489`](https://blogs.cappriciosec.com/cve/137/CVE-2023-29489)? Then Type Below command
+   - Want to Learn about [`crlfi`](https://blogs.cappriciosec.com/blog/138/Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty)? Then Type Below command
       - ```bash
-          CVE-2023-29489 -b
+          crlfi -b
         ```
      
 <p align="center">
   <b>🚨 Disclaimer</b>
   
 </p>
 <p align="center">
 <b>This tool is created for security bug identification and assistance; Cappricio Securities is not liable for any illegal use. 
   Use responsibly within legal and ethical boundaries. 🔐🛡️</b></p>
 
 
 ## Working PoC Video
 
-[![asciicast](https://blogs.cappriciosec.com/uploaders/cve1.png)](https://asciinema.org/a/xB30FPnwpUJiqiyVzY20OutOD)
+[![asciicast](https://blogs.cappriciosec.com/uploaders/Screenshot%202024-04-23%20at%202.32.40%20PM.png)](https://asciinema.org/a/CZVs5PpxP7cFBvNAeNurt5hxt)
 
 
 
 
 ## Help menu
 
 #### Get all items
 
 ```bash
 👋 Hey Hacker
-                                                                v1.0
-  ______   ______    ___  ___  ___  ____    ___ ___  ____ ___ ___ 
- / ___/ | / / __/___|_  |/ _ \|_  ||_  /___|_  / _ \/ / /( _ ) _ \
-/ /__ | |/ / _//___/ __// // / __/_/_ <___/ __/\_, /_  _/ _  \_, /
-\___/ |___/___/   /____/\___/____/____/  /____/___/ /_/ \___/___/    
+                                v1.0
+   __________  __    __________
+  / ____/ __ \/ /   / ____/  _/
+ / /   / /_/ / /   / /_   / /
+/ /___/ _, _/ /___/ __/ _/ /
+\____/_/ /_/_____/_/   /___/
 
-                                   Developed By https://cappriciosec.com
+                                Developed By https://cappriciosec.com
 
 
-CVE-2023-29489 : Bug scanner for WebPentesters and Bugbounty Hunters 
+crlfi : Bug scanner for WebPentesters and Bugbounty Hunters 
 
-$ CVE-2023-29489 [option]
+$ crlfi [option]
 
-Usage: CVE-2023-29489 [options]
+Usage: crlfi [options]
 ```
 
 
 | Argument | Type     | Description                | Examples |
 | :-------- | :------- | :------------------------- | :------------------------- |
-| `-u` | `--url` | URL to scan | CVE-2023-29489 -u https://target.com |
-| `-i` | `--input` | filename Read input from txt  | CVE-2023-29489 -i target.txt | 
-| `-o` | `--output` | filename Write output in txt file | CVE-2023-29489 -i target.txt -o output.txt |
-| `-c` | `--chatid` | Creating Telegram Notification | CVE-2023-29489 --chatid yourid |
-| `-b` | `--blog` | To Read about CVE-2023-29489 Bug | CVE-2023-29489 -b |
-| `-h` | `--help` | Help Menu | CVE-2023-29489 -h |
+| `-u` | `--url` | URL to scan | crlfi -u https://target.com |
+| `-i` | `--input` | filename Read input from txt  | crlfi -i target.txt | 
+| `-o` | `--output` | filename Write output in txt file | crlfi -i target.txt -o output.txt |
+| `-c` | `--chatid` | Creating Telegram Notification | crlfi --chatid yourid |
+| `-b` | `--blog` | To Read about crlfi Bug | crlfi -b |
+| `-h` | `--help` | Help Menu | crlfi -h |
 
 
 
 ## 🔗 Links
 [![Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/)
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--v/)
 [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker)
 
 
 
 ## Author
 
-- [@karthithehacker](https://github.com/karthi-the-hacker/)
+- [@cappriciosec](https://github.com/cappricio-securities/)
 
 
 
 ## Feedback
 
-If you have any feedback, please reach out to us at contact@karthithehacker.com
+If you have any feedback, please reach out to us at contact@cappriciosec.com
```

#### html2text {}

```diff
@@ -1,59 +1,51 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.2 Author: @cappriciosec Author-
-email:
-cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
-Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
-MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
-Content-Type: text/markdown License-File: LICENSE
                                     [logo]
 ## Badges [![MIT License](https://img.shields.io/badge/License-MIT-green.svg)]
 (https://choosealicense.com/licenses/mit/) ![PyPI - Version](https://
 img.shields.io/pypi/v/crlfi) ![PyPI - Downloads](https://img.shields.io/pypi/
 dm/crlfi) ![GitHub all releases](https://img.shields.io/github/downloads/
 Cappricio-Securities/crlfi/total) _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/
 _C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_r_l_f_i_]![Profile_view](https://komarev.com/ghpvc/
 ?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/
 cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
-via pip - ```bash pip install CVE-2023-29489 ``` - Run bellow command to check
-- `CVE-2023-29489 -h` ## Configurations 2. We integrated with the Telegram API
-   to receive instant notifications for vulnerability detection. - Telegram
-  Notification - ```bash CVE-2023-29489 --chatid ``` - Open your telegram and
-   search for [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/
+via pip - ```bash pip install crlfi ``` - Run bellow command to check - `crlfi
+-h` ## Configurations 2. We integrated with the Telegram API to receive instant
+ notifications for vulnerability detection. - Telegram Notification - ```bash
+            crlfi --chatid ``` - Open your telegram and search for
+         [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/
   #@CappricioSecuritiesTools_bot) and click start ## Usages 3. This tool has
- multiple use cases. - To Check Single URL - ```bash CVE-2023-29489 -u http://
-example.com ``` - To Check List of URL - ```bash CVE-2023-29489 -i urls.txt ```
-- Save output into TXT file - ```bash CVE-2023-29489 -i urls.txt -o out.txt ```
- - Want to Learn about [`CVE-2023-29489`](https://blogs.cappriciosec.com/cve/
- 137/CVE-2023-29489)? Then Type Below command - ```bash CVE-2023-29489 -b ```
+multiple use cases. - To Check Single URL - ```bash crlfi -u http://example.com
+ ``` - To Check List of URL - ```bash crlfi -i urls.txt ``` - Save output into
+  TXT file - ```bash crlfi -i urls.txt -o out.txt ``` - Want to Learn about
+              [`crlfi`](https://blogs.cappriciosec.com/blog/138/
+Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty)?
+                Then Type Below command - ```bash crlfi -b ```
                                 ?ð???¨ DDiissccllaaiimmeerr
 TThhiiss ttooooll iiss ccrreeaatteedd ffoorr sseeccuurriittyy bbuugg iiddeennttiiffiiccaattiioonn aanndd aassssiissttaannccee;; CCaapppprriicciioo
 SSeeccuurriittiieess iiss nnoott lliiaabbllee ffoorr aannyy iilllleeggaall uussee.. UUssee rreessppoonnssiibbllyy wwiitthhiinn lleeggaall aanndd
                         eetthhiiccaall bboouunnddaarriieess.. ?ð????ð???¡?ï?¸?
 ## Working PoC Video [![asciicast](https://blogs.cappriciosec.com/uploaders/
-cve1.png)](https://asciinema.org/a/xB30FPnwpUJiqiyVzY20OutOD) ## Help menu ####
-Get all items ```bash ð Hey Hacker v1.0 ______ ______ ___ ___ ___ ____ ___
-___ ____ ___ ___ / ___/ | / / __/___|_ |/ _ \|_ ||_ /___|_ / _ \/ / /( _ ) _ \
-/ /__ | |/ / _//___/ __// // / __/_/_ <___/ __/\_, /_ _/ _ \_, / \___/ |___/
-___/ /____/\___/____/____/ /____/___/ /_/ \___/___/ Developed By https://
-cappriciosec.com CVE-2023-29489 : Bug scanner for WebPentesters and Bugbounty
-Hunters $ CVE-2023-29489 [option] Usage: CVE-2023-29489 [options] ``` |
-Argument | Type | Description | Examples | | :-------- | :------- | :----------
---------------- | :------------------------- | | `-u` | `--url` | URL to scan |
-CVE-2023-29489 -u https://target.com | | `-i` | `--input` | filename Read input
-from txt | CVE-2023-29489 -i target.txt | | `-o` | `--output` | filename Write
-output in txt file | CVE-2023-29489 -i target.txt -o output.txt | | `-c` | `--
-chatid` | Creating Telegram Notification | CVE-2023-29489 --chatid yourid | |
-`-b` | `--blog` | To Read about CVE-2023-29489 Bug | CVE-2023-29489 -b | | `-h`
-| `--help` | Help Menu | CVE-2023-29489 -h | ## ð Links [![Website](https://
-img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-
-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin](https://
-img.shields.io/badge/linkedin-0A66C2?style=for-the-
+Screenshot%202024-04-23%20at%202.32.40%20PM.png)](https://asciinema.org/a/
+CZVs5PpxP7cFBvNAeNurt5hxt) ## Help menu #### Get all items ```bash ð Hey
+Hacker v1.0 __________ __ __________ / ____/ __ \/ / / ____/ _/ / / / /_/ / / /
+/_ / / / /___/ _, _/ /___/ __/ _/ / \____/_/ /_/_____/_/ /___/ Developed By
+https://cappriciosec.com crlfi : Bug scanner for WebPentesters and Bugbounty
+Hunters $ crlfi [option] Usage: crlfi [options] ``` | Argument | Type |
+Description | Examples | | :-------- | :------- | :------------------------- |
+:------------------------- | | `-u` | `--url` | URL to scan | crlfi -u https://
+target.com | | `-i` | `--input` | filename Read input from txt | crlfi -
+i target.txt | | `-o` | `--output` | filename Write output in txt file | crlfi
+-i target.txt -o output.txt | | `-c` | `--chatid` | Creating Telegram
+Notification | crlfi --chatid yourid | | `-b` | `--blog` | To Read about crlfi
+Bug | crlfi -b | | `-h` | `--help` | Help Menu | crlfi -h | ## ð Links [!
+[Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-
+badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin]
+(https://img.shields.io/badge/linkedin-0A66C2?style=for-the-
 badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--
 v/) [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker) ##
-Author - [@karthithehacker](https://github.com/karthi-the-hacker/) ## Feedback
-If you have any feedback, please reach out to us at contact@karthithehacker.com
+Author - [@cappriciosec](https://github.com/cappricio-securities/) ## Feedback
+If you have any feedback, please reach out to us at contact@cappriciosec.com
```

### Comparing `crlfi-0.0.2/crlfi.egg-info/PKG-INFO` & `crlfi-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: crlfi
-Version: 0.0.2
+Version: 0.0.3
 Author: @cappriciosec
 Author-email: <contact@cappriciosec.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 <div align="center">
-  <img src="https://raw.githubusercontent.com/Cappricio-Securities/CVE-2023-29489/main/images/CVE-2023-29489.png" alt="logo">
+  <img src="https://raw.githubusercontent.com/Cappricio-Securities/crlfi/main/image/CRLFI.png" alt="logo">
 </div>
 
 
 ## Badges
 
 
 
@@ -46,107 +46,108 @@
 
 ## Installation 
 
 1. Install Python3 and pip [Instructions Here](https://www.python.org/downloads/) (If you can't figure this out, you shouldn't really be using this)
 
    - Install via pip
      - ```bash
-          pip install CVE-2023-29489 
+          pip install crlfi
         ```
    - Run bellow command to check
-     - `CVE-2023-29489 -h`
+     - `crlfi -h`
 
 ## Configurations 
 2. We integrated with the Telegram API to receive instant notifications for vulnerability detection.
    
    - Telegram Notification
      - ```bash
-          CVE-2023-29489 --chatid <YourTelegramChatID>
+          crlfi --chatid <YourTelegramChatID>
         ```
    - Open your telegram and search for [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/#@CappricioSecuritiesTools_bot) and click start
 
 ## Usages 
 3. This tool has multiple use cases.
    
    - To Check Single URL
      - ```bash
-          CVE-2023-29489 -u http://example.com 
+          crlfi -u http://example.com 
         ```
    - To Check List of URL 
       - ```bash
-          CVE-2023-29489 -i urls.txt 
+          crlfi -i urls.txt 
         ```
    - Save output into TXT file
       - ```bash
-          CVE-2023-29489 -i urls.txt -o out.txt
+          crlfi -i urls.txt -o out.txt
         ```
-   - Want to Learn about [`CVE-2023-29489`](https://blogs.cappriciosec.com/cve/137/CVE-2023-29489)? Then Type Below command
+   - Want to Learn about [`crlfi`](https://blogs.cappriciosec.com/blog/138/Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty)? Then Type Below command
       - ```bash
-          CVE-2023-29489 -b
+          crlfi -b
         ```
      
 <p align="center">
   <b>🚨 Disclaimer</b>
   
 </p>
 <p align="center">
 <b>This tool is created for security bug identification and assistance; Cappricio Securities is not liable for any illegal use. 
   Use responsibly within legal and ethical boundaries. 🔐🛡️</b></p>
 
 
 ## Working PoC Video
 
-[![asciicast](https://blogs.cappriciosec.com/uploaders/cve1.png)](https://asciinema.org/a/xB30FPnwpUJiqiyVzY20OutOD)
+[![asciicast](https://blogs.cappriciosec.com/uploaders/Screenshot%202024-04-23%20at%202.32.40%20PM.png)](https://asciinema.org/a/CZVs5PpxP7cFBvNAeNurt5hxt)
 
 
 
 
 ## Help menu
 
 #### Get all items
 
 ```bash
 👋 Hey Hacker
-                                                                v1.0
-  ______   ______    ___  ___  ___  ____    ___ ___  ____ ___ ___ 
- / ___/ | / / __/___|_  |/ _ \|_  ||_  /___|_  / _ \/ / /( _ ) _ \
-/ /__ | |/ / _//___/ __// // / __/_/_ <___/ __/\_, /_  _/ _  \_, /
-\___/ |___/___/   /____/\___/____/____/  /____/___/ /_/ \___/___/    
+                                v1.0
+   __________  __    __________
+  / ____/ __ \/ /   / ____/  _/
+ / /   / /_/ / /   / /_   / /
+/ /___/ _, _/ /___/ __/ _/ /
+\____/_/ /_/_____/_/   /___/
 
-                                   Developed By https://cappriciosec.com
+                                Developed By https://cappriciosec.com
 
 
-CVE-2023-29489 : Bug scanner for WebPentesters and Bugbounty Hunters 
+crlfi : Bug scanner for WebPentesters and Bugbounty Hunters 
 
-$ CVE-2023-29489 [option]
+$ crlfi [option]
 
-Usage: CVE-2023-29489 [options]
+Usage: crlfi [options]
 ```
 
 
 | Argument | Type     | Description                | Examples |
 | :-------- | :------- | :------------------------- | :------------------------- |
-| `-u` | `--url` | URL to scan | CVE-2023-29489 -u https://target.com |
-| `-i` | `--input` | filename Read input from txt  | CVE-2023-29489 -i target.txt | 
-| `-o` | `--output` | filename Write output in txt file | CVE-2023-29489 -i target.txt -o output.txt |
-| `-c` | `--chatid` | Creating Telegram Notification | CVE-2023-29489 --chatid yourid |
-| `-b` | `--blog` | To Read about CVE-2023-29489 Bug | CVE-2023-29489 -b |
-| `-h` | `--help` | Help Menu | CVE-2023-29489 -h |
+| `-u` | `--url` | URL to scan | crlfi -u https://target.com |
+| `-i` | `--input` | filename Read input from txt  | crlfi -i target.txt | 
+| `-o` | `--output` | filename Write output in txt file | crlfi -i target.txt -o output.txt |
+| `-c` | `--chatid` | Creating Telegram Notification | crlfi --chatid yourid |
+| `-b` | `--blog` | To Read about crlfi Bug | crlfi -b |
+| `-h` | `--help` | Help Menu | crlfi -h |
 
 
 
 ## 🔗 Links
 [![Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/)
 [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--v/)
 [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker)
 
 
 
 ## Author
 
-- [@karthithehacker](https://github.com/karthi-the-hacker/)
+- [@cappriciosec](https://github.com/cappricio-securities/)
 
 
 
 ## Feedback
 
-If you have any feedback, please reach out to us at contact@karthithehacker.com
+If you have any feedback, please reach out to us at contact@cappriciosec.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crlfi Version: 0.0.2 Author: @cappriciosec Author-
+Metadata-Version: 2.1 Name: crlfi Version: 0.0.3 Author: @cappriciosec Author-
 email:
 cappriciosec.com> Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Description-
 Content-Type: text/markdown License-File: LICENSE
                                     [logo]
@@ -14,46 +14,45 @@
 _C_a_p_p_r_i_c_i_o_-_S_e_c_u_r_i_t_i_e_s_/_c_r_l_f_i_]![Profile_view](https://komarev.com/ghpvc/
 ?username=Cappricio-Securities&label=Profile%20views&color=0e75b6&style=flat)
 [![Follow Twitter](https://img.shields.io/twitter/follow/
 cappricio_sec?style=social)](https://twitter.com/cappricio_sec)
  ## License [MIT](https://choosealicense.com/licenses/mit/) ## Installation 1.
 Install Python3 and pip [Instructions Here](https://www.python.org/downloads/)
  (If you can't figure this out, you shouldn't really be using this) - Install
-via pip - ```bash pip install CVE-2023-29489 ``` - Run bellow command to check
-- `CVE-2023-29489 -h` ## Configurations 2. We integrated with the Telegram API
-   to receive instant notifications for vulnerability detection. - Telegram
-  Notification - ```bash CVE-2023-29489 --chatid ``` - Open your telegram and
-   search for [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/
+via pip - ```bash pip install crlfi ``` - Run bellow command to check - `crlfi
+-h` ## Configurations 2. We integrated with the Telegram API to receive instant
+ notifications for vulnerability detection. - Telegram Notification - ```bash
+            crlfi --chatid ``` - Open your telegram and search for
+         [`@CappricioSecuritiesTools_bot`](https://web.telegram.org/k/
   #@CappricioSecuritiesTools_bot) and click start ## Usages 3. This tool has
- multiple use cases. - To Check Single URL - ```bash CVE-2023-29489 -u http://
-example.com ``` - To Check List of URL - ```bash CVE-2023-29489 -i urls.txt ```
-- Save output into TXT file - ```bash CVE-2023-29489 -i urls.txt -o out.txt ```
- - Want to Learn about [`CVE-2023-29489`](https://blogs.cappriciosec.com/cve/
- 137/CVE-2023-29489)? Then Type Below command - ```bash CVE-2023-29489 -b ```
+multiple use cases. - To Check Single URL - ```bash crlfi -u http://example.com
+ ``` - To Check List of URL - ```bash crlfi -i urls.txt ``` - Save output into
+  TXT file - ```bash crlfi -i urls.txt -o out.txt ``` - Want to Learn about
+              [`crlfi`](https://blogs.cappriciosec.com/blog/138/
+Cappricio%20Securities%20Discovers%20CRLF%20Injection%20Vulnerability%20in%20Popular%20Website,%20Responsible%20Disclosure%20Earns%20Bounty)?
+                Then Type Below command - ```bash crlfi -b ```
                                 ?ð???¨ DDiissccllaaiimmeerr
 TThhiiss ttooooll iiss ccrreeaatteedd ffoorr sseeccuurriittyy bbuugg iiddeennttiiffiiccaattiioonn aanndd aassssiissttaannccee;; CCaapppprriicciioo
 SSeeccuurriittiieess iiss nnoott lliiaabbllee ffoorr aannyy iilllleeggaall uussee.. UUssee rreessppoonnssiibbllyy wwiitthhiinn lleeggaall aanndd
                         eetthhiiccaall bboouunnddaarriieess.. ?ð????ð???¡?ï?¸?
 ## Working PoC Video [![asciicast](https://blogs.cappriciosec.com/uploaders/
-cve1.png)](https://asciinema.org/a/xB30FPnwpUJiqiyVzY20OutOD) ## Help menu ####
-Get all items ```bash ð Hey Hacker v1.0 ______ ______ ___ ___ ___ ____ ___
-___ ____ ___ ___ / ___/ | / / __/___|_ |/ _ \|_ ||_ /___|_ / _ \/ / /( _ ) _ \
-/ /__ | |/ / _//___/ __// // / __/_/_ <___/ __/\_, /_ _/ _ \_, / \___/ |___/
-___/ /____/\___/____/____/ /____/___/ /_/ \___/___/ Developed By https://
-cappriciosec.com CVE-2023-29489 : Bug scanner for WebPentesters and Bugbounty
-Hunters $ CVE-2023-29489 [option] Usage: CVE-2023-29489 [options] ``` |
-Argument | Type | Description | Examples | | :-------- | :------- | :----------
---------------- | :------------------------- | | `-u` | `--url` | URL to scan |
-CVE-2023-29489 -u https://target.com | | `-i` | `--input` | filename Read input
-from txt | CVE-2023-29489 -i target.txt | | `-o` | `--output` | filename Write
-output in txt file | CVE-2023-29489 -i target.txt -o output.txt | | `-c` | `--
-chatid` | Creating Telegram Notification | CVE-2023-29489 --chatid yourid | |
-`-b` | `--blog` | To Read about CVE-2023-29489 Bug | CVE-2023-29489 -b | | `-h`
-| `--help` | Help Menu | CVE-2023-29489 -h | ## ð Links [![Website](https://
-img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-
-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin](https://
-img.shields.io/badge/linkedin-0A66C2?style=for-the-
+Screenshot%202024-04-23%20at%202.32.40%20PM.png)](https://asciinema.org/a/
+CZVs5PpxP7cFBvNAeNurt5hxt) ## Help menu #### Get all items ```bash ð Hey
+Hacker v1.0 __________ __ __________ / ____/ __ \/ / / ____/ _/ / / / /_/ / / /
+/_ / / / /___/ _, _/ /___/ __/ _/ / \____/_/ /_/_____/_/ /___/ Developed By
+https://cappriciosec.com crlfi : Bug scanner for WebPentesters and Bugbounty
+Hunters $ crlfi [option] Usage: crlfi [options] ``` | Argument | Type |
+Description | Examples | | :-------- | :------- | :------------------------- |
+:------------------------- | | `-u` | `--url` | URL to scan | crlfi -u https://
+target.com | | `-i` | `--input` | filename Read input from txt | crlfi -
+i target.txt | | `-o` | `--output` | filename Write output in txt file | crlfi
+-i target.txt -o output.txt | | `-c` | `--chatid` | Creating Telegram
+Notification | crlfi --chatid yourid | | `-b` | `--blog` | To Read about crlfi
+Bug | crlfi -b | | `-h` | `--help` | Help Menu | crlfi -h | ## ð Links [!
+[Website](https://img.shields.io/badge/my_portfolio-000?style=for-the-
+badge&logo=ko-fi&logoColor=white)](https://cappriciosec.com/) [![linkedin]
+(https://img.shields.io/badge/linkedin-0A66C2?style=for-the-
 badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karthikeyan--
 v/) [![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-
 badge&logo=twitter&logoColor=white)](https://twitter.com/karthithehacker) ##
-Author - [@karthithehacker](https://github.com/karthi-the-hacker/) ## Feedback
-If you have any feedback, please reach out to us at contact@karthithehacker.com
+Author - [@cappriciosec](https://github.com/cappricio-securities/) ## Feedback
+If you have any feedback, please reach out to us at contact@cappriciosec.com
```

### Comparing `crlfi-0.0.2/cve/includes/bot.py` & `crlfi-0.0.3/cve/includes/bot.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/cve/includes/scan.py` & `crlfi-0.0.3/cve/includes/scan.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/cve/main.py` & `crlfi-0.0.3/cve/main.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/cve/utils/configure.py` & `crlfi-0.0.3/cve/utils/configure.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/cve/utils/const.py` & `crlfi-0.0.3/cve/utils/const.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/cve/utils/helpers.py` & `crlfi-0.0.3/cve/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `crlfi-0.0.2/setup.py` & `crlfi-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A Tool to find an Easy Bounty - crlfi'
 LONG_DESCRIPTION = 'This is a tool used by several security researchers to find Carriage Return Line Feed Injection Bug'
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
```

